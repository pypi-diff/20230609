# Comparing `tmp/pysoundanalyser-0.3.2.tar.gz` & `tmp/pysoundanalyser-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoundanalyser-0.3.2.tar", last modified: Mon Jun  5 08:15:05 2023, max compression
+gzip compressed data, was "pysoundanalyser-0.3.4.tar", last modified: Fri Jun  9 09:50:17 2023, max compression
```

## Comparing `pysoundanalyser-0.3.2.tar` & `pysoundanalyser-0.3.4.tar`

### file list

```diff
@@ -1,162 +1,169 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.2/COPYING.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.2/CREDITS.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.2/INSTALL.txt
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.2/MANIFEST.in
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/PKG-INFO
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.2/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.176185 pysoundanalyser-0.3.2/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.2/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.png
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.svg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.208185 pysoundanalyser-0.3.2/prep-release/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.259187 pysoundanalyser-0.3.2/prep-release/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.2/prep-release/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.2/prep-release/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.2/prep-release/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.2/prep-release/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.2/prep-release/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.2/prep-release/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.2/prep-release/debian/rules
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:03.694146 pysoundanalyser-0.3.2/prep-release/launchpad/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.357189 pysoundanalyser-0.3.2/prep-release/launchpad/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/rules
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.2/prep-release/launchpad_build.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.2/prep-release/make_deb.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/prep-release/minor_minor_number.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt6.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser.pro
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_de.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_el.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77435 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_en_GB.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_es.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    79000 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_fr.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93371 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_it.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77424 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_ru.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2652 2023-06-05 08:14:40.000000 pysoundanalyser-0.3.2/prep-release/release.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.2/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.2/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.2/prep-release/uploadToWebsite.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1527 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pyproject.toml
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.382190 pysoundanalyser-0.3.2/pysoundanalyser/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.2/pysoundanalyser/__init__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    80415 2023-06-03 15:22:30.000000 pysoundanalyser-0.3.2/pysoundanalyser/__main__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    13121 2023-05-20 15:42:12.000000 pysoundanalyser-0.3.2/pysoundanalyser/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11329 2023-05-20 15:31:32.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_apply_filter.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1993 2023-05-08 21:53:20.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_change_channel.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     4556 2023-05-20 15:31:53.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_concatenate.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2832 2023-05-20 15:32:08.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_cut.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    24487 2023-05-20 17:31:33.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_edit_preferences.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5932 2023-05-20 15:32:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_noise.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8214 2023-05-20 15:41:21.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sinusoid.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    34378 2023-05-20 15:32:58.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sound.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     6397 2023-05-20 15:33:11.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_get_font.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3684 2023-05-20 15:33:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_resample.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3287 2023-05-08 21:46:08.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_save_sound.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.386190 pysoundanalyser-0.3.2/pysoundanalyser/doc/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      634 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:03.696147 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.389190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.391190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.400190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    11185 2023-06-04 19:56:48.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alabaster.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1128 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_info_32.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      944 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       78 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/background_b01.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/basic.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       82 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bg-page.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9827 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1145 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      165 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bullet_orange.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      107 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/contents.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.401190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/theme.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14940 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       42 2017-05-15 18:58:47.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/custom.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/doctools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/documentation_options.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/file.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6714 2023-06-04 19:58:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/haiku.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/jquery.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.401190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/js/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/js/theme.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/language_data.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/minus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      120 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/navigation.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/plus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/pygments.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6263 2023-06-04 20:00:19.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/underscore.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3668 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/genindex.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5481 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/index.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6262 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/installation.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5815 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/intro.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      351 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/objects.inv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4067 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4231 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/searchindex.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9618 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/user_interface.html
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.402190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/latex/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   144787 2023-06-05 08:13:42.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      989 2023-06-05 08:13:31.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/conf.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/installation.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/intro.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      800 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/make.bat
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/mkdoc.sh
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/user_interface.rst
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11077 2023-05-21 07:35:18.000000 pysoundanalyser-0.3.2/pysoundanalyser/global_parameters.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2023-06-04 19:54:17.000000 pysoundanalyser-0.3.2/pysoundanalyser/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   108155 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1296 2023-04-30 11:36:30.000000 pysoundanalyser-0.3.2/pysoundanalyser/random_id.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.2/pysoundanalyser/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1598 2023-04-30 11:36:57.000000 pysoundanalyser-0.3.2/pysoundanalyser/threaded_plotters.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1432 2023-04-30 11:37:09.000000 pysoundanalyser-0.3.2/pysoundanalyser/utilities_open_manual.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10331 2023-05-20 14:57:23.000000 pysoundanalyser-0.3.2/pysoundanalyser/utility_functions.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.2/pysoundanalyser/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/wavpy_sndf.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7514 2023-05-20 15:34:46.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_acf_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     9305 2023-05-20 15:34:59.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_autocorrelogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    20600 2023-05-20 15:35:22.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_generic_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11904 2023-05-20 15:35:37.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_spectrogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8447 2023-05-20 15:35:51.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_spectrum_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5635 2023-05-20 15:36:13.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_waveform_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pysoundanalyser.desktop
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.384190 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5590 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/top_level.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.2/resources.qrc
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.403190 pysoundanalyser-0.3.2/scripts/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.2/scripts/pysoundanalyser-launcher.bat
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/setup.cfg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.421191 pysoundanalyser-0.3.2/translations/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_de.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_el.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_en_GB.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_es.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_fr.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    28965 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_it.qm
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_it_IT.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_ru.qm
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.393622 pysoundanalyser-0.3.4/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.4/COPYING.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.4/CREDITS.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.4/INSTALL.txt
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.4/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-09 09:50:17.392622 pysoundanalyser-0.3.4/PKG-INFO
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.4/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.724605 pysoundanalyser-0.3.4/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.4/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.png
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.svg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.778607 pysoundanalyser-0.3.4/prep-release/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.830608 pysoundanalyser-0.3.4/prep-release/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.4/prep-release/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.4/prep-release/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.4/prep-release/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.4/prep-release/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.4/prep-release/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.4/prep-release/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.4/prep-release/debian/rules
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.506599 pysoundanalyser-0.3.4/prep-release/launchpad/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.876609 pysoundanalyser-0.3.4/prep-release/launchpad/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.4/prep-release/launchpad/debian/rules
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.4/prep-release/launchpad_build.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.4/prep-release/make_deb.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/prep-release/minor_minor_number.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt6.sh
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      185 2023-06-08 22:08:52.000000 pysoundanalyser-0.3.4/prep-release/pypi_build.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser.pro
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_de.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_el.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77438 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_en_GB.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77410 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_es.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    79003 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_fr.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93374 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77427 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/prep-release/pysoundanalyser_ru.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3671 2023-06-08 22:19:59.000000 pysoundanalyser-0.3.4/prep-release/release.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.4/prep-release/switch_pyqt5.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.4/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.4/prep-release/uploadToWebsite.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      206 2023-06-08 22:09:58.000000 pysoundanalyser-0.3.4/prep-release/win_installer_readme.md
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      146 2023-06-08 22:10:19.000000 pysoundanalyser-0.3.4/prep-release/win_launch_iss_compiler.bat
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      521 2023-06-08 22:10:33.000000 pysoundanalyser-0.3.4/prep-release/win_launch_iss_compiler.sh
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3930 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/prep-release/win_pysoundanalyser.iss
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      768 2023-06-08 22:16:33.000000 pysoundanalyser-0.3.4/prep-release/winbuild.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1527 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/pyproject.toml
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.908610 pysoundanalyser-0.3.4/pysoundanalyser/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.4/pysoundanalyser/__init__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    82246 2023-06-09 09:38:11.000000 pysoundanalyser-0.3.4/pysoundanalyser/__main__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2023-06-09 09:49:37.000000 pysoundanalyser-0.3.4/pysoundanalyser/_version_info.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    13121 2023-05-20 15:42:12.000000 pysoundanalyser-0.3.4/pysoundanalyser/audio_manager.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11329 2023-05-20 15:31:32.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_apply_filter.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1993 2023-05-08 21:53:20.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_change_channel.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     4556 2023-05-20 15:31:53.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_concatenate.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2832 2023-05-20 15:32:08.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_cut.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    24487 2023-05-20 17:31:33.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_edit_preferences.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5932 2023-05-20 15:32:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_noise.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8214 2023-05-20 15:41:21.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sinusoid.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    34378 2023-05-20 15:32:58.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sound.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     6397 2023-05-20 15:33:11.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_get_font.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3684 2023-05-20 15:33:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_resample.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3287 2023-05-08 21:46:08.000000 pysoundanalyser-0.3.4/pysoundanalyser/dialog_save_sound.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.925610 pysoundanalyser-0.3.4/pysoundanalyser/doc/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      634 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.507599 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.928610 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.972612 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.313620 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11185 2023-06-04 19:56:48.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alabaster.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1128 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_info_32.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      944 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       78 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/background_b01.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/basic.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       82 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bg-page.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9827 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1145 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      165 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bullet_orange.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      107 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/contents.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.326620 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/theme.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14940 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       42 2017-05-15 18:58:47.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/custom.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/doctools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/file.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6714 2023-06-04 19:58:28.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/haiku.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.352621 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/theme.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/language_data.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/minus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      120 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/navigation.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/plus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/pygments.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6263 2023-06-04 20:00:19.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/underscore.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3668 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/genindex.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5481 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/index.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6262 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/installation.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5815 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/intro.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      351 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/objects.inv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4067 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4231 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/searchindex.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9618 2023-06-09 09:50:03.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/user_interface.html
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.365622 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   144833 2023-06-09 09:50:09.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      989 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/conf.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/installation.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/intro.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      800 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/make.bat
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/mkdoc.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/doc/user_interface.rst
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11077 2023-05-21 07:35:18.000000 pysoundanalyser-0.3.4/pysoundanalyser/global_parameters.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2023-06-09 09:38:00.000000 pysoundanalyser-0.3.4/pysoundanalyser/pyqtver.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   109505 2023-06-09 09:50:00.000000 pysoundanalyser-0.3.4/pysoundanalyser/qrc_resources.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1296 2023-04-30 11:36:30.000000 pysoundanalyser-0.3.4/pysoundanalyser/random_id.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.4/pysoundanalyser/sndlib.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1598 2023-04-30 11:36:57.000000 pysoundanalyser-0.3.4/pysoundanalyser/threaded_plotters.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1432 2023-04-30 11:37:09.000000 pysoundanalyser-0.3.4/pysoundanalyser/utilities_open_manual.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10331 2023-05-20 14:57:23.000000 pysoundanalyser-0.3.4/pysoundanalyser/utility_functions.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.4/pysoundanalyser/wavpy.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.4/pysoundanalyser/wavpy_sndf.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7514 2023-05-20 15:34:46.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_acf_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     9305 2023-05-20 15:34:59.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_autocorrelogram_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    20600 2023-05-20 15:35:22.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_generic_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11904 2023-05-20 15:35:37.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_spectrogram_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8447 2023-05-20 15:35:51.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_spectrum_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5635 2023-05-20 15:36:13.000000 pysoundanalyser-0.3.4/pysoundanalyser/win_waveform_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/pysoundanalyser.desktop
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:16.910610 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5809 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:16.000000 pysoundanalyser-0.3.4/pysoundanalyser.egg-info/top_level.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.4/resources.qrc
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.366622 pysoundanalyser-0.3.4/scripts/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.4/scripts/pysoundanalyser-launcher.bat
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-09 09:50:17.393622 pysoundanalyser-0.3.4/setup.cfg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      961 2023-06-09 09:49:38.000000 pysoundanalyser-0.3.4/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-09 09:50:17.392622 pysoundanalyser-0.3.4/translations/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_de.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_el.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_en_GB.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_es.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_fr.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    28965 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_it.qm
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_it_IT.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2023-06-09 09:50:01.000000 pysoundanalyser-0.3.4/translations/pysoundanalyser_ru.qm
```

### Comparing `pysoundanalyser-0.3.2/COPYING.txt` & `pysoundanalyser-0.3.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/MANIFEST.in` & `pysoundanalyser-0.3.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/PKG-INFO` & `pysoundanalyser-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.2
+Version: 0.3.4
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysoundanalyser-0.3.2/icons/exit.svg` & `pysoundanalyser-0.3.4/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.ico` & `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.ico`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.png` & `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.svg` & `pysoundanalyser-0.3.4/icons/johnny_automatic_crashing_wave.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/debian/changelog` & `pysoundanalyser-0.3.4/prep-release/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/debian/control` & `pysoundanalyser-0.3.4/prep-release/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/debian/copyright` & `pysoundanalyser-0.3.4/prep-release/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/debian/rules` & `pysoundanalyser-0.3.4/prep-release/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/launchpad/debian/changelog` & `pysoundanalyser-0.3.4/prep-release/launchpad/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/launchpad/debian/control` & `pysoundanalyser-0.3.4/prep-release/launchpad/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/launchpad/debian/copyright` & `pysoundanalyser-0.3.4/prep-release/launchpad/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/launchpad/debian/rules` & `pysoundanalyser-0.3.4/prep-release/launchpad/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/launchpad_build.py` & `pysoundanalyser-0.3.4/prep-release/launchpad_build.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/make_deb.py` & `pysoundanalyser-0.3.4/prep-release/make_deb.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt6.sh` & `pysoundanalyser-0.3.4/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser.pro` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser.pro`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_de.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_de.ts`

 * *Files 1% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_de.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_de.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -829,245 +829,245 @@
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_el.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_el.ts`

 * *Files 1% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_el.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_el.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -829,245 +829,245 @@
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_en_GB.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_en_GB.ts`

 * *Files 0% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_en_GB.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_en_GB.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished">Preferences</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -829,245 +829,245 @@
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_es.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_es.ts`

 * *Files 1% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_es.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_es.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -829,245 +829,245 @@
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_fr.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_fr.ts`

 * *Files 0% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_fr.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_fr.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished">&amp;Fichier</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished">Quitter</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished">&amp;Aide</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -859,245 +859,245 @@
       <source>L</source>
       <translation type="obsolete">G</translation>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_it.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts`

 * *Files 1% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_it.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_it.ts`

```diff
@@ -134,478 +134,478 @@
       <source>Grid</source>
       <translation type="obsolete">Griglia</translation>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation>&amp;File</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation>Esci</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation>Esci</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation>&amp;Modifica</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation>Preferenze</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation>Seleziona tutti</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation>&amp;Ottieni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation>&amp;Trasforma</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation>&amp;Applica Filtro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation>FIR2 Predefiniti</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation>&amp;Genera</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation>Tono AM</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation>Tono FM</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation>Rumore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation>Silenzio</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation>Sinusoide</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation>Onda sonora</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation>Spettro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation>Spettrogramma</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation>Autocorrelazione</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation>Autocorrelogramma</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation>&amp;Aiuto</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation>Manuale (html)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation>Manuale (pdf)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation>Riguardo pysoundanalyser</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation>Carica suono</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation>Salva come</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation>Clona suono</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation>Rinomina</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation>Rimuovi</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation>Rimuovi tutti</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation>Riproduci</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation>Grafico onda sonora</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation>Cambia Freq. Campionamento</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation>Scalare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation>Differenza di livello</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation>Concatena</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation>Sposta giù</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation>Sposta su</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation>Etichetta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation>Canale</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation>Nessuna Selezione</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation>Avviso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation>Si può spostare solo un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation>pysoundanalyser - Scegli file da caricare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation>Sinistro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation>Destro</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation>Impossibile aprire %1 IOError</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation>Nessuna selezione</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation>Selezione multipla</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation>Impossibile salvare suoni con frequenze di campionamento diverse</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation>Scegli il file da salvare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation>Tutti i file (*)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation>Si può cambiare solo il nome di un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation>Nuovo nome:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation>Dialogo di input</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation>Si può cambiare solo un suono alla volta</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation>Solo due suoni alla volta possono essere comparati</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation>Scalare il livello</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation>Aggiungi o rimuovi decibel</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation>Non è possibile riprodurre suoni con frequenza di campionamento diversa</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation>Concatena suoni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation>Solo due suoni alla volta possono essere concatenati</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation>Impossibile concatenare suoni con frequenze di campionamento differenti</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation>passabasso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation>passaalto</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation>passabanda</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation>fermabanda</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation>Entrambe</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation>Bianco</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation>Rosa</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation>Rosso</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation>Blu</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation>Viola</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="1181"/>
       <source>F0 (Hz)</source>
       <translation type="obsolete">F0 (Hz)</translation>
@@ -782,65 +782,65 @@
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="1218"/>
       <source>Harmonicity:</source>
       <translation type="obsolete">Armonicità:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation>IRN</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation>Pitch di Huggins</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation>IPD Lineare</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation>IPD a scalino</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation>ITD</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation>Nessuno</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation>Dispari a sinistra</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation>Dispari a destra</translation>
     </message>
     <message>
       <location filename="../pysoundanalyser/__main__.py" line="1270"/>
       <source>Frequency (Hz)</source>
       <translation type="obsolete">Frequenza (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -1143,245 +1143,245 @@
       <source>L</source>
       <translation type="obsolete">S</translation>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation>F0 (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation>Larghezza di banda (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation>Larghezza di banda (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation>Intervallo (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation>ITD (micro s)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation>IPD (radianti)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation>Livello componenti banda stretta (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation>Iterazioni</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation>Gain</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation>Armonica inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation>Armonica superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation>Frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation>Frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation>Stop inferiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation>Stop superiore</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation>Livello armonico (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation>Livello spettrale (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation>Livello componente (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation>Durata (ms)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation>Rampa (sm)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation>Rumore 1 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation>Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation>Livello rumore 1 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation>Rumore 2 frequenza inferiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation>Rumore 1 frequenza superiore (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation>Livello rumore 2 (dB SPL)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation>Allungamento (%)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation>Intervallo armonico (centesimi)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation>Orecchio:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation>Tipo:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation>Fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation>Tipo rumore:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation>Tipo IRN:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation>Relazione di fase:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation>Differenza dicotica:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation>Armonicità:</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation>Frequenza (Hz)</translation>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_ru.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_ru.ts`

 * *Files 1% similar despite different names*

#### Comparing `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_ru.ts` & `pysoundanalyser-0.3.4/prep-release/pysoundanalyser_ru.ts`

```diff
@@ -116,528 +116,528 @@
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="107"/>
+      <location filename="../pysoundanalyser/__main__.py" line="148"/>
       <source>Python Sound Analyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="115"/>
+      <location filename="../pysoundanalyser/__main__.py" line="156"/>
       <source>&amp;File</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="117"/>
+      <location filename="../pysoundanalyser/__main__.py" line="158"/>
       <source>Exit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="119"/>
+      <location filename="../pysoundanalyser/__main__.py" line="160"/>
       <source>Exit application</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="126"/>
+      <location filename="../pysoundanalyser/__main__.py" line="167"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="127"/>
+      <location filename="../pysoundanalyser/__main__.py" line="168"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="131"/>
+      <location filename="../pysoundanalyser/__main__.py" line="172"/>
       <source>Select All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="136"/>
+      <location filename="../pysoundanalyser/__main__.py" line="177"/>
       <source>&amp;Get</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="761"/>
+      <location filename="../pysoundanalyser/__main__.py" line="802"/>
       <source>Root Mean Square</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="142"/>
+      <location filename="../pysoundanalyser/__main__.py" line="183"/>
       <source>&amp;Process</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="143"/>
+      <location filename="../pysoundanalyser/__main__.py" line="184"/>
       <source>&amp;Apply Filter</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="144"/>
+      <location filename="../pysoundanalyser/__main__.py" line="185"/>
       <source>FIR2 Presets</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="150"/>
+      <location filename="../pysoundanalyser/__main__.py" line="191"/>
       <source>&amp;Generate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="151"/>
+      <location filename="../pysoundanalyser/__main__.py" line="192"/>
       <source>Harmonic Complex</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="154"/>
+      <location filename="../pysoundanalyser/__main__.py" line="195"/>
       <source>AM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="157"/>
+      <location filename="../pysoundanalyser/__main__.py" line="198"/>
       <source>FM Tone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="160"/>
+      <location filename="../pysoundanalyser/__main__.py" line="201"/>
       <source>Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="163"/>
+      <location filename="../pysoundanalyser/__main__.py" line="204"/>
       <source>Silence</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1265"/>
       <source>Sinusoid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="171"/>
+      <location filename="../pysoundanalyser/__main__.py" line="212"/>
       <source>&amp;Plot</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="172"/>
+      <location filename="../pysoundanalyser/__main__.py" line="213"/>
       <source>Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="235"/>
+      <location filename="../pysoundanalyser/__main__.py" line="276"/>
       <source>Spectrum</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="238"/>
+      <location filename="../pysoundanalyser/__main__.py" line="279"/>
       <source>Spectrogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="242"/>
+      <location filename="../pysoundanalyser/__main__.py" line="283"/>
       <source>Autocorrelation</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="245"/>
+      <location filename="../pysoundanalyser/__main__.py" line="286"/>
       <source>Autocorrelogram</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="234"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="236"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="199"/>
+      <location filename="../pysoundanalyser/__main__.py" line="240"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>About pysoundanalyser</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="253"/>
       <source>Load Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="256"/>
       <source>Save As</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="260"/>
       <source>Clone Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="223"/>
+      <location filename="../pysoundanalyser/__main__.py" line="264"/>
       <source>Rename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="267"/>
       <source>Remove</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="229"/>
+      <location filename="../pysoundanalyser/__main__.py" line="270"/>
       <source>Remove All</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="273"/>
       <source>Play</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="249"/>
+      <location filename="../pysoundanalyser/__main__.py" line="290"/>
       <source>Plot Waveform</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="252"/>
+      <location filename="../pysoundanalyser/__main__.py" line="293"/>
       <source>Resample</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="256"/>
+      <location filename="../pysoundanalyser/__main__.py" line="297"/>
       <source>Scale</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>Level Difference</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="264"/>
+      <location filename="../pysoundanalyser/__main__.py" line="305"/>
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="267"/>
+      <location filename="../pysoundanalyser/__main__.py" line="308"/>
       <source>Cut</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="312"/>
       <source>Move Down</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="315"/>
       <source>Move Up</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Label</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="285"/>
+      <location filename="../pysoundanalyser/__main__.py" line="326"/>
       <source>Channel</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="315"/>
+      <location filename="../pysoundanalyser/__main__.py" line="356"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="379"/>
+      <location filename="../pysoundanalyser/__main__.py" line="420"/>
       <source>Only one sound can be moved at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>pysoundanalyser - Choose file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="392"/>
+      <location filename="../pysoundanalyser/__main__.py" line="433"/>
       <source>Supported Sound Files (*.wav);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1387"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1428"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1384"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1425"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="489"/>
+      <location filename="../pysoundanalyser/__main__.py" line="530"/>
       <source>Cannot open %1 IOError</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="506"/>
+      <location filename="../pysoundanalyser/__main__.py" line="547"/>
       <source>No Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="517"/>
+      <location filename="../pysoundanalyser/__main__.py" line="558"/>
       <source>{0} is 
  {1} {2} dB than 
  {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="519"/>
+      <location filename="../pysoundanalyser/__main__.py" line="560"/>
       <source>Multiple Selection</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="531"/>
+      <location filename="../pysoundanalyser/__main__.py" line="572"/>
       <source>Duration: {0} sec.
 
 Channel: {1} 
 
 Samp. Freq.: {2} 
 
 Bits: {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="937"/>
+      <location filename="../pysoundanalyser/__main__.py" line="978"/>
       <source>No sound selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="568"/>
+      <location filename="../pysoundanalyser/__main__.py" line="609"/>
       <source>Cannot write sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="587"/>
+      <location filename="../pysoundanalyser/__main__.py" line="628"/>
       <source>Mono</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>Choose file to write</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>.{0}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="593"/>
+      <location filename="../pysoundanalyser/__main__.py" line="634"/>
       <source>All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="672"/>
+      <location filename="../pysoundanalyser/__main__.py" line="713"/>
       <source>Only one sound can be renamed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="678"/>
+      <location filename="../pysoundanalyser/__main__.py" line="719"/>
       <source>New name:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="679"/>
+      <location filename="../pysoundanalyser/__main__.py" line="720"/>
       <source>Input Dialog</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="687"/>
+      <location filename="../pysoundanalyser/__main__.py" line="728"/>
       <source>Only sound can be changed at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="705"/>
+      <location filename="../pysoundanalyser/__main__.py" line="746"/>
       <source>Only two sounds can be compared at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="717"/>
+      <location filename="../pysoundanalyser/__main__.py" line="758"/>
       <source>{0} is {1} {2} dB than {3}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Scale Level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="725"/>
+      <location filename="../pysoundanalyser/__main__.py" line="766"/>
       <source>Add or subtract decibels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="760"/>
+      <location filename="../pysoundanalyser/__main__.py" line="801"/>
       <source>{0} {1} : {2}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="776"/>
+      <location filename="../pysoundanalyser/__main__.py" line="817"/>
       <source>Cannot play sounds with different sample rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="838"/>
+      <location filename="../pysoundanalyser/__main__.py" line="879"/>
       <source>none</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="854"/>
+      <location filename="../pysoundanalyser/__main__.py" line="895"/>
       <source>No sounds selected.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Concatenate Sounds</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="857"/>
+      <location filename="../pysoundanalyser/__main__.py" line="898"/>
       <source>Only two sounds can be concatenated at a time</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="863"/>
+      <location filename="../pysoundanalyser/__main__.py" line="904"/>
       <source>Cannot concatenate sounds with different sampling rates</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cut Sound</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="925"/>
+      <location filename="../pysoundanalyser/__main__.py" line="966"/>
       <source>Values out of range</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="927"/>
+      <location filename="../pysoundanalyser/__main__.py" line="968"/>
       <source>Cannot cut entire sound, please use remove button</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="942"/>
+      <location filename="../pysoundanalyser/__main__.py" line="983"/>
       <source>lowpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="949"/>
+      <location filename="../pysoundanalyser/__main__.py" line="990"/>
       <source>highpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="956"/>
+      <location filename="../pysoundanalyser/__main__.py" line="997"/>
       <source>bandpass</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="965"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1006"/>
       <source>bandstop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1340"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1381"/>
       <source>Both</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="990"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1031"/>
       <source>White</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1287"/>
       <source>Pink</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="996"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1037"/>
       <source>Red</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1000"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1041"/>
       <source>Blue</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1004"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1045"/>
       <source>Violet</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1267"/>
       <source>Narrowband Noise</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1269"/>
       <source>IRN</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
       <source>Huggins Pitch</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Linear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1273"/>
       <source>IPD Stepped</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1275"/>
       <source>ITD</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1280"/>
       <source>None</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1240"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1281"/>
       <source>Odd Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1440"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1481"/>
       <source>&lt;b&gt;pysoundanalyser - Python Sound Analyser&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2010-2023 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -829,245 +829,245 @@
       <source>Concatenate</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>dialog</name>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1181"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1222"/>
       <source>F0 (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1182"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1223"/>
       <source>Bandwidth (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1183"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1224"/>
       <source>Bandwidth (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1184"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1225"/>
       <source>Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1185"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1226"/>
       <source>ITD (micro s)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1186"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1227"/>
       <source>IPD (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1187"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1228"/>
       <source>Narrow Band Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1188"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1229"/>
       <source>Iterations</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1189"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1230"/>
       <source>Gain</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1190"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1231"/>
       <source>Low Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1191"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1232"/>
       <source>High Harmonic</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1192"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1233"/>
       <source>Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1193"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1234"/>
       <source>High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1194"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1235"/>
       <source>Low Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1195"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1236"/>
       <source>High Stop</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1196"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1237"/>
       <source>Harmonic Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1197"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1238"/>
       <source>Spectrum Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1198"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1239"/>
       <source>Component Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1334"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1375"/>
       <source>Duration (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1308"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1349"/>
       <source>Ramp (ms)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1201"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1242"/>
       <source>No. 1 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1202"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1243"/>
       <source>No. 1 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1203"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1244"/>
       <source>No. 1 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1204"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1245"/>
       <source>No. 2 Low Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1205"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1246"/>
       <source>No. 2 High Freq. (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1206"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1247"/>
       <source>No. 2 S. Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1207"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1248"/>
       <source>Stretch (%)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1208"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1249"/>
       <source>Harmonic Spacing (Cents)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1335"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1376"/>
       <source>Ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1211"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1252"/>
       <source>Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1212"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1253"/>
       <source>Phase:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1213"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1254"/>
       <source>Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1214"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1255"/>
       <source>Dichotic Noise Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1215"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1256"/>
       <source>IRN Type:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1216"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1257"/>
       <source>Phase relationship:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1217"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1258"/>
       <source>Dichotic Difference:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1218"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1259"/>
       <source>Harmonicity:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1219"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1260"/>
       <source>Bandwidth Unit:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1270"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1311"/>
       <source>Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1271"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1312"/>
       <source>AM Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1272"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1313"/>
       <source>AM Depth</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1306"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1347"/>
       <source>Carrier Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1274"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1315"/>
       <source>Modulation Phase (radians)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1309"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1350"/>
       <source>Level (dB SPL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1303"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1344"/>
       <source>Carrier Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1304"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1345"/>
       <source>Modulation Frequency (Hz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../pysoundanalyser/__main__.py" line="1305"/>
+      <location filename="../pysoundanalyser/__main__.py" line="1346"/>
       <source>Modulation Index</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>generateNoiseDialog</name>
     <message>
```

### Comparing `pysoundanalyser-0.3.2/prep-release/release.py` & `pysoundanalyser-0.3.4/prep-release/release.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,22 @@
         sys.exit(2)
     for opt, arg in opts:
         if opt in ("-m", "--message"):
             message = arg
     major_v = 0
     minor_v = 3
 
+    pyqtver = input('pyqtver: ')
+    if pyqtver == 5:
+        os.system("python3 prep-release/switch_pyqt5.py")
+        os.system("python3 prep-release/mkupdate_pyqt5")
+    elif pyqtver == 6:
+        os.system("python3 prep-release/switch_pyqt6.py")
+        os.system("python3 prep-release/mkupdate_pyqt6")
+
     #read minor minor release number
     f = open('prep-release/minor_minor_number.txt', 'r')
     ln = f.readlines()
     f.close()
     minor_minor_v = int(ln[0].strip()) + 1
     #write incremented minor minor release number
     f = open('prep-release/minor_minor_number.txt', 'w')
@@ -75,14 +83,37 @@
         if ln[i].strip().split('=')[0].strip() == "Version":
             ln[i] = 'Version = ' + gittag +',\n'
 
     f = open('pysoundanalyser.desktop', 'w')
     f.writelines(ln)
     f.close()
 
+    f = open('setup_cx.py', 'r')
+    ln = f.readlines()
+    f.close()
+    for i in range(len(ln)):
+        if ln[i].strip().split('=')[0].strip() == "version":
+            ln[i] = '    version="' + gittag +'",\n'
+
+    f = open('setup_cx.py', 'w')
+    f.writelines(ln)
+    f.close()
+
+    f = open('prep-release/win_pysoundanalyser.iss', 'r')
+    ln = f.readlines()
+    f.close()
+    for i in range(len(ln)):
+        if len(ln[i].strip().split(" "))>1:
+            if ln[i].strip().split(" ")[1] == "MyAppVersion":
+                ln[i] = "#define MyAppVersion " + '"' + gittag + '"\n'#'    version="' + gittag +'"\n'
+
+    f = open('prep-release/win_pysoundanalyser.iss', 'w')
+    f.writelines(ln)
+    f.close()
+
  
     subprocess.call('git commit -a -m"' + message+'"', shell=True)
     #tag the commit so that it can be easily retrieved
     subprocess.call('git tag -a "' + gittag +'"' + ' -m "' + gittag +'"', shell=True)
     
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `pysoundanalyser-0.3.2/prep-release/switch_pyqt5.py` & `pysoundanalyser-0.3.4/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/switch_pyqt6.py` & `pysoundanalyser-0.3.4/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/prep-release/uploadToWebsite.py` & `pysoundanalyser-0.3.4/prep-release/uploadToWebsite.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pyproject.toml` & `pysoundanalyser-0.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysoundanalyser"
-    version="0.3.2"
+    version="0.3.4"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python program for visualizing short sounds (waveform, spectrum, etc...)"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/__main__.py` & `pysoundanalyser-0.3.4/pysoundanalyser/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,57 +12,98 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 #    You should have received a copy of the GNU General Public License
 #    along with pysoundanalyser.  If not, see <http://www.gnu.org/licenses/>.
 
-import argparse, sys, platform, os, copy, pickle, traceback
+import argparse, sys, platform, os, copy, logging, pickle, signal, scipy, time, traceback
 from pysoundanalyser.pyqtver import*
 if pyqtversion == 5:
     from PyQt5 import QtGui, QtCore
     from PyQt5.QtGui import QIcon
-    from PyQt5.QtWidgets import QAbstractItemView, QAction, QApplication, QDialogButtonBox, QGridLayout, QFileDialog, QInputDialog, QLabel, QMainWindow, QMessageBox, QPushButton, QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget
+    from PyQt5.QtWidgets import QAbstractItemView, QAction, QApplication, QDialog, QDialogButtonBox, QGridLayout, QFileDialog, QInputDialog, QLabel, QMainWindow, QMessageBox, QPushButton, QScrollArea, QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget
 elif pyqtversion == 6:
     from PyQt6 import QtGui, QtCore
     from PyQt6.QtGui import QAction, QIcon
-    from PyQt6.QtWidgets import QAbstractItemView, QApplication, QDialogButtonBox, QGridLayout, QFileDialog, QInputDialog, QLabel, QMainWindow, QMessageBox, QPushButton, QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget
+    from PyQt6.QtWidgets import QAbstractItemView, QApplication, QDialog, QDialogButtonBox, QGridLayout, QFileDialog, QInputDialog, QLabel, QMainWindow, QMessageBox, QPushButton, QScrollArea, QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget
 
-import logging, signal
-from pysoundanalyser import qrc_resources
 
 from numpy import sin, cos, pi, sqrt, abs, arange, zeros, mean, concatenate, convolve, angle, real, log2, log10, int_, linspace, repeat, ceil, unique, hamming, hanning, blackman, bartlett, round, transpose
 from numpy.fft import rfft, irfft, fft, ifft
-import scipy, time
 from tempfile import mkstemp
+
+from pysoundanalyser import qrc_resources
 from pysoundanalyser.global_parameters import*
 from pysoundanalyser._version_info import*
 from pysoundanalyser.utilities_open_manual import*
 from pysoundanalyser.threaded_plotters import*
 from pysoundanalyser.audio_manager import*
+
 __version__ = pysoundanalyser_version
 signal.signal(signal.SIGINT, signal.SIG_DFL)
 
-
-
 local_dir = os.path.expanduser("~") +'/.local/share/data/pysoundanalyser/'
 if os.path.exists(local_dir) == False:
     os.makedirs(local_dir)
 stderrFile = os.path.expanduser("~") +'/.local/share/data/pysoundanalyser/pysoundanalyser_stderr_log.txt'
 
 logging.basicConfig(filename=stderrFile,level=logging.DEBUG,)
 
 
+# def excepthook(except_type, except_val, tbck):
+#     """ Show errors in message box"""
+#     # recover traceback
+#     tb = traceback.format_exception(except_type, except_val, tbck)
+#     ret = QMessageBox.critical(None, "Critical Error! Something went wrong, the following info may help you troubleshooting",
+#                                     ''.join(tb),
+#                                     QMessageBox.StandardButton.Ok)
+#     timeStamp = ''+ time.strftime("%d/%m/%y %H:%M:%S", time.localtime()) + ' ' + '\n'
+#     logMsg = timeStamp + ''.join(tb)
+#     logging.debug(logMsg)
+
 def excepthook(except_type, except_val, tbck):
     """ Show errors in message box"""
     # recover traceback
     tb = traceback.format_exception(except_type, except_val, tbck)
-    ret = QMessageBox.critical(None, "Critical Error! Something went wrong, the following info may help you troubleshooting",
-                                    ''.join(tb),
-                                    QMessageBox.StandardButton.Ok)
+    def onClickSaveTbButton():
+        ftow = QFileDialog.getSaveFileName(None, 'Choose where to save the traceback', "traceback.txt", 'All Files (*)')[0]
+        if len(ftow) > 0:
+            if fnmatch.fnmatch(ftow, '*.txt') == False:
+                ftow = ftow + '.txt'
+            fName = open(ftow, 'w')
+            fName.write("".join(tb))
+            fName.close()
+    
+    diag = QDialog(None, Qt.WindowType.CustomizeWindowHint | Qt.WindowType.WindowCloseButtonHint)
+    diag.window().setWindowTitle("Critical Error!")
+    siz = QVBoxLayout()
+    lay = QVBoxLayout()
+    saveTbButton = QPushButton("Save Traceback", diag)
+    saveTbButton.clicked.connect(onClickSaveTbButton)
+    lab = QLabel("Sorry, something went wrong. The attached traceback can help you troubleshoot the problem: \n\n" + "".join(tb))
+    lab.setMargin(10)
+    lab.setWordWrap(True)
+    lab.setTextInteractionFlags(Qt.TextInteractionFlag.TextSelectableByMouse)
+    lab.setStyleSheet("QLabel { background-color: white }");
+    lay.addWidget(lab)
+
+    sc = QScrollArea()
+    sc.setWidget(lab)
+    siz.addWidget(sc) #SCROLLAREA IS A WIDGET SO IT NEEDS TO BE ADDED TO A LAYOUT
+
+    buttonBox = QDialogButtonBox(QDialogButtonBox.StandardButton.Ok|QDialogButtonBox.StandardButton.Cancel)
+
+    buttonBox.accepted.connect(diag.accept)
+    buttonBox.rejected.connect(diag.reject)
+    siz.addWidget(saveTbButton)
+    siz.addWidget(buttonBox)
+    diag.setLayout(siz)
+    diag.exec()
+
     timeStamp = ''+ time.strftime("%d/%m/%y %H:%M:%S", time.localtime()) + ' ' + '\n'
     logMsg = timeStamp + ''.join(tb)
     logging.debug(logMsg)
 
 if platform.system() == 'Windows':
     import winsound
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/audio_manager.py` & `pysoundanalyser-0.3.4/pysoundanalyser/audio_manager.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_apply_filter.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_apply_filter.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_change_channel.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_change_channel.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_concatenate.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_concatenate.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_cut.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_cut.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_edit_preferences.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_noise.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_noise.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sinusoid.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sinusoid.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sound.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_generate_sound.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_get_font.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_get_font.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_resample.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_resample.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/dialog_save_sound.py` & `pysoundanalyser-0.3.4/pysoundanalyser/dialog_save_sound.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/Makefile` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alabaster.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_info_32.png` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_info_32.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/basic.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/badge_only.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/theme.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/doctools.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/haiku.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/haiku.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/jquery.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/js/theme.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/language_data.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/pygments.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/searchtools.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/underscore.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/genindex.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>Index &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/index.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/installation.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/installation.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>Installation &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/intro.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/intro.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>What is pysoundanalyser? &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>What is pysoundanalyser? &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/search.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>Search &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/searchindex.js` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/user_interface.html` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/html/user_interface.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>User Interface &mdash; pysoundanalyser 0.3.2 documentation</title>
+  <title>User Interface &mdash; pysoundanalyser 0.3.4 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 15% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pysoundanalyser
-Release 0.3.2
+Release 0.3.4
 
 Samuele Carcagno
 
-Jun 05, 2023
+Jun 09, 2023
 
 CONTENTS:
 
 1
 
 What is pysoundanalyser?
 
@@ -46,15 +46,15 @@
 sounds generated for psychoacoustics research. pysoundanalyser can also generate some types of sounds used in
 psychoacoustics research (e.g. pure tones, amplitude modulated tones, frequency modulated tones, different colors of
 noise, etc. . . ).
 The repository of pysoundanalyser is hosted on GitHub. If you find bugs, please report them there.
 
 1
 
-pysoundanalyser, Release 0.3.2
+pysoundanalyser, Release 0.3.4
 
 2
 
 Chapter 1. What is pysoundanalyser?
 
 CHAPTER
 
@@ -80,15 +80,15 @@
 • PyAudio
 if you’re using Linux you can also install pyalsaaudio to have an addition sound output option. If you’re using conda
 on Windows I’d recommend installing PyAudio via pip because the PyAudio version available on conda is not built
 with support for the WASAPI output interface (at least that was the case the last time I checked).
 
 3
 
-pysoundanalyser, Release 0.3.2
+pysoundanalyser, Release 0.3.4
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
@@ -129,15 +129,15 @@
 • Spectrum Plot the spectrum of the currently selected sound.
 • Spectrogram Plot the spectrogram of the currently selected sound.
 • Autocorrelation Plot the autocorrelation function of the currently selected sound.
 • Autocorrelogram Plot the autocorrelogram of the currently selected sound.
 
 5
 
-pysoundanalyser, Release 0.3.2
+pysoundanalyser, Release 0.3.4
 
 • Level Difference Show the difference in level between two selected sounds.
 • Scale Change the level of the currently selected sound.
 • Resample Resample the currently selected sound.
 • Rename Rename the currently selected sound.
 • Remove Remove the currently selected sound from the workspace.
 • Remove All Remove all sounds from the workspace.
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/conf.py` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'pysoundanalyser'
 copyright = '2010-2023, Samuele Carcagno'
 author = 'Samuele Carcagno'
-release = "0.3.2"
+release = "0.3.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/installation.rst` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/intro.rst` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/make.bat` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/doc/user_interface.rst` & `pysoundanalyser-0.3.4/pysoundanalyser/doc/user_interface.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/global_parameters.py` & `pysoundanalyser-0.3.4/pysoundanalyser/global_parameters.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/qrc_resources.py` & `pysoundanalyser-0.3.4/pysoundanalyser/qrc_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,243 @@
 # -*- coding: utf-8 -*-
 
 # Resource object code
 #
-# Created by: The Resource Compiler for PyQt5 (Qt v5.15.8)
+# Created by: The Resource Compiler for PyQt5 (Qt v5.15.2)
 #
 # WARNING! All changes made in this file will be lost!
 
 from PyQt5 import QtCore
 
 qt_resource_data = b"\
+\x00\x00\x0d\xee\
+\x00\
+\x00\x40\xee\x78\x9c\xed\x5a\x59\x73\xdb\xc8\x11\x7e\xf7\xaf\x60\
+\xe8\x17\xbb\x96\x04\xe7\x3e\x68\x49\x5b\x8e\x5d\x9b\xda\x94\x92\
+\xad\x5a\xef\x56\x1e\x53\x10\x38\x92\xb0\x06\x09\x06\x00\x25\xd1\
+\xbf\x3e\xdd\x00\x88\x83\x1c\x4a\xa0\xac\xdd\xa4\x12\x93\x76\x89\
+\xe8\xe9\x39\xfa\x9b\x3e\x67\x70\xf6\xfd\xc3\x32\x19\xdd\xb9\x2c\
+\x8f\xd3\xd5\xf9\x98\x06\x64\x3c\x72\xab\x28\x5d\xc4\xab\x9b\xf3\
+\xf1\xaf\xbf\xfc\x30\x35\xe3\x51\x5e\x84\xab\x45\x98\xa4\x2b\x77\
+\x3e\x5e\xa5\xe3\xef\x2f\x5e\x9d\xfd\x69\x3a\x1d\x7d\xc8\x5c\x58\
+\xb8\xc5\xe8\x3e\x2e\x6e\x47\x3f\xae\x3e\xe7\x51\xb8\x76\xa3\x37\
+\xb7\x45\xb1\x9e\xcf\x66\xf7\xf7\xf7\x41\x5c\x13\x83\x34\xbb\x99\
+\xbd\x1d\x4d\xa7\xd0\x33\xbf\xbb\x79\x35\x1a\x8d\x60\xda\x55\x3e\
+\x5f\x44\xe7\xe3\x9a\x7f\xbd\xc9\x92\x92\x6f\x11\xcd\x5c\xe2\x96\
+\x6e\x55\xe4\x33\x1a\xd0\xd9\xb8\x65\x8f\x5a\xf6\x7b\x77\x15\x64\
+\x2e\x4f\x37\x59\x54\x0d\x1f\x45\x5d\xce\x6c\x71\xdd\xb2\xc2\x4a\
+\xee\x79\xc9\x44\xad\xb5\x33\xc2\x66\x8c\x4d\x81\x63\x9a\x6f\x57\
+\x45\xf8\x30\x5d\xe5\xaf\x3b\x5d\x61\x81\xbe\xae\x8c\x10\x32\x83\
+\xb6\x96\x73\x18\xd7\xfc\x21\x01\x18\x8e\x2e\xa6\x6c\xed\xce\x0e\
+\xd0\xaf\xe1\x7f\xd3\xa1\xc1\xb0\x92\xf5\x1a\x7a\xba\x60\xe5\x8a\
+\xd9\xc7\x5f\x3e\xce\x76\xdc\x53\x12\x2c\x8a\x45\x67\x98\x5d\xaf\
+\xde\xbc\xbd\xed\x58\x85\x4b\x97\xaf\xc3\xc8\xe5\xcd\x14\x65\xff\
+\xdd\xc3\xdc\x3d\xac\xd3\xac\x98\x6e\x17\x6b\x58\x8c\x25\x01\x29\
+\x3f\x5e\x9e\x87\x01\x3c\xd7\x71\xe2\x70\xce\xf3\xf1\xec\x36\x5d\
+\xba\xd9\x6f\xf1\x72\x19\x46\xb3\x8f\x2e\xff\x5c\xa4\xeb\xd9\x7d\
+\x0c\x1c\xc1\x7a\x55\x21\x77\x1f\x2f\x8a\xdb\xf3\xb1\x30\xeb\x87\
+\xf2\xf9\xd6\xc5\x37\xb7\x45\x87\x10\x2f\xce\xc7\x00\x33\xa5\xbc\
+\x9e\x6e\x87\xc4\xbc\xd1\x65\x12\x70\xd6\x5f\x49\xa7\x49\xf0\xef\
+\x16\xee\xce\x25\xfd\xbe\x8b\x34\xba\x0a\xf3\x66\x89\x45\x7c\xe3\
+\xb2\x62\x16\xdd\xe5\xb3\xeb\xcc\xb9\x45\xb5\xd4\x12\x3d\xb0\x88\
+\x9b\x74\x1a\x47\xe9\x6a\x5a\xdc\x82\xb2\xce\x60\x86\x24\xbc\x4a\
+\xdc\x2c\x8c\x0a\x98\x23\x3f\x18\xb8\x92\x3d\xdf\xe6\x85\x5b\x4e\
+\x93\xf4\x66\x9a\x6e\x8a\x60\xa7\x29\xcd\x12\x81\xb8\xde\x14\xff\
+\x74\x0f\x85\x5b\x55\x6b\x85\xd9\x3a\x1b\x57\x36\x63\xb7\x86\x36\
+\xbe\x80\x01\xce\x16\xee\x3a\xc7\x81\x2a\x64\xf0\x89\x97\x0d\xd0\
+\x04\x0a\xe6\xc2\xec\x2f\x59\xb8\x88\xc1\xa6\x2a\xa6\x8a\xad\xdf\
+\x62\x8d\x55\x75\x1f\xe8\x95\x83\xa4\x3b\xde\x1a\x6e\xa0\x00\x8f\
+\x19\xb7\xe4\xf4\xfa\x3a\x77\xb0\x2d\xa4\x43\xcb\x8b\x6d\xe2\x2a\
+\xee\x69\x94\x26\x69\x36\x7f\x1d\x39\xfc\xbe\x2b\x49\x29\xa8\x5c\
+\x5c\x6c\xe7\xf4\xdd\x78\x34\x7b\x6a\x36\x4b\x88\x67\x36\x5a\xab\
+\xd9\x13\xb3\x5a\x87\xdf\xbd\x59\x77\x5d\xdb\xd9\xcf\x66\x7d\x18\
+\x4e\x46\xcd\xb4\x88\x34\xdb\x08\x4b\x48\x5c\x04\x6b\x0d\x93\xfb\
+\x70\x9b\x0f\x80\xd5\x27\xe8\x13\x02\x5e\x97\x9f\x67\xc0\x6a\x2c\
+\xf3\xc1\x7a\xfa\x6c\x2f\x0a\x23\x79\x01\x18\x8d\x4f\xb0\x27\x60\
+\x94\x0c\xbf\xcf\x81\xd1\x88\xd3\x61\xf4\xcd\xf6\x92\x30\x2a\x73\
+\x0c\x25\xcf\x62\x84\xc3\xef\x51\x13\xf1\x40\xe9\x31\xbd\x16\x0f\
+\x4d\x8e\xa3\xe6\x99\x5d\x51\xfc\xee\x41\xf1\xd8\xec\x3e\xc3\xef\
+\xcc\xce\x5e\x0e\x45\x29\x9e\xd6\x35\xa9\x06\x02\x74\x3a\xf0\x03\
+\x74\x4f\xfa\xfc\xf0\x40\xcf\x18\x5e\xe1\xf7\xf7\xf7\x8c\x82\xbd\
+\x80\x49\x0b\x9f\x91\x3d\x21\xa0\x66\xda\x91\xf0\x39\x26\x2d\x7c\
+\x9b\xfa\x84\x49\xfb\x66\x7b\x49\x18\x39\x79\x1a\x25\xee\x75\x7c\
+\xc3\xd4\x41\x12\xfc\x7e\x8d\x32\x72\xaf\x23\x1c\x36\x3b\x35\xf8\
+\x7d\x61\x65\x3c\xa6\x6d\xc7\x61\x36\x4a\xb1\x13\x3c\x67\xbd\xbc\
+\x7d\x0d\x7b\x5c\x53\x77\x80\xc1\x5c\xe2\x24\x4f\xe9\x9b\xcd\xef\
+\x21\xfd\xb3\xa9\x3f\x10\x46\x79\x54\x5b\x87\xa7\x30\x43\x61\x94\
+\xec\x24\x18\x8f\xa4\x30\x43\x61\x94\xe2\x29\x18\xf1\x29\x4c\x4e\
+\x86\xb1\xac\x01\xe7\xb7\x99\x83\x9a\xf5\xb5\x07\xcf\x2e\xdc\xfd\
+\x29\xa0\xb9\x75\x58\xd1\x03\xac\xdc\x06\x9a\x50\x2a\x5a\x09\xa2\
+\xed\xf9\x98\x05\x90\xdb\x5b\x6e\x5a\xea\xb5\x97\xf7\xda\xcb\x9b\
+\x01\xab\x0e\xa8\x06\x4e\xd9\x10\x6f\xea\x15\xfc\x92\x85\xab\x1c\
+\x8a\xd2\xe5\xf9\x78\x19\x16\x59\xfc\xf0\x86\x06\x4c\x72\x21\xd8\
+\x64\xca\x02\x66\x15\xb5\xd2\x4d\xa9\x9a\xd0\x40\x0b\x2d\x14\x29\
+\x1f\x48\x60\x25\x87\xec\x7e\x32\xa5\x32\x10\xda\x12\x33\xa1\xd0\
+\x4f\x2b\xc5\xdf\x1e\x4c\xf1\xeb\x2a\x2e\xa0\xd8\xde\xe4\x2e\xfb\
+\x84\x05\xeb\x4f\xab\x5f\x73\xd7\x6e\x85\x1f\x74\x5c\xb4\x0c\x94\
+\x10\x9a\xeb\x9e\x7c\x5c\x05\x82\x51\xca\x74\x0f\x0b\x26\x02\xc3\
+\x35\x65\xaa\x87\xdb\x21\x6f\xe4\xe5\x7d\x0c\x8c\xca\x76\x27\xc4\
+\xf3\x43\x72\xa5\x19\x07\x64\x94\xe6\x52\x23\x4c\x72\x42\x55\x60\
+\x34\x27\x6a\x28\x0c\xc7\x75\xc3\x9a\xce\x0a\x1f\x55\x31\x35\x20\
+\x4e\x3f\x01\xf7\xb0\x45\x1e\xc7\x89\x01\x2a\xca\x12\x3d\x11\x81\
+\x90\x8a\x31\x53\xaa\xc9\x54\x06\x46\x4a\x4b\x69\xf9\xc4\x02\xc5\
+\x35\x53\x06\x94\x46\xf0\x40\x6a\x64\x50\x34\xb0\x40\xa5\x6f\x7b\
+\xda\xaa\xa0\xf4\xa7\x92\x8a\xde\xc6\x0b\x00\x5c\x40\xa4\x63\xbd\
+\x8d\xb7\x3c\xd0\x86\x90\x8e\x92\x44\x5e\xde\xc8\xcb\xeb\x43\x9d\
+\x0f\x42\xbd\x0c\xeb\xc3\x51\xf7\x3b\xe8\x67\xea\x9d\xe2\x12\xc0\
+\x69\x29\x60\x28\x56\x18\x2b\x4e\xd5\xb9\x2d\x03\x63\x30\x01\x18\
+\x08\x58\x79\x2b\x34\x50\x39\x18\x38\x97\x96\xb5\x4e\x64\x4b\x01\
+\x55\xc0\x4f\x82\xaa\x77\x78\xa9\x8f\xd7\x9b\x4b\x9a\x61\xa8\x0e\
+\xc9\x39\x07\xa2\x3a\x40\x78\x0d\x02\x59\x50\xdc\x9e\xf0\xd4\x04\
+\x84\x53\xb6\x27\x3c\x78\x5b\x43\x04\xa5\xba\x27\xbc\x00\x73\x17\
+\xd2\x30\xf9\xa8\xf0\x4a\x0c\x13\x5e\x8a\xff\x02\x43\x96\x9c\x08\
+\x2d\x27\x32\x20\x20\x99\x54\x60\xba\x06\x43\x01\x37\xcc\x6a\x34\
+\x6b\x01\x0e\x4f\x10\xce\x14\x44\x08\x70\xb0\xda\x4a\x0a\xbf\x6c\
+\x20\x0c\xe7\x84\xf7\x0c\x19\x02\x14\x63\x9a\x76\xaa\x7a\x34\x64\
+\x88\x45\xdc\x2a\xa2\x49\xcf\x90\x61\x2f\x8c\xe1\xf0\xaf\x67\xc8\
+\x87\xbc\x91\x97\xd7\x67\xc8\x7a\xa0\x21\xab\x01\x07\x40\xa7\x1b\
+\x72\x81\x3f\x93\xb0\x70\x6f\xa6\x14\x4c\x4c\x51\xd6\xda\xf0\xb3\
+\x0c\x55\x04\x5a\x81\xaa\x89\xbe\xa1\x0a\x18\x52\x0b\xaa\xf6\x75\
+\x95\x12\xad\xd9\x9e\xa1\x52\xf0\xc6\x0c\xb6\xeb\x51\x5d\x35\x03\
+\x51\x1b\x72\xde\xf3\x62\x86\x0a\x9e\x47\x08\x6b\x85\xee\x1b\x2a\
+\xe8\x97\x94\xb2\xe3\x5a\x4a\xe1\x79\x00\x69\x08\x80\xd2\x13\xde\
+\x00\x7a\x10\xa2\xc4\xe3\xc2\xdb\x81\x86\x3a\xe4\xcc\xf0\xc5\x84\
+\x47\x7f\xa4\xc0\xe2\xf6\x5c\x34\x38\x63\x4a\x94\xec\x7b\x29\x46\
+\x03\x49\x29\x35\x72\x7f\xe7\x89\x36\x56\x3e\xea\xa5\x2c\x61\xc3\
+\x84\xb7\x6a\xa8\xf0\x67\x33\x3c\xc9\x2e\x7f\x35\x47\xe9\x78\x8e\
+\xbe\xb8\x8b\xdd\x7d\x35\x46\x5e\x64\xe9\x67\xc8\xf3\x5f\x87\xa2\
+\x53\x6b\x5e\xc7\x49\x02\xb4\xaa\x32\xaf\x69\xb8\x64\x3c\xdd\xaf\
+\x1f\xd7\xe1\x8d\x2b\xeb\x02\xe0\xab\x0a\x83\xba\xe1\x2a\xcd\x16\
+\x2e\xdb\x35\xa9\xf2\xd3\x6b\xaa\x4b\x07\xac\xaf\x99\x14\x96\xd0\
+\x46\xa0\x46\x1c\x1c\xbc\xc3\x46\x7c\xed\xf9\x6d\xb8\x48\xef\x01\
+\xf2\xfd\xc6\x2f\x69\x0a\xf6\x0f\xc9\xab\x54\xe0\xd1\x0f\x9a\xd1\
+\x81\x71\x1d\x60\x08\x27\x07\x03\x97\xd9\x3e\xd8\xb4\x30\xd4\xd3\
+\x73\x93\x65\xb0\x03\xd3\x24\xdc\x3a\x90\xad\xfc\xb3\xdb\xfe\xfc\
+\x36\xbd\xbf\xc9\x10\xa3\xeb\x30\x69\x40\x6a\xba\x62\xd3\xf4\xea\
+\x2a\x7d\x40\xc7\xb4\x39\x68\x5e\xa4\xd1\x06\x6f\xec\xa6\x9b\x4a\
+\x1b\xeb\x5b\x9a\x0e\x07\x8e\xdf\x95\xda\x3b\xcb\x7d\xbc\x82\xc6\
+\x69\x7d\xfb\xa3\xe9\x01\xae\x35\xc3\xee\x3a\x48\x37\x01\x6f\x9f\
+\x03\x9d\xbc\xa2\x47\x1a\xb7\x68\xfa\x74\xa7\x63\x4b\x57\x84\x8b\
+\xb0\x08\x5b\x2d\xd9\x51\x76\x87\x80\x67\xd9\xe2\x7a\xfe\xf3\xc7\
+\x1f\x9a\x4a\x33\x8a\xe6\xff\x48\xb3\xcf\x6d\x91\x88\x0c\xe1\x55\
+\xba\x81\x35\x35\xd5\x2f\xde\xca\x44\x73\x74\xe6\x61\x71\x11\x2f\
+\x41\x76\xbc\x18\xfc\xee\x61\x99\x80\x5a\x37\x0d\x3d\xe6\x62\xbb\
+\x76\xed\xa0\xd5\xb0\xbb\x4b\x4e\xef\x45\xe9\x22\x5a\xc6\xd8\x69\
+\xf6\xa9\x00\x8d\xff\x11\x27\xe9\x54\xc4\xd5\xa0\x11\x5e\xd3\xa6\
+\xd9\x45\x67\x60\x14\xe0\xfd\x4d\x53\xb7\xf6\x96\x10\x17\x89\xbb\
+\xf8\x6b\xf8\x79\x73\x35\xfa\x54\x38\x30\xdd\xac\x5c\x6e\x45\xef\
+\x8e\x31\x3b\x1c\xa4\xe4\x3c\x98\x0f\x87\xad\x64\xb8\xa8\x45\xa8\
+\xee\xfe\x82\xe5\x26\x8f\xa3\xdb\x30\x49\x82\xe8\x4b\xd9\xb5\xe6\
+\x6a\x7b\xc2\x14\x49\x1c\xb9\x55\xfe\x34\x2c\xe5\xb4\xf1\x1d\xd8\
+\xf4\x72\x99\xae\xf2\x12\xa1\xba\x6f\x3e\xbb\xda\x4e\xf3\x70\x06\
+\x45\xc6\xec\x00\x9e\x4a\xb0\x4f\xe5\xbd\xdc\xe8\x32\xbd\x19\xfd\
+\xb4\x29\x7c\x12\x97\x52\x6c\xae\x7e\x03\x2f\xd5\x83\x01\x17\xf3\
+\xe7\xf0\x66\x0f\x49\xa4\x26\xf1\x45\x02\xe3\xa5\x38\x5e\xfd\x7c\
+\x8c\xe9\x49\x1e\xf7\x10\x7b\x39\x2a\x5a\x6f\xfe\x0a\xc9\xfe\x4a\
+\xcb\xcd\x42\x95\xed\xaa\xf0\xe5\x3e\xb2\x1d\x2d\x3e\x11\xd4\xfe\
+\x96\xad\x5d\x06\x6a\x99\x3f\xb9\x65\xbe\x3b\xfc\x9f\xdd\x3a\x4b\
+\x17\x9b\xf2\x12\xb5\xbf\x57\x5f\x39\xf0\xc7\x18\x42\x45\x7c\xb5\
+\xf1\x0e\x9c\xb9\x7f\x6d\x62\xe8\xf1\xac\x91\xff\x9e\x16\x00\xc9\
+\xcb\x8e\xf9\xbe\x38\xbe\xd8\xaf\x42\xc1\x65\xf1\x5d\xb9\xa5\xa8\
+\x0d\xf9\xcb\x2e\xfa\xd3\x6d\x98\xb9\xf7\x49\xfc\xb9\x0b\x46\xa9\
+\x7a\xb5\xaa\xed\x0e\xcf\x3a\xfe\xf4\x6c\xb6\xf3\xb6\xe5\xd3\x4d\
+\xeb\x85\x7b\xe1\xa9\x71\xe1\x49\x78\xe5\x20\xb4\x5f\x62\xe3\xe8\
+\xa0\xf5\x26\x4b\x37\xeb\x65\xba\x70\x75\xf7\xc6\x81\x83\x2d\x34\
+\x75\x45\x19\x92\x35\x81\xec\x47\x74\x92\xbc\xec\xc1\x4b\x2e\x4f\
+\xc4\x20\x10\xf3\x5e\x6e\x57\x65\x89\x90\x27\x91\x36\x25\x6a\xde\
+\x51\xa0\x78\x82\x46\x3a\xd5\x43\x1d\xcf\x30\x7f\xa6\xb6\xdb\xa5\
+\xac\x3a\x60\x69\xd6\xb0\x36\x21\xac\x0f\x2e\x0f\xcf\xc2\xfb\x87\
+\xc1\x98\xe2\xcc\x21\x14\xbc\x79\x7d\x78\x00\xf1\xb6\x6c\xf5\x1c\
+\xa7\x97\xe4\x6c\x93\xb8\xb9\xbb\x73\xab\x74\xb1\x78\x57\xe5\x4f\
+\x9d\x23\x66\x7c\xac\x22\x70\xa7\x5f\x4d\xc6\x4c\x0e\x70\x9e\x83\
+\x62\x16\x5d\xda\x6f\x69\xbc\x9a\x83\x4e\xba\xec\xdd\x32\xcc\x3e\
+\xbb\x6c\xbe\x4a\x57\xae\xfe\x3d\xcd\x8b\x30\x2b\x7a\x94\x65\xbc\
+\xe8\x3d\xbb\x55\xfd\x5c\x8f\x59\x0e\x95\xc4\xf0\x67\x4e\x77\x35\
+\xcf\xae\x6d\x11\x42\x0a\x91\x65\xe1\xb6\xd7\x03\xa9\xd5\xe9\x6d\
+\xe7\x0a\xb1\x6e\x3b\x84\xe1\x2e\xce\xe3\xab\x38\x41\x62\xf9\x33\
+\x71\xef\x16\x71\xbe\x06\x95\x99\xc7\x2b\x14\xe8\x5d\x7a\xe7\xb2\
+\xeb\x24\xbd\xdf\xb5\x77\xca\xe6\x8e\x2a\x6d\xcb\x4d\xd5\x5c\xc9\
+\xce\xb1\x03\x2a\x87\x08\x84\x05\xa5\x31\x07\xca\x41\xc1\x5d\x32\
+\x62\x3a\x07\xa9\x3b\xe5\x80\x64\x92\x99\x6e\x43\xab\x1c\x82\x3c\
+\x5f\x39\x0e\xcf\x51\x4e\x57\x8e\x2e\xd0\xdf\x34\xe3\xa8\x66\xac\
+\xc3\xe2\xb6\xd9\xa7\xa6\x5c\x01\x67\x84\x19\x1a\x24\xc5\x11\x7e\
+\x7a\xdb\x8b\x3d\xac\xe9\x9c\x32\x02\xed\x6f\x23\xd0\x1e\x4e\x8d\
+\xa5\x6c\xd2\x1c\x98\x8d\x2e\x91\x4a\x8d\xe2\xcc\x4e\x78\x40\xa4\
+\xc0\xb7\x08\x80\x0a\x55\x9c\x15\x94\x32\x89\x54\x6b\x34\xb5\xa2\
+\xa6\x1a\xc9\x29\xf0\x02\x99\x1a\xaa\x65\x35\xc2\xc1\xb8\x5f\x46\
+\x07\xaa\xb5\x27\xdf\xbe\xfc\x1e\x84\x8e\xa2\x39\x60\x0b\xfc\x9b\
+\xe6\xdd\xe6\x7d\x95\x38\xa2\x32\x07\x4a\xd5\x1b\x79\x4f\x29\x1f\
+\x51\x5f\xbf\xa6\x57\x83\x1d\x9a\xca\xbe\x4d\x3d\x62\x82\x4a\xbc\
+\xdd\x33\xd7\x03\xe4\xfc\xee\xa6\xd2\x0e\x19\x48\xc6\x8d\x22\xb0\
+\xe3\x96\x59\x08\x58\x72\xf4\x01\xa9\x94\x33\xca\x44\x87\x0a\xfb\
+\x6d\xa8\xd2\x52\x4e\x44\xc0\x84\x84\x88\x24\x7a\x34\xc5\x95\xa1\
+\x4c\x55\x9a\xb1\xa3\xb2\x00\xcf\xcb\x14\xc5\x31\xbb\x54\x6d\xb4\
+\xb6\xba\x33\x0f\xe8\x10\x25\x9c\x2a\xd5\x59\x51\x4b\xbb\x1c\xc1\
+\x6f\x65\x15\x97\xaa\x43\xfd\x30\x12\x50\x9b\x1a\x43\x2c\xef\x50\
+\x81\x26\x08\x17\x8a\x76\xe6\xe9\xd1\xea\x15\x5d\x76\xa9\xcd\xea\
+\x3f\xf4\xa8\x3b\x39\xdb\x79\x5a\x3c\xda\x15\xb5\xb4\x4b\x2f\x9e\
+\xdf\xac\x62\xa0\x55\xb0\x26\x7f\xa8\xef\x56\x9f\x36\x8c\x6e\x84\
+\x2a\x97\xe0\x37\x05\x12\x70\xd8\xe0\x5e\xec\x6b\x03\x22\x37\xfb\
+\xe1\x93\xd9\x00\x7c\x1f\xeb\x9c\x14\xef\x22\x2e\xb7\x81\x95\x94\
+\xf3\xfd\x00\xad\x8c\xa0\x9a\x77\xf3\x3c\x0e\x41\x5b\x49\xbc\x51\
+\x7d\xdc\xa5\xa3\x3b\x3f\x1f\x87\x59\x74\x2c\x2a\x43\x28\xb7\x56\
+\x28\xc9\xe8\xe0\x9c\x8d\x3d\x23\x67\xfb\x16\x96\x1f\x0b\xcb\xfb\
+\x71\xd6\x28\xd5\x49\xa3\x76\x7b\xe9\xbf\xcf\x6d\x9b\xbd\x97\xc0\
+\x4d\x33\xd6\x0c\x87\xb7\xcc\x6d\xf3\x16\xcf\x8d\xc1\x7b\x19\xcb\
+\x65\x3f\xc6\x0b\x12\x08\x83\xf1\x7c\xd4\x0c\x3f\x7a\x3f\x6a\xc6\
+\x1a\x35\xdd\x46\x64\x44\xe1\x3b\xb2\x01\xa8\x37\x37\x06\x02\xfd\
+\xb0\x0e\xbe\x19\xbe\x34\x8b\x28\x0e\x2e\x6e\xa0\xf6\xd1\x46\x58\
+\xff\x8d\x61\xdd\x34\xd5\x81\xd4\xd6\xe0\x35\x75\x20\xe1\x2f\xb7\
+\x6f\x8f\xd8\xca\x09\x69\xea\xeb\x28\x6a\xf5\xfc\x94\x92\xa5\x3a\
+\xf1\xed\x5b\x00\x09\x6c\xf9\x31\x6c\xdf\x04\xa0\x32\x5c\x2d\x0e\
+\x6c\xa0\xa2\xfe\xaf\xdb\x40\x95\x38\x40\xa1\x42\x71\xf7\x26\x14\
+\xb6\x11\xdf\xf0\x28\xd3\xca\x86\x0a\x15\x08\x97\x92\x2b\x4c\x20\
+\x6d\xa0\x94\x80\xf0\x2c\x8e\x51\x55\x40\xb5\xa2\x42\x03\x95\x41\
+\x59\x0b\x41\x5b\xc8\x09\x83\x08\x0a\x79\x29\xe1\x25\xaf\xb4\x94\
+\x0b\x48\x14\x28\xc5\x93\x6c\x4a\x68\x9f\x8a\x6b\xd0\x44\xe9\xde\
+\x1a\xda\x95\x75\x42\x70\x6b\xc1\x82\x1f\x1a\xd9\x7e\x82\x8d\x39\
+\xf6\x10\x9d\x24\x81\x24\x86\x30\x2a\x86\x3a\x69\x7c\xd7\xe6\x77\
+\x75\xd2\xff\xf7\x1a\x0a\x91\x9a\x81\x4d\x1b\xd0\x0e\x16\x08\x6d\
+\x88\xa8\x34\xa9\xa1\xea\x00\x37\xa1\x4c\x05\xa1\x8e\xd6\x90\xf2\
+\x49\x7a\x84\x0a\x4e\x1d\x0a\x20\x21\x08\x26\xb2\x90\x42\x72\xa8\
+\x97\x80\x8a\x27\x3c\x1c\x9d\x22\x68\xa5\x95\xc2\x5a\x36\xc1\x4b\
+\x7c\xcd\xa1\x76\x42\x4d\x66\x56\x30\x43\x4a\x4d\x16\xa8\xeb\xfd\
+\xf9\x9b\x55\xf9\xb5\x53\x0e\xd0\xce\x13\xcb\x45\x5f\xc5\x08\xd2\
+\x9a\x3e\x70\x0c\x93\x1f\x90\xd0\x4e\x28\xc6\x01\x70\x7f\xb2\x04\
+\x63\x47\x85\xec\x08\x4c\x98\xb0\xd2\xe0\x41\xf1\x4b\x64\x8e\x50\
+\xf1\x5e\xd0\x72\xab\x91\x0a\x70\x09\x22\xc0\x4e\x2b\x40\x20\x19\
+\x53\x15\xaf\x80\x40\xa4\xf5\x04\x0f\xc1\x8c\xd0\x54\xf4\xa9\x06\
+\x7a\x31\x53\x9a\xb6\x6f\x65\xdf\xb2\xeb\x53\x6b\x4e\x6f\x19\x69\
+\xc5\xdb\x97\x4c\xb7\x21\x59\x60\x86\x0b\xf2\xf5\x01\xdd\x9b\xe0\
+\x6a\x8f\xef\xfc\x96\xda\xbe\x44\x58\x3f\x76\x5a\xc4\x34\x58\xa6\
+\x39\x7e\x5a\xd4\xa5\x42\xc9\xcc\x85\x41\xdb\x87\xa2\x1a\x0a\xe7\
+\xa7\x4f\x8b\xda\xe3\x2b\xe5\xc9\x9b\x0f\x4e\xbd\x4e\xf1\x7a\x79\
+\xee\x3d\x26\xd3\xfb\x4e\x0f\xd2\x11\xc1\x09\x08\x83\x0e\x47\xe2\
+\x8b\xa6\x28\x0c\x64\xa6\x4a\x0a\xcd\xd0\xd7\x5b\x62\xac\xc6\xb8\
+\x00\x59\x0c\x25\x90\x6d\x80\xd3\x93\x81\x66\x8a\x72\x3c\x38\xf0\
+\x51\x31\xdf\xd1\x8c\x31\x8b\x71\x81\x31\xa3\xb9\xc1\x31\x29\xbe\
+\x95\x08\x6e\x50\x05\x8c\x32\xa6\x19\xf6\x86\x08\x42\x2d\xce\x0f\
+\xbd\x61\x72\x03\xce\x91\x8b\x00\x2f\x05\x0c\xcc\x8e\x6f\x2b\x42\
+\x7a\x61\x4a\x78\x39\x01\x9c\xca\xe8\x23\x05\xb3\x78\xb8\xc2\xf1\
+\x8d\x14\x98\x09\xa2\x8a\x0d\xb8\x62\x78\x44\xc7\xa1\x8f\x30\x38\
+\x37\x48\xa4\x20\x36\x61\xf2\xee\xa1\x5d\x7a\x65\xf7\xb8\xd5\x67\
+\x9f\x12\x9b\x6f\xe5\xe8\x7f\xec\x94\x18\xb4\x3f\x8f\x72\x9f\xa1\
+\xed\x9d\x13\x83\x02\x0a\xad\xeb\xc4\x88\x4b\xc8\xab\x49\xa5\x96\
+\x07\x54\xb4\x6b\x41\xb8\x14\x65\x14\x96\x9c\xc8\x4a\x2d\xc1\xd2\
+\x8d\x45\x05\x04\xfd\x82\xbc\xbb\x52\x4b\x70\x00\x4a\x13\x54\x56\
+\x48\x08\x38\x95\xa8\x6c\x42\x29\x06\xfe\x01\x92\x2a\x85\xc6\xa5\
+\xbc\xb4\x0f\x23\x66\x02\xb4\x03\x5a\x9a\x04\x33\x02\x4f\xa3\xcb\
+\x17\x44\x0d\x67\x0a\x39\x31\xcf\x87\xbc\x00\x68\xd2\x30\xae\x24\
+\xd2\x28\x2c\x52\xd4\xbd\x0f\xa8\xa0\xfe\x44\xe0\x0b\xe9\xb8\x1e\
+\x42\x35\xd5\x1c\x25\x34\x9c\x28\xae\x71\xe5\xca\x72\xc5\x69\x25\
+\xb7\x94\x9a\xc0\x3c\x28\x8f\x31\x54\x0b\x5c\x25\xe4\x7a\xd6\xaa\
+\xd2\x78\xa4\x24\xca\x78\x69\xe5\xdc\x90\xc8\x00\x32\x88\x9a\x25\
+\x5c\x03\x15\xdd\x03\xa7\x8a\x6a\x7c\x29\x9b\x0b\xab\x88\xf4\xa2\
+\xfb\x2d\x9f\xf9\xc3\xcf\xd0\xc1\xed\x0e\x3d\x43\x3f\x9b\xdd\x5c\
+\xbc\x3a\xc3\x57\x6f\x2e\x5e\xfd\x1b\x91\xc7\x79\xe1\
 \x00\x00\x37\x3f\
 \x3c\
 \x3f\x78\x6d\x6c\x20\x76\x65\x72\x73\x69\x6f\x6e\x3d\x22\x31\x2e\
 \x30\x22\x20\x65\x6e\x63\x6f\x64\x69\x6e\x67\x3d\x22\x75\x74\x66\
 \x2d\x38\x22\x3f\x3e\x0d\x0a\x3c\x21\x2d\x2d\x20\x47\x65\x6e\x65\
 \x72\x61\x74\x6f\x72\x3a\x20\x41\x64\x6f\x62\x65\x20\x49\x6c\x6c\
 \x75\x73\x74\x72\x61\x74\x6f\x72\x20\x31\x32\x2e\x30\x2e\x31\x2c\
@@ -891,691 +1116,484 @@
 \x30\x2e\x35\x37\x38\x2c\x30\x2e\x39\x34\x35\x2c\x33\x30\x2e\x31\
 \x31\x33\x2c\x30\x2e\x30\x33\x35\x63\x37\x2e\x36\x30\x34\x2d\x30\
 \x2e\x37\x32\x36\x2c\x32\x31\x2e\x39\x31\x33\x2c\x30\x2e\x33\x37\
 \x33\x2c\x32\x37\x2e\x39\x34\x36\x2d\x35\x2e\x32\x34\x38\x43\x35\
 \x30\x2e\x39\x2c\x38\x31\x2e\x31\x35\x33\x2c\x30\x2c\x38\x36\x2e\
 \x32\x39\x32\x2c\x30\x2c\x37\x36\x2e\x34\x37\x22\x2f\x3e\x0d\x0a\
 \x3c\x2f\x67\x3e\x0d\x0a\x3c\x2f\x73\x76\x67\x3e\x0d\x0a\
-\x00\x00\x0d\xee\
-\x00\
-\x00\x40\xee\x78\x9c\xed\x5a\x59\x73\xdb\xc8\x11\x7e\xf7\xaf\x60\
-\xe8\x17\xbb\x96\x04\xe7\x3e\x68\x49\x5b\x8e\x5d\x9b\xda\x94\x92\
-\xad\x5a\xef\x56\x1e\x53\x10\x38\x92\xb0\x06\x09\x06\x00\x25\xd1\
-\xbf\x3e\xdd\x00\x88\x83\x1c\x4a\xa0\xac\xdd\xa4\x12\x93\x76\x89\
-\xe8\xe9\x39\xfa\x9b\x3e\x67\x70\xf6\xfd\xc3\x32\x19\xdd\xb9\x2c\
-\x8f\xd3\xd5\xf9\x98\x06\x64\x3c\x72\xab\x28\x5d\xc4\xab\x9b\xf3\
-\xf1\xaf\xbf\xfc\x30\x35\xe3\x51\x5e\x84\xab\x45\x98\xa4\x2b\x77\
-\x3e\x5e\xa5\xe3\xef\x2f\x5e\x9d\xfd\x69\x3a\x1d\x7d\xc8\x5c\x58\
-\xb8\xc5\xe8\x3e\x2e\x6e\x47\x3f\xae\x3e\xe7\x51\xb8\x76\xa3\x37\
-\xb7\x45\xb1\x9e\xcf\x66\xf7\xf7\xf7\x41\x5c\x13\x83\x34\xbb\x99\
-\xbd\x1d\x4d\xa7\xd0\x33\xbf\xbb\x79\x35\x1a\x8d\x60\xda\x55\x3e\
-\x5f\x44\xe7\xe3\x9a\x7f\xbd\xc9\x92\x92\x6f\x11\xcd\x5c\xe2\x96\
-\x6e\x55\xe4\x33\x1a\xd0\xd9\xb8\x65\x8f\x5a\xf6\x7b\x77\x15\x64\
-\x2e\x4f\x37\x59\x54\x0d\x1f\x45\x5d\xce\x6c\x71\xdd\xb2\xc2\x4a\
-\xee\x79\xc9\x44\xad\xb5\x33\xc2\x66\x8c\x4d\x81\x63\x9a\x6f\x57\
-\x45\xf8\x30\x5d\xe5\xaf\x3b\x5d\x61\x81\xbe\xae\x8c\x10\x32\x83\
-\xb6\x96\x73\x18\xd7\xfc\x21\x01\x18\x8e\x2e\xa6\x6c\xed\xce\x0e\
-\xd0\xaf\xe1\x7f\xd3\xa1\xc1\xb0\x92\xf5\x1a\x7a\xba\x60\xe5\x8a\
-\xd9\xc7\x5f\x3e\xce\x76\xdc\x53\x12\x2c\x8a\x45\x67\x98\x5d\xaf\
-\xde\xbc\xbd\xed\x58\x85\x4b\x97\xaf\xc3\xc8\xe5\xcd\x14\x65\xff\
-\xdd\xc3\xdc\x3d\xac\xd3\xac\x98\x6e\x17\x6b\x58\x8c\x25\x01\x29\
-\x3f\x5e\x9e\x87\x01\x3c\xd7\x71\xe2\x70\xce\xf3\xf1\xec\x36\x5d\
-\xba\xd9\x6f\xf1\x72\x19\x46\xb3\x8f\x2e\xff\x5c\xa4\xeb\xd9\x7d\
-\x0c\x1c\xc1\x7a\x55\x21\x77\x1f\x2f\x8a\xdb\xf3\xb1\x30\xeb\x87\
-\xf2\xf9\xd6\xc5\x37\xb7\x45\x87\x10\x2f\xce\xc7\x00\x33\xa5\xbc\
-\x9e\x6e\x87\xc4\xbc\xd1\x65\x12\x70\xd6\x5f\x49\xa7\x49\xf0\xef\
-\x16\xee\xce\x25\xfd\xbe\x8b\x34\xba\x0a\xf3\x66\x89\x45\x7c\xe3\
-\xb2\x62\x16\xdd\xe5\xb3\xeb\xcc\xb9\x45\xb5\xd4\x12\x3d\xb0\x88\
-\x9b\x74\x1a\x47\xe9\x6a\x5a\xdc\x82\xb2\xce\x60\x86\x24\xbc\x4a\
-\xdc\x2c\x8c\x0a\x98\x23\x3f\x18\xb8\x92\x3d\xdf\xe6\x85\x5b\x4e\
-\x93\xf4\x66\x9a\x6e\x8a\x60\xa7\x29\xcd\x12\x81\xb8\xde\x14\xff\
-\x74\x0f\x85\x5b\x55\x6b\x85\xd9\x3a\x1b\x57\x36\x63\xb7\x86\x36\
-\xbe\x80\x01\xce\x16\xee\x3a\xc7\x81\x2a\x64\xf0\x89\x97\x0d\xd0\
-\x04\x0a\xe6\xc2\xec\x2f\x59\xb8\x88\xc1\xa6\x2a\xa6\x8a\xad\xdf\
-\x62\x8d\x55\x75\x1f\xe8\x95\x83\xa4\x3b\xde\x1a\x6e\xa0\x00\x8f\
-\x19\xb7\xe4\xf4\xfa\x3a\x77\xb0\x2d\xa4\x43\xcb\x8b\x6d\xe2\x2a\
-\xee\x69\x94\x26\x69\x36\x7f\x1d\x39\xfc\xbe\x2b\x49\x29\xa8\x5c\
-\x5c\x6c\xe7\xf4\xdd\x78\x34\x7b\x6a\x36\x4b\x88\x67\x36\x5a\xab\
-\xd9\x13\xb3\x5a\x87\xdf\xbd\x59\x77\x5d\xdb\xd9\xcf\x66\x7d\x18\
-\x4e\x46\xcd\xb4\x88\x34\xdb\x08\x4b\x48\x5c\x04\x6b\x0d\x93\xfb\
-\x70\x9b\x0f\x80\xd5\x27\xe8\x13\x02\x5e\x97\x9f\x67\xc0\x6a\x2c\
-\xf3\xc1\x7a\xfa\x6c\x2f\x0a\x23\x79\x01\x18\x8d\x4f\xb0\x27\x60\
-\x94\x0c\xbf\xcf\x81\xd1\x88\xd3\x61\xf4\xcd\xf6\x92\x30\x2a\x73\
-\x0c\x25\xcf\x62\x84\xc3\xef\x51\x13\xf1\x40\xe9\x31\xbd\x16\x0f\
-\x4d\x8e\xa3\xe6\x99\x5d\x51\xfc\xee\x41\xf1\xd8\xec\x3e\xc3\xef\
-\xcc\xce\x5e\x0e\x45\x29\x9e\xd6\x35\xa9\x06\x02\x74\x3a\xf0\x03\
-\x74\x4f\xfa\xfc\xf0\x40\xcf\x18\x5e\xe1\xf7\xf7\xf7\x8c\x82\xbd\
-\x80\x49\x0b\x9f\x91\x3d\x21\xa0\x66\xda\x91\xf0\x39\x26\x2d\x7c\
-\x9b\xfa\x84\x49\xfb\x66\x7b\x49\x18\x39\x79\x1a\x25\xee\x75\x7c\
-\xc3\xd4\x41\x12\xfc\x7e\x8d\x32\x72\xaf\x23\x1c\x36\x3b\x35\xf8\
-\x7d\x61\x65\x3c\xa6\x6d\xc7\x61\x36\x4a\xb1\x13\x3c\x67\xbd\xbc\
-\x7d\x0d\x7b\x5c\x53\x77\x80\xc1\x5c\xe2\x24\x4f\xe9\x9b\xcd\xef\
-\x21\xfd\xb3\xa9\x3f\x10\x46\x79\x54\x5b\x87\xa7\x30\x43\x61\x94\
-\xec\x24\x18\x8f\xa4\x30\x43\x61\x94\xe2\x29\x18\xf1\x29\x4c\x4e\
-\x86\xb1\xac\x01\xe7\xb7\x99\x83\x9a\xf5\xb5\x07\xcf\x2e\xdc\xfd\
-\x29\xa0\xb9\x75\x58\xd1\x03\xac\xdc\x06\x9a\x50\x2a\x5a\x09\xa2\
-\xed\xf9\x98\x05\x90\xdb\x5b\x6e\x5a\xea\xb5\x97\xf7\xda\xcb\x9b\
-\x01\xab\x0e\xa8\x06\x4e\xd9\x10\x6f\xea\x15\xfc\x92\x85\xab\x1c\
-\x8a\xd2\xe5\xf9\x78\x19\x16\x59\xfc\xf0\x86\x06\x4c\x72\x21\xd8\
-\x64\xca\x02\x66\x15\xb5\xd2\x4d\xa9\x9a\xd0\x40\x0b\x2d\x14\x29\
-\x1f\x48\x60\x25\x87\xec\x7e\x32\xa5\x32\x10\xda\x12\x33\xa1\xd0\
-\x4f\x2b\xc5\xdf\x1e\x4c\xf1\xeb\x2a\x2e\xa0\xd8\xde\xe4\x2e\xfb\
-\x84\x05\xeb\x4f\xab\x5f\x73\xd7\x6e\x85\x1f\x74\x5c\xb4\x0c\x94\
-\x10\x9a\xeb\x9e\x7c\x5c\x05\x82\x51\xca\x74\x0f\x0b\x26\x02\xc3\
-\x35\x65\xaa\x87\xdb\x21\x6f\xe4\xe5\x7d\x0c\x8c\xca\x76\x27\xc4\
-\xf3\x43\x72\xa5\x19\x07\x64\x94\xe6\x52\x23\x4c\x72\x42\x55\x60\
-\x34\x27\x6a\x28\x0c\xc7\x75\xc3\x9a\xce\x0a\x1f\x55\x31\x35\x20\
-\x4e\x3f\x01\xf7\xb0\x45\x1e\xc7\x89\x01\x2a\xca\x12\x3d\x11\x81\
-\x90\x8a\x31\x53\xaa\xc9\x54\x06\x46\x4a\x4b\x69\xf9\xc4\x02\xc5\
-\x35\x53\x06\x94\x46\xf0\x40\x6a\x64\x50\x34\xb0\x40\xa5\x6f\x7b\
-\xda\xaa\xa0\xf4\xa7\x92\x8a\xde\xc6\x0b\x00\x5c\x40\xa4\x63\xbd\
-\x8d\xb7\x3c\xd0\x86\x90\x8e\x92\x44\x5e\xde\xc8\xcb\xeb\x43\x9d\
-\x0f\x42\xbd\x0c\xeb\xc3\x51\xf7\x3b\xe8\x67\xea\x9d\xe2\x12\xc0\
-\x69\x29\x60\x28\x56\x18\x2b\x4e\xd5\xb9\x2d\x03\x63\x30\x01\x18\
-\x08\x58\x79\x2b\x34\x50\x39\x18\x38\x97\x96\xb5\x4e\x64\x4b\x01\
-\x55\xc0\x4f\x82\xaa\x77\x78\xa9\x8f\xd7\x9b\x4b\x9a\x61\xa8\x0e\
-\xc9\x39\x07\xa2\x3a\x40\x78\x0d\x02\x59\x50\xdc\x9e\xf0\xd4\x04\
-\x84\x53\xb6\x27\x3c\x78\x5b\x43\x04\xa5\xba\x27\xbc\x00\x73\x17\
-\xd2\x30\xf9\xa8\xf0\x4a\x0c\x13\x5e\x8a\xff\x02\x43\x96\x9c\x08\
-\x2d\x27\x32\x20\x20\x99\x54\x60\xba\x06\x43\x01\x37\xcc\x6a\x34\
-\x6b\x01\x0e\x4f\x10\xce\x14\x44\x08\x70\xb0\xda\x4a\x0a\xbf\x6c\
-\x20\x0c\xe7\x84\xf7\x0c\x19\x02\x14\x63\x9a\x76\xaa\x7a\x34\x64\
-\x88\x45\xdc\x2a\xa2\x49\xcf\x90\x61\x2f\x8c\xe1\xf0\xaf\x67\xc8\
-\x87\xbc\x91\x97\xd7\x67\xc8\x7a\xa0\x21\xab\x01\x07\x40\xa7\x1b\
-\x72\x81\x3f\x93\xb0\x70\x6f\xa6\x14\x4c\x4c\x51\xd6\xda\xf0\xb3\
-\x0c\x55\x04\x5a\x81\xaa\x89\xbe\xa1\x0a\x18\x52\x0b\xaa\xf6\x75\
-\x95\x12\xad\xd9\x9e\xa1\x52\xf0\xc6\x0c\xb6\xeb\x51\x5d\x35\x03\
-\x51\x1b\x72\xde\xf3\x62\x86\x0a\x9e\x47\x08\x6b\x85\xee\x1b\x2a\
-\xe8\x97\x94\xb2\xe3\x5a\x4a\xe1\x79\x00\x69\x08\x80\xd2\x13\xde\
-\x00\x7a\x10\xa2\xc4\xe3\xc2\xdb\x81\x86\x3a\xe4\xcc\xf0\xc5\x84\
-\x47\x7f\xa4\xc0\xe2\xf6\x5c\x34\x38\x63\x4a\x94\xec\x7b\x29\x46\
-\x03\x49\x29\x35\x72\x7f\xe7\x89\x36\x56\x3e\xea\xa5\x2c\x61\xc3\
-\x84\xb7\x6a\xa8\xf0\x67\x33\x3c\xc9\x2e\x7f\x35\x47\xe9\x78\x8e\
-\xbe\xb8\x8b\xdd\x7d\x35\x46\x5e\x64\xe9\x67\xc8\xf3\x5f\x87\xa2\
-\x53\x6b\x5e\xc7\x49\x02\xb4\xaa\x32\xaf\x69\xb8\x64\x3c\xdd\xaf\
-\x1f\xd7\xe1\x8d\x2b\xeb\x02\xe0\xab\x0a\x83\xba\xe1\x2a\xcd\x16\
-\x2e\xdb\x35\xa9\xf2\xd3\x6b\xaa\x4b\x07\xac\xaf\x99\x14\x96\xd0\
-\x46\xa0\x46\x1c\x1c\xbc\xc3\x46\x7c\xed\xf9\x6d\xb8\x48\xef\x01\
-\xf2\xfd\xc6\x2f\x69\x0a\xf6\x0f\xc9\xab\x54\xe0\xd1\x0f\x9a\xd1\
-\x81\x71\x1d\x60\x08\x27\x07\x03\x97\xd9\x3e\xd8\xb4\x30\xd4\xd3\
-\x73\x93\x65\xb0\x03\xd3\x24\xdc\x3a\x90\xad\xfc\xb3\xdb\xfe\xfc\
-\x36\xbd\xbf\xc9\x10\xa3\xeb\x30\x69\x40\x6a\xba\x62\xd3\xf4\xea\
-\x2a\x7d\x40\xc7\xb4\x39\x68\x5e\xa4\xd1\x06\x6f\xec\xa6\x9b\x4a\
-\x1b\xeb\x5b\x9a\x0e\x07\x8e\xdf\x95\xda\x3b\xcb\x7d\xbc\x82\xc6\
-\x69\x7d\xfb\xa3\xe9\x01\xae\x35\xc3\xee\x3a\x48\x37\x01\x6f\x9f\
-\x03\x9d\xbc\xa2\x47\x1a\xb7\x68\xfa\x74\xa7\x63\x4b\x57\x84\x8b\
-\xb0\x08\x5b\x2d\xd9\x51\x76\x87\x80\x67\xd9\xe2\x7a\xfe\xf3\xc7\
-\x1f\x9a\x4a\x33\x8a\xe6\xff\x48\xb3\xcf\x6d\x91\x88\x0c\xe1\x55\
-\xba\x81\x35\x35\xd5\x2f\xde\xca\x44\x73\x74\xe6\x61\x71\x11\x2f\
-\x41\x76\xbc\x18\xfc\xee\x61\x99\x80\x5a\x37\x0d\x3d\xe6\x62\xbb\
-\x76\xed\xa0\xd5\xb0\xbb\x4b\x4e\xef\x45\xe9\x22\x5a\xc6\xd8\x69\
-\xf6\xa9\x00\x8d\xff\x11\x27\xe9\x54\xc4\xd5\xa0\x11\x5e\xd3\xa6\
-\xd9\x45\x67\x60\x14\xe0\xfd\x4d\x53\xb7\xf6\x96\x10\x17\x89\xbb\
-\xf8\x6b\xf8\x79\x73\x35\xfa\x54\x38\x30\xdd\xac\x5c\x6e\x45\xef\
-\x8e\x31\x3b\x1c\xa4\xe4\x3c\x98\x0f\x87\xad\x64\xb8\xa8\x45\xa8\
-\xee\xfe\x82\xe5\x26\x8f\xa3\xdb\x30\x49\x82\xe8\x4b\xd9\xb5\xe6\
-\x6a\x7b\xc2\x14\x49\x1c\xb9\x55\xfe\x34\x2c\xe5\xb4\xf1\x1d\xd8\
-\xf4\x72\x99\xae\xf2\x12\xa1\xba\x6f\x3e\xbb\xda\x4e\xf3\x70\x06\
-\x45\xc6\xec\x00\x9e\x4a\xb0\x4f\xe5\xbd\xdc\xe8\x32\xbd\x19\xfd\
-\xb4\x29\x7c\x12\x97\x52\x6c\xae\x7e\x03\x2f\xd5\x83\x01\x17\xf3\
-\xe7\xf0\x66\x0f\x49\xa4\x26\xf1\x45\x02\xe3\xa5\x38\x5e\xfd\x7c\
-\x8c\xe9\x49\x1e\xf7\x10\x7b\x39\x2a\x5a\x6f\xfe\x0a\xc9\xfe\x4a\
-\xcb\xcd\x42\x95\xed\xaa\xf0\xe5\x3e\xb2\x1d\x2d\x3e\x11\xd4\xfe\
-\x96\xad\x5d\x06\x6a\x99\x3f\xb9\x65\xbe\x3b\xfc\x9f\xdd\x3a\x4b\
-\x17\x9b\xf2\x12\xb5\xbf\x57\x5f\x39\xf0\xc7\x18\x42\x45\x7c\xb5\
-\xf1\x0e\x9c\xb9\x7f\x6d\x62\xe8\xf1\xac\x91\xff\x9e\x16\x00\xc9\
-\xcb\x8e\xf9\xbe\x38\xbe\xd8\xaf\x42\xc1\x65\xf1\x5d\xb9\xa5\xa8\
-\x0d\xf9\xcb\x2e\xfa\xd3\x6d\x98\xb9\xf7\x49\xfc\xb9\x0b\x46\xa9\
-\x7a\xb5\xaa\xed\x0e\xcf\x3a\xfe\xf4\x6c\xb6\xf3\xb6\xe5\xd3\x4d\
-\xeb\x85\x7b\xe1\xa9\x71\xe1\x49\x78\xe5\x20\xb4\x5f\x62\xe3\xe8\
-\xa0\xf5\x26\x4b\x37\xeb\x65\xba\x70\x75\xf7\xc6\x81\x83\x2d\x34\
-\x75\x45\x19\x92\x35\x81\xec\x47\x74\x92\xbc\xec\xc1\x4b\x2e\x4f\
-\xc4\x20\x10\xf3\x5e\x6e\x57\x65\x89\x90\x27\x91\x36\x25\x6a\xde\
-\x51\xa0\x78\x82\x46\x3a\xd5\x43\x1d\xcf\x30\x7f\xa6\xb6\xdb\xa5\
-\xac\x3a\x60\x69\xd6\xb0\x36\x21\xac\x0f\x2e\x0f\xcf\xc2\xfb\x87\
-\xc1\x98\xe2\xcc\x21\x14\xbc\x79\x7d\x78\x00\xf1\xb6\x6c\xf5\x1c\
-\xa7\x97\xe4\x6c\x93\xb8\xb9\xbb\x73\xab\x74\xb1\x78\x57\xe5\x4f\
-\x9d\x23\x66\x7c\xac\x22\x70\xa7\x5f\x4d\xc6\x4c\x0e\x70\x9e\x83\
-\x62\x16\x5d\xda\x6f\x69\xbc\x9a\x83\x4e\xba\xec\xdd\x32\xcc\x3e\
-\xbb\x6c\xbe\x4a\x57\xae\xfe\x3d\xcd\x8b\x30\x2b\x7a\x94\x65\xbc\
-\xe8\x3d\xbb\x55\xfd\x5c\x8f\x59\x0e\x95\xc4\xf0\x67\x4e\x77\x35\
-\xcf\xae\x6d\x11\x42\x0a\x91\x65\xe1\xb6\xd7\x03\xa9\xd5\xe9\x6d\
-\xe7\x0a\xb1\x6e\x3b\x84\xe1\x2e\xce\xe3\xab\x38\x41\x62\xf9\x33\
-\x71\xef\x16\x71\xbe\x06\x95\x99\xc7\x2b\x14\xe8\x5d\x7a\xe7\xb2\
-\xeb\x24\xbd\xdf\xb5\x77\xca\xe6\x8e\x2a\x6d\xcb\x4d\xd5\x5c\xc9\
-\xce\xb1\x03\x2a\x87\x08\x84\x05\xa5\x31\x07\xca\x41\xc1\x5d\x32\
-\x62\x3a\x07\xa9\x3b\xe5\x80\x64\x92\x99\x6e\x43\xab\x1c\x82\x3c\
-\x5f\x39\x0e\xcf\x51\x4e\x57\x8e\x2e\xd0\xdf\x34\xe3\xa8\x66\xac\
-\xc3\xe2\xb6\xd9\xa7\xa6\x5c\x01\x67\x84\x19\x1a\x24\xc5\x11\x7e\
-\x7a\xdb\x8b\x3d\xac\xe9\x9c\x32\x02\xed\x6f\x23\xd0\x1e\x4e\x8d\
-\xa5\x6c\xd2\x1c\x98\x8d\x2e\x91\x4a\x8d\xe2\xcc\x4e\x78\x40\xa4\
-\xc0\xb7\x08\x80\x0a\x55\x9c\x15\x94\x32\x89\x54\x6b\x34\xb5\xa2\
-\xa6\x1a\xc9\x29\xf0\x02\x99\x1a\xaa\x65\x35\xc2\xc1\xb8\x5f\x46\
-\x07\xaa\xb5\x27\xdf\xbe\xfc\x1e\x84\x8e\xa2\x39\x60\x0b\xfc\x9b\
-\xe6\xdd\xe6\x7d\x95\x38\xa2\x32\x07\x4a\xd5\x1b\x79\x4f\x29\x1f\
-\x51\x5f\xbf\xa6\x57\x83\x1d\x9a\xca\xbe\x4d\x3d\x62\x82\x4a\xbc\
-\xdd\x33\xd7\x03\xe4\xfc\xee\xa6\xd2\x0e\x19\x48\xc6\x8d\x22\xb0\
-\xe3\x96\x59\x08\x58\x72\xf4\x01\xa9\x94\x33\xca\x44\x87\x0a\xfb\
-\x6d\xa8\xd2\x52\x4e\x44\xc0\x84\x84\x88\x24\x7a\x34\xc5\x95\xa1\
-\x4c\x55\x9a\xb1\xa3\xb2\x00\xcf\xcb\x14\xc5\x31\xbb\x54\x6d\xb4\
-\xb6\xba\x33\x0f\xe8\x10\x25\x9c\x2a\xd5\x59\x51\x4b\xbb\x1c\xc1\
-\x6f\x65\x15\x97\xaa\x43\xfd\x30\x12\x50\x9b\x1a\x43\x2c\xef\x50\
-\x81\x26\x08\x17\x8a\x76\xe6\xe9\xd1\xea\x15\x5d\x76\xa9\xcd\xea\
-\x3f\xf4\xa8\x3b\x39\xdb\x79\x5a\x3c\xda\x15\xb5\xb4\x4b\x2f\x9e\
-\xdf\xac\x62\xa0\x55\xb0\x26\x7f\xa8\xef\x56\x9f\x36\x8c\x6e\x84\
-\x2a\x97\xe0\x37\x05\x12\x70\xd8\xe0\x5e\xec\x6b\x03\x22\x37\xfb\
-\xe1\x93\xd9\x00\x7c\x1f\xeb\x9c\x14\xef\x22\x2e\xb7\x81\x95\x94\
-\xf3\xfd\x00\xad\x8c\xa0\x9a\x77\xf3\x3c\x0e\x41\x5b\x49\xbc\x51\
-\x7d\xdc\xa5\xa3\x3b\x3f\x1f\x87\x59\x74\x2c\x2a\x43\x28\xb7\x56\
-\x28\xc9\xe8\xe0\x9c\x8d\x3d\x23\x67\xfb\x16\x96\x1f\x0b\xcb\xfb\
-\x71\xd6\x28\xd5\x49\xa3\x76\x7b\xe9\xbf\xcf\x6d\x9b\xbd\x97\xc0\
-\x4d\x33\xd6\x0c\x87\xb7\xcc\x6d\xf3\x16\xcf\x8d\xc1\x7b\x19\xcb\
-\x65\x3f\xc6\x0b\x12\x08\x83\xf1\x7c\xd4\x0c\x3f\x7a\x3f\x6a\xc6\
-\x1a\x35\xdd\x46\x64\x44\xe1\x3b\xb2\x01\xa8\x37\x37\x06\x02\xfd\
-\xb0\x0e\xbe\x19\xbe\x34\x8b\x28\x0e\x2e\x6e\xa0\xf6\xd1\x46\x58\
-\xff\x8d\x61\xdd\x34\xd5\x81\xd4\xd6\xe0\x35\x75\x20\xe1\x2f\xb7\
-\x6f\x8f\xd8\xca\x09\x69\xea\xeb\x28\x6a\xf5\xfc\x94\x92\xa5\x3a\
-\xf1\xed\x5b\x00\x09\x6c\xf9\x31\x6c\xdf\x04\xa0\x32\x5c\x2d\x0e\
-\x6c\xa0\xa2\xfe\xaf\xdb\x40\x95\x38\x40\xa1\x42\x71\xf7\x26\x14\
-\xb6\x11\xdf\xf0\x28\xd3\xca\x86\x0a\x15\x08\x97\x92\x2b\x4c\x20\
-\x6d\xa0\x94\x80\xf0\x2c\x8e\x51\x55\x40\xb5\xa2\x42\x03\x95\x41\
-\x59\x0b\x41\x5b\xc8\x09\x83\x08\x0a\x79\x29\xe1\x25\xaf\xb4\x94\
-\x0b\x48\x14\x28\xc5\x93\x6c\x4a\x68\x9f\x8a\x6b\xd0\x44\xe9\xde\
-\x1a\xda\x95\x75\x42\x70\x6b\xc1\x82\x1f\x1a\xd9\x7e\x82\x8d\x39\
-\xf6\x10\x9d\x24\x81\x24\x86\x30\x2a\x86\x3a\x69\x7c\xd7\xe6\x77\
-\x75\xd2\xff\xf7\x1a\x0a\x91\x9a\x81\x4d\x1b\xd0\x0e\x16\x08\x6d\
-\x88\xa8\x34\xa9\xa1\xea\x00\x37\xa1\x4c\x05\xa1\x8e\xd6\x90\xf2\
-\x49\x7a\x84\x0a\x4e\x1d\x0a\x20\x21\x08\x26\xb2\x90\x42\x72\xa8\
-\x97\x80\x8a\x27\x3c\x1c\x9d\x22\x68\xa5\x95\xc2\x5a\x36\xc1\x4b\
-\x7c\xcd\xa1\x76\x42\x4d\x66\x56\x30\x43\x4a\x4d\x16\xa8\xeb\xfd\
-\xf9\x9b\x55\xf9\xb5\x53\x0e\xd0\xce\x13\xcb\x45\x5f\xc5\x08\xd2\
-\x9a\x3e\x70\x0c\x93\x1f\x90\xd0\x4e\x28\xc6\x01\x70\x7f\xb2\x04\
-\x63\x47\x85\xec\x08\x4c\x98\xb0\xd2\xe0\x41\xf1\x4b\x64\x8e\x50\
-\xf1\x5e\xd0\x72\xab\x91\x0a\x70\x09\x22\xc0\x4e\x2b\x40\x20\x19\
-\x53\x15\xaf\x80\x40\xa4\xf5\x04\x0f\xc1\x8c\xd0\x54\xf4\xa9\x06\
-\x7a\x31\x53\x9a\xb6\x6f\x65\xdf\xb2\xeb\x53\x6b\x4e\x6f\x19\x69\
-\xc5\xdb\x97\x4c\xb7\x21\x59\x60\x86\x0b\xf2\xf5\x01\xdd\x9b\xe0\
-\x6a\x8f\xef\xfc\x96\xda\xbe\x44\x58\x3f\x76\x5a\xc4\x34\x58\xa6\
-\x39\x7e\x5a\xd4\xa5\x42\xc9\xcc\x85\x41\xdb\x87\xa2\x1a\x0a\xe7\
-\xa7\x4f\x8b\xda\xe3\x2b\xe5\xc9\x9b\x0f\x4e\xbd\x4e\xf1\x7a\x79\
-\xee\x3d\x26\xd3\xfb\x4e\x0f\xd2\x11\xc1\x09\x08\x83\x0e\x47\xe2\
-\x8b\xa6\x28\x0c\x64\xa6\x4a\x0a\xcd\xd0\xd7\x5b\x62\xac\xc6\xb8\
-\x00\x59\x0c\x25\x90\x6d\x80\xd3\x93\x81\x66\x8a\x72\x3c\x38\xf0\
-\x51\x31\xdf\xd1\x8c\x31\x8b\x71\x81\x31\xa3\xb9\xc1\x31\x29\xbe\
-\x95\x08\x6e\x50\x05\x8c\x32\xa6\x19\xf6\x86\x08\x42\x2d\xce\x0f\
-\xbd\x61\x72\x03\xce\x91\x8b\x00\x2f\x05\x0c\xcc\x8e\x6f\x2b\x42\
-\x7a\x61\x4a\x78\x39\x01\x9c\xca\xe8\x23\x05\xb3\x78\xb8\xc2\xf1\
-\x8d\x14\x98\x09\xa2\x8a\x0d\xb8\x62\x78\x44\xc7\xa1\x8f\x30\x38\
-\x37\x48\xa4\x20\x36\x61\xf2\xee\xa1\x5d\x7a\x65\xf7\xb8\xd5\x67\
-\x9f\x12\x9b\x6f\xe5\xe8\x7f\xec\x94\x18\xb4\x3f\x8f\x72\x9f\xa1\
-\xed\x9d\x13\x83\x02\x0a\xad\xeb\xc4\x88\x4b\xc8\xab\x49\xa5\x96\
-\x07\x54\xb4\x6b\x41\xb8\x14\x65\x14\x96\x9c\xc8\x4a\x2d\xc1\xd2\
-\x8d\x45\x05\x04\xfd\x82\xbc\xbb\x52\x4b\x70\x00\x4a\x13\x54\x56\
-\x48\x08\x38\x95\xa8\x6c\x42\x29\x06\xfe\x01\x92\x2a\x85\xc6\xa5\
-\xbc\xb4\x0f\x23\x66\x02\xb4\x03\x5a\x9a\x04\x33\x02\x4f\xa3\xcb\
-\x17\x44\x0d\x67\x0a\x39\x31\xcf\x87\xbc\x00\x68\xd2\x30\xae\x24\
-\xd2\x28\x2c\x52\xd4\xbd\x0f\xa8\xa0\xfe\x44\xe0\x0b\xe9\xb8\x1e\
-\x42\x35\xd5\x1c\x25\x34\x9c\x28\xae\x71\xe5\xca\x72\xc5\x69\x25\
-\xb7\x94\x9a\xc0\x3c\x28\x8f\x31\x54\x0b\x5c\x25\xe4\x7a\xd6\xaa\
-\xd2\x78\xa4\x24\xca\x78\x69\xe5\xdc\x90\xc8\x00\x32\x88\x9a\x25\
-\x5c\x03\x15\xdd\x03\xa7\x8a\x6a\x7c\x29\x9b\x0b\xab\x88\xf4\xa2\
-\xfb\x2d\x9f\xf9\xc3\xcf\xd0\xc1\xed\x0e\x3d\x43\x3f\x9b\xdd\x5c\
-\xbc\x3a\xc3\x57\x6f\x2e\x5e\xfd\x1b\x91\xc7\x79\xe1\
 \x00\x00\x00\x10\
 \x3c\
 \xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\
 \x00\x00\x00\x7a\
 \x3c\
 \xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\xa7\
 \x00\x00\x00\x05\x65\x6e\x5f\x47\x42\x42\x00\x00\x00\x08\x0c\xdd\
 \xc2\x03\x00\x00\x00\x00\x69\x00\x00\x00\x47\x03\x00\x00\x00\x16\
 \x00\x50\x00\x72\x00\x65\x00\x66\x00\x65\x00\x72\x00\x65\x00\x6e\
 \x00\x63\x00\x65\x00\x73\x08\x00\x00\x00\x00\x06\x00\x00\x00\x0b\
 \x50\x72\x65\x66\x65\x72\x65\x6e\x63\x65\x73\x07\x00\x00\x00\x11\
 \x61\x70\x70\x6c\x69\x63\x61\x74\x69\x6f\x6e\x57\x69\x6e\x64\x6f\
 \x77\x01\x88\x00\x00\x00\x02\x01\x01\
-\x00\x00\x00\x10\
-\x3c\
-\xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\
-\x00\x00\x1b\x20\
+\x00\x00\x1c\x67\
 \x00\
-\x00\x64\x65\x78\x9c\xb5\x3c\x09\x74\x1c\xd5\x91\x5f\xc7\x8c\x46\
-\xa3\xd1\x61\x59\x16\xc2\xf8\x68\x1b\x4b\x96\x64\x5b\x48\xc2\x5c\
-\x02\x03\xd2\x48\xb2\x64\xeb\x42\x23\x5f\x2c\x60\x5a\x33\xad\x51\
-\x43\x4f\xf7\xd0\xdd\x23\x59\x4e\x48\xc8\x69\xc8\x7a\x81\x40\x4c\
-\x6e\x70\x36\xc1\x4e\x58\x48\x20\x09\x2c\x21\x09\xb0\x81\x25\x24\
-\x84\x2b\x17\x39\x48\xc8\xc2\x92\x67\x08\x2f\x24\xe4\xda\x24\x40\
-\xb6\xfe\xff\x3d\xd3\xbf\x67\xba\xff\xcc\xc8\x8e\xf5\xec\x92\x67\
-\xba\xea\xd7\xaf\x5f\x55\xbf\xaa\x7e\xfd\x3e\xef\xfe\x58\xd3\x77\
-\x5f\xff\xd4\xa1\x27\xd7\xac\x78\xe8\xf2\xcf\x7c\xf3\x17\x47\x11\
-\x42\x3e\xd9\xdc\x3b\x3c\xd5\x87\x50\xe5\x2c\x42\xdb\x1e\x45\xa8\
-\x66\x03\x42\x63\x2a\x42\x25\x5f\xa1\xb0\xee\x1f\x14\x5e\x70\x2b\
-\xc0\xf7\xc3\xe7\xcf\x52\xb8\xa4\x83\xc2\x0b\xeb\x11\xda\xfd\x55\
-\x84\x4e\xb9\x92\xc2\xd3\x5e\x40\xa5\x77\x01\x1d\xdf\x9d\xa8\xec\
-\xb2\xab\x11\xf2\x7f\x08\x95\xdf\x7c\x2f\x42\x81\x27\x29\xdc\x34\
-\x81\xca\x6f\xf9\x3c\xfc\xff\x2d\x0a\x37\xbd\x97\xc2\x6e\x81\xc2\
-\xb3\x3f\x8e\xca\xef\xbf\x18\xa1\x9e\x0e\x54\xfe\x74\x39\xf0\x73\
-\x0c\x95\x3f\xf7\x36\xfc\xff\xef\xa8\xfc\xd8\x1f\x61\xcc\xf5\xc8\
-\xb7\xe1\x87\x30\xfe\x6b\x14\xb6\x2f\xa3\x70\xc3\x3c\x85\x1d\x9f\
-\xa4\x70\xf3\x46\x0a\x2f\xfc\x09\xf2\x0d\x8e\x23\xb4\x54\xa6\x70\
-\xc7\x5e\xe4\xdb\x39\x80\x50\xe9\x3e\x0a\x97\xfd\x99\xc2\xc1\x77\
-\x21\x5f\x72\x3b\x42\xcb\xd7\x51\x78\xda\x34\x85\x43\x1b\x90\x4f\
-\xbf\x0e\x3e\xdf\x89\x7c\x87\xe1\xb9\xe1\xa7\x51\x05\x7e\x7e\xcd\
-\xe3\xa8\xfe\xb6\x3b\x40\x82\x4f\x50\xb8\x25\x84\xda\xbf\x0e\xfc\
-\x96\xbf\x85\xda\x9f\x69\x86\xf9\xf7\xa0\xf6\xd7\x3a\x01\xfe\x1a\
-\x6d\x30\x62\x20\x87\x95\x68\x78\x58\x47\x68\xdd\x14\xda\xfe\x81\
-\x87\x81\xcf\x10\x85\xdd\x77\xa3\xf1\x93\xff\x84\x50\xd3\x7d\x68\
-\x72\xdf\x37\x60\x5e\x5f\x42\x3b\xb6\xc9\x08\x0d\xbc\x89\x76\x5c\
-\x7e\x08\xf8\x7b\x88\xc2\x8e\xe7\xd0\x0e\xf5\x36\xe0\xf3\x7e\xb4\
-\xfb\x2d\x90\xc3\x8a\x87\x29\x6c\xbf\x88\xc2\x8d\x65\x14\x76\x36\
-\x50\x78\xc6\x11\x0a\x87\x5e\x45\x7b\x3e\x06\xfc\xac\x54\xd1\x25\
-\xb0\x16\xa8\xf4\x29\x0a\xb7\xff\x27\xba\x64\xe8\x6f\xb0\xae\x4f\
-\xa3\x4b\x0e\x4f\xc1\xe7\xb7\x51\xb8\xea\x00\x85\x67\x8e\x51\xb8\
-\xad\x04\x5d\xfa\xbb\xdb\x11\x12\x0e\x52\xd8\xf5\x59\x0a\xb7\xff\
-\x16\x5d\xf6\x43\xe0\xeb\xa4\x2b\xd0\xf4\x6b\x5f\x40\xe8\xf4\x23\
-\xe8\x86\xf0\xc9\xc0\xf7\xbf\xa2\x3f\x8b\x77\x83\xfc\xea\x4a\xda\
-\x52\xdf\x41\xe8\xac\x87\x4b\x36\x5e\x98\x84\xf5\x59\x5d\x72\xda\
-\xd9\x6d\xb0\x1e\xe1\x92\x3d\x8f\xdc\x88\x50\xf3\xf3\x25\x57\xac\
-\xdb\x83\x50\xfd\x53\x25\xfa\x0d\xab\x40\x1f\xd6\x94\xdc\xf0\x9d\
-\x2d\x00\xe7\x4a\x3e\x3c\xf7\x08\x42\xa7\x0e\x95\x7c\xf4\x13\xf0\
-\xdc\x86\x7b\x4a\xee\x58\x7d\x16\x42\x65\x5d\x14\x2e\xb9\x94\xc2\
-\x5d\x3f\xa3\x70\xcf\x3d\x25\x0f\xdc\xbb\x0d\xa1\xd1\x48\xc9\xf7\
-\x57\xbf\x88\xd0\xc8\x7c\x69\xff\xab\x97\x20\x34\xf9\x72\xe9\xc2\
-\x69\x95\x80\xb7\x50\xba\xbf\x16\xc6\xe9\xf9\x42\xe9\x0d\xf7\x83\
-\x5c\xcf\x7d\xa8\xf4\xf1\x7e\x90\x7b\xd7\xf3\xa5\x3f\xfc\xf5\x2b\
-\x08\xb5\xfe\x1b\x85\x3b\x8f\x96\xfe\xcc\xfc\x6f\x84\x42\x2f\x94\
-\xbe\xd2\xf0\x57\xd0\xc3\x33\xca\x90\x0a\x74\x4f\x5d\x5a\xb6\xf6\
-\xf1\x97\x10\xaa\xdd\x5d\xb6\xe1\x19\x58\xe7\xf1\x78\x59\xe4\x93\
-\x57\x80\x1e\xee\x2d\xbb\xb4\x11\x74\x3f\xb8\x50\xa6\xce\xfe\x00\
-\xf4\xe1\x00\x85\xeb\xff\x5e\xf6\x9e\x47\x7a\x40\xff\xbe\x56\xf6\
-\xd1\x87\x3e\x80\xd0\xea\xc3\x65\xb7\xed\x81\xe7\x27\xbe\x58\xf6\
-\xf2\xe6\x30\x42\x15\x97\x94\xbd\xfd\x89\x97\x61\xfd\xfe\x52\xbe\
-\xf6\x7b\x3f\x85\xf5\xd9\x5b\xde\xf2\x47\xf8\xbe\xab\xa4\x7c\xf0\
-\x11\xe0\x77\xf5\x58\xb9\x92\x82\x79\x2f\xfd\x71\xf9\x8d\xf7\x01\
-\x9f\x53\x5f\x2a\x3f\x82\xf5\xee\x9c\xed\xe5\x77\xf5\x0d\x03\x5f\
-\x3f\x2a\xff\xad\xbe\x16\xf4\xe9\xf7\xbe\xb6\x3f\x80\x9d\x8c\xaf\
-\xf6\x6d\xfc\x12\xcc\xbb\xa4\x9f\xc2\x3a\x95\xc2\x0b\x2a\x7d\xa7\
-\x2f\xbb\x1c\xe4\x60\xf8\xd4\xeb\x60\xbd\xb7\xfe\xc1\x67\xcc\x00\
-\x7f\xe3\x8f\xfa\xe6\xff\xeb\x01\x58\x9f\x5b\x28\x3c\xa3\xc1\x77\
-\xed\xf6\x4b\x81\x8f\xcf\xf9\x0e\x0e\xc2\xfc\x4f\xb9\xd5\x77\x70\
-\xe8\x0c\xe0\x6f\xad\xef\xe0\x83\xdf\x05\x7d\xee\xa6\x70\xf7\x3d\
-\x14\x5e\x7c\xad\xef\x96\x83\xa7\x83\xbc\x64\x0a\x77\xff\xdd\x77\
-\xe4\x61\xb0\xf7\x89\x2d\xbe\x3b\x1e\x7f\x08\xec\xeb\x2f\xbe\xaf\
-\x9b\xc0\x57\xcb\xcd\xbe\x67\xa6\xe1\xf3\xd5\x3f\xa5\xb0\xeb\x4a\
-\xdf\xf3\xef\xbc\x19\xec\xbd\xc4\xf7\xcb\xc7\xaa\x11\x5a\x7b\x83\
-\xef\x4f\xf7\xf9\x60\x1e\x5f\xf5\x87\xb6\x2d\x05\xff\x73\x96\xbf\
-\xf7\xd6\x20\xac\x47\x2f\x85\x23\x4f\x50\xb8\x73\x8d\x3f\x7c\xcd\
-\xcf\x60\x7d\x97\xf9\x77\x9b\xa0\x47\xed\x4f\xfa\x77\x7f\x1e\xf4\
-\xb2\xf1\x1a\x0a\xb7\x86\xfd\x17\xaf\x05\x3f\x54\x33\xe5\xbf\x74\
-\xef\x66\xd0\xa7\x0f\xfa\xf7\xfe\x7c\x39\xd8\x25\xa2\xf0\x9c\x77\
-\xfb\x6f\x44\x11\xb0\xcf\x6f\xfa\x0f\xdd\x3d\x81\x50\xef\xf7\xfd\
-\xb7\xd4\x9f\x03\xb0\xc1\x7f\xe7\x7f\xc0\xbc\x2f\xba\xd4\x7f\xb7\
-\x0f\xe4\xd4\xdc\xe5\x7f\xe0\x1b\x2b\x81\xdf\x7a\xff\xb7\xbe\xa7\
-\x80\x1c\x7e\xe2\x7f\xf6\x29\xf0\x79\x0d\xcb\x2a\x6a\x67\x80\x4e\
-\xe9\x85\x14\x0e\x9e\x5e\xd1\x70\x19\xd8\x79\xf5\xf6\x8a\xb6\xad\
-\xa0\xff\xf5\x2d\x15\x1b\xa6\x3e\x05\xf6\x75\xb4\x62\xd4\x80\x75\
-\x29\xfb\x32\x85\x63\xcf\x51\xb8\x7b\x3d\x85\x7b\xde\xae\xd8\xfd\
-\xc4\x31\xf8\xfe\x77\x14\xee\xbe\x82\xc2\x8b\x7b\x2b\x62\x47\x61\
-\xbc\xb6\x0f\x56\x10\xfb\xe9\x5f\x59\x71\xe8\x56\x90\x87\x7f\xa8\
-\xe2\xf0\x9f\x5e\x05\xff\xf0\x46\xc5\xed\xcf\xbc\x17\xe4\xb1\xbe\
-\xe2\x37\x7f\xc1\xfc\xbc\x16\x68\xf8\xeb\xaf\xc0\xde\xef\xa7\xb0\
-\xf3\x3e\x0a\xcf\xbc\x99\xc2\x6d\xe1\x40\x77\x27\x8c\x77\x4a\x67\
-\x60\xbb\x7a\x2a\xd8\xed\x23\x14\xae\x6f\x0d\x6c\xbf\x0b\xbe\x5f\
-\xe3\xa3\x70\xbd\x16\x98\xfa\xb3\x00\xe3\xfe\x98\xc2\xa9\x9f\x06\
-\xc4\xd5\x60\xc7\xad\xbf\xa6\x70\x57\x5f\x60\xfa\xff\xbe\x06\x76\
-\xfd\x4a\x20\x39\x80\xd7\xeb\x07\x81\x1b\xeb\x60\xfd\x2e\xbc\x29\
-\xf0\x91\xcb\x81\x3f\x74\x11\x85\xe7\x5e\x1d\x38\xd4\x0c\xfe\x31\
-\x7c\x5b\xe0\xd0\x0e\x80\x03\xd5\x81\x4f\x6e\xfe\x1c\xe0\x6d\x0b\
-\xdc\xf5\x10\xe8\x6b\xdf\xaa\xc0\x23\x8f\x82\x1e\x37\x7f\x30\xf0\
-\xc4\x0f\x40\xde\xc2\x50\xe0\xb9\x09\xf0\x87\xe8\x1a\x0a\xcf\xfb\
-\x62\xe0\xc5\x8d\xa0\x6f\xd5\x37\x51\xd8\xfe\xa1\x4a\x74\xcb\x01\
-\xf0\x1b\xef\xa8\x5c\xfb\x34\xd0\xeb\x51\x2a\xcd\xb3\xc0\x0e\x1b\
-\x8e\x56\x1e\x34\x41\x7f\x57\x6e\xaa\x3c\xd2\x75\x27\xe8\x75\xa0\
-\xf2\xd8\xd4\x9b\x60\xaf\x47\x2a\x5f\xb9\xe2\xe3\x08\x9d\x7f\x7f\
-\xe5\x1f\x1b\xdf\x05\x76\xba\xbc\xf2\xed\x30\xac\xc7\x04\x0a\x96\
-\x3e\x0a\xfa\xbc\x6a\x5b\xb0\x66\x3f\xe8\x4d\xe4\xcb\xc1\xfe\xa5\
-\x60\x8f\x8d\x4f\x07\xa5\x0e\xd0\x97\xc6\x0e\x0a\x07\x5f\x0f\x4a\
-\x1f\x01\xfb\x3a\xeb\xf4\xe0\x75\xd7\x82\x7e\xb4\x9c\x1d\x7c\xf8\
-\x26\x98\xf7\xf6\x58\xf0\xc5\xce\xff\x05\xbb\x5a\xa0\xb0\xee\xab\
-\x14\x5e\x70\x51\xf0\xa5\x4a\xd8\x8f\x82\x6b\x83\xbf\x99\x01\x7b\
-\xad\x78\x2a\xf8\xda\xab\xd7\xc2\x73\xa5\x14\xd6\x9d\x42\xe1\xf9\
-\xd1\x20\xd1\xef\xda\x3b\xaa\x1a\x8f\x81\x5e\x9e\x7b\x5a\xd5\x49\
-\x5d\xe0\x57\x96\xae\xac\x3a\xf9\xf9\x05\x98\x77\x67\xd5\xc9\xaf\
-\x81\x1f\xe8\xd8\x5e\x75\xde\x10\xac\xfb\xb6\xeb\xab\xae\xff\x80\
-\x01\xf6\x73\xa0\xea\xc3\x7f\x00\x3e\x76\x34\x54\x7d\xf6\xf9\x10\
-\xcc\xf7\xcd\xaa\x47\x0f\x80\xdf\xa8\xfe\x51\xd5\xa3\xbf\x04\xb1\
-\x4d\xfd\x4b\xd5\xeb\xef\xfb\x05\xcc\xeb\xdb\xa1\xe6\x31\xa0\x7f\
-\xb2\x1c\xda\x5c\x0d\xf6\xb1\xf5\x23\xa1\xfe\x0e\xb0\xfb\x9d\x6f\
-\x52\xb8\x67\x73\x68\x50\x3d\x0c\x7a\xd2\x13\x1a\xd4\x30\x5c\x08\
-\x8d\xfc\x7b\x0a\xf6\x23\x2d\x34\xfd\x6d\x20\x54\xfa\x46\xc8\xbc\
-\x0a\xfc\xff\xba\x63\xa1\x54\xe9\x83\xc0\xd7\xcd\xa1\x03\x9f\x59\
-\x01\x7a\xf4\x3f\xa1\x8f\xf5\x83\x7f\x5f\x71\x19\x85\x11\x23\xf4\
-\xe9\xdd\xc0\xcf\xb2\x0b\x43\x47\x5f\x01\xbf\xb6\xe9\x41\x0a\xbb\
-\xf7\x86\xee\x7d\x12\xec\x66\xdd\xd1\xd0\xe3\x6f\xc2\xfe\x72\xc6\
-\xe5\xa1\x9f\x1f\xf8\x04\xd8\xe9\xf7\x42\xbf\xf8\x56\x19\xec\x97\
-\xbf\xa9\x5e\xf2\xb7\x65\xa0\x9f\xa3\x14\x9e\xf1\x22\x85\xc3\xa7\
-\x56\x5f\x37\x71\x12\xe8\x41\x2d\x85\x13\x29\x0a\xa7\x9a\xab\x0f\
-\x3f\x0b\xeb\xd0\xb4\xb2\xfa\xf6\x97\xc1\xff\x9d\xdf\x58\xfd\xd8\
-\x33\xa0\x5f\xbd\xfb\x6b\xca\xef\x03\x3e\xcb\xe7\x29\x6c\x1b\xa0\
-\xf0\xa2\x55\x14\xee\xfa\x34\x85\x7b\xe6\x6b\xfa\x6f\x68\x02\x79\
-\xbf\x5c\x33\x3c\x3c\x09\xcf\xdf\x59\xa3\xdd\x03\x31\x4c\xd5\xb3\
-\x35\xef\x1c\xda\x0f\xfe\xf8\xca\x9a\xc3\x57\x42\x7c\x72\xd1\xed\
-\x35\xf7\x44\xbf\x09\xfe\xe2\x7d\xb5\x15\xef\x07\x3b\x5e\xf3\x46\
-\xed\x96\x1b\x61\xdc\x92\xd7\x29\x6c\xb8\x8a\xc2\xbe\x6f\xd4\x8e\
-\x3f\x06\xfa\xb7\xed\xf7\xb5\x37\x85\xc0\x4f\xf7\x5f\x5f\x7b\x08\
-\xc3\xb0\x50\x7b\xe8\x25\xa0\x3f\x7c\xb0\xf6\xc8\x1e\x58\xcf\x2d\
-\x3b\x6b\xbf\xfb\x2e\xd0\xbf\x73\x5e\xaa\x7d\x21\xf1\x6e\xd8\x2f\
-\x6e\xad\x7d\x41\x85\xf5\x5a\xb3\x95\xc2\xf5\xf7\xd5\xbe\xd8\x09\
-\x76\x13\x7c\xbd\xf6\xad\xaf\x80\x1d\x2d\xbf\x09\x36\xa1\x8b\xbf\
-\x0f\x12\x42\xad\xa8\x1f\xc9\x68\x06\x7e\x24\xa4\xc3\x5f\x15\xed\
-\x47\x22\x12\x50\x0c\x3e\x8d\x22\x0d\x99\x04\x8a\xa8\x27\x40\xdc\
-\x19\xfc\x6d\xe8\x97\xa3\xb3\x9a\x29\x47\x85\x7e\x79\x66\x46\xd2\
-\x25\x35\x2a\xf5\x54\xe0\x6f\x4b\x30\xc1\x7a\xd4\x0b\x84\x12\x80\
-\xaa\x5a\x24\x6c\xd4\xc0\x90\xa8\x27\x34\x55\x8e\xda\x8f\xaf\xcb\
-\x79\x5c\x80\xd1\x14\xf8\x49\xc1\x27\x71\xf8\xdd\x44\x5a\x86\x40\
-\x7d\x9a\x80\x10\x31\x75\xc9\x8c\xce\x4a\x31\x9b\x54\x63\x16\x29\
-\x19\x50\x7f\xc5\x8c\x1e\x4a\x23\xcb\xe6\x02\xc3\xb0\x00\x66\x8a\
-\x1f\x8d\xa2\x59\x6b\xde\x02\x1a\x82\xd1\xe3\xf0\x23\x03\x29\x23\
-\x43\xa0\x7a\x28\x15\x8f\xcb\xaa\x21\x4c\xc8\x30\x34\x3b\xf0\x30\
-\xd0\xe8\x07\xbc\x11\x82\x21\x01\xd7\x20\xcb\x0c\x5e\x70\x78\xa2\
-\x5f\x18\x91\x55\x49\xd4\x6d\xa4\xe5\x19\x24\x2c\x6e\x83\x08\x59\
-\x21\xe8\xf6\x74\xab\x30\x62\xc4\x94\x92\x49\x76\x9e\x7e\xc0\x9c\
-\x44\x63\x99\xa7\xca\x86\x27\xc7\x9c\xdf\x4e\xa1\x7e\xe6\xdb\xa9\
-\x7e\xfb\xdb\x8d\x80\x99\x22\x32\xc2\x8b\x4d\xc7\x9e\x86\x7f\x55\
-\x98\x38\xe5\xc3\x24\xdf\x98\xf0\x23\x66\x68\xd4\x8d\x89\xba\xae\
-\xcd\x4f\x8b\x6a\x4c\x18\xd3\x64\x43\xb2\x09\x36\xc1\x60\x32\x4a\
-\x92\x75\xd3\x19\xd2\xb6\xd8\xab\x08\x86\x30\xb5\x90\x64\xd5\xa4\
-\x06\x8d\xc1\x53\x06\xfc\xa4\x1c\x53\x2e\x1f\xd3\x54\x89\xd5\xa6\
-\x08\x91\x49\x0a\x1e\xd4\xe0\xb7\x18\x23\xd6\x40\x44\x56\x53\x86\
-\x26\x33\xa2\x09\x66\xb8\xb1\xc7\xf7\x65\x8d\xdc\x84\xc2\x84\x47\
-\xcc\xa5\x02\x93\xde\x0f\x18\x58\x65\x6c\xc2\x55\x61\x4d\xd7\x25\
-\x45\x34\x65\x4d\xc5\x78\x15\x62\x74\x66\x42\xd1\x4c\x4b\x5d\xb0\
-\xc1\xe0\xb5\xd2\x40\x41\xb4\x8c\xca\x60\x2e\x93\xc0\xa7\x69\xeb\
-\xdb\xb0\x9a\x4c\x99\x60\x25\xa2\xa2\xc5\x73\xe8\x34\xc2\x4a\x60\
-\xb5\xc3\xaa\x12\x23\x74\x5a\x61\x8e\x6d\x19\xec\x8a\x11\x31\x2e\
-\xb4\x1a\x6d\x39\x88\x94\x7f\x25\xb3\x84\x4a\x5a\xe7\x6c\x7d\xc3\
-\xba\x26\x84\x35\x45\xd3\x73\xb0\x57\x80\x40\x93\x96\xe4\xd3\x14\
-\x46\x3c\x28\xec\x92\x63\xe6\x6c\x0e\x85\x55\x3c\x0a\xec\xba\xdb\
-\x34\x7a\x72\x88\xd4\xa3\x41\x0b\x85\x6a\x1c\x8b\x58\xb1\x4b\x56\
-\x63\xda\x7c\x2e\xd2\x2a\xd4\x02\x26\x9e\x84\x1f\xc5\xf2\x4a\x02\
-\x21\xa3\x10\x12\xb6\x0e\x55\xb7\xf4\x26\x93\xca\x82\x30\x28\x2b\
-\xa6\x44\x44\xb0\x44\x84\x0f\xe4\x28\x59\x51\x4a\xdd\xe2\xa2\x05\
-\x8d\xc2\x24\x62\xc4\x05\x12\x92\xb6\xda\xb4\x0c\xc4\x64\x93\x83\
-\x1c\x04\x64\x3a\xba\xc4\x20\xc1\x98\x12\x07\xa9\x06\x90\xb6\x12\
-\x37\x8b\xdd\xad\x3d\x5a\x65\xcb\x56\x49\x95\x74\xd1\xe4\x21\xd7\
-\x01\xf2\x38\x31\x4d\x99\x90\x90\x6d\xab\x01\x74\x1e\xaf\x21\x22\
-\x39\x19\xab\x27\x23\x27\x5f\xcb\x90\xa4\x24\xbd\xd0\xfe\x01\x7f\
-\x98\x47\xf1\x2a\x70\x46\x68\x80\x11\xa6\xc8\x42\x1a\x20\x4a\x8d\
-\x38\x62\x7b\x7a\x81\x96\x09\x5d\x8b\x4a\x86\x51\xd0\x60\xe5\x1d\
-\xef\xe8\xbc\x9a\x2b\x87\x29\x62\xb1\xd8\x68\x7a\x61\x01\x05\x5b\
-\x75\x7a\x47\x85\x29\xcb\x81\x78\x20\x77\x12\xbb\x8b\x83\x28\x6c\
-\xcb\x4b\xa2\x05\xa2\xcc\x29\xcb\x0f\xaa\xc4\xbe\xf1\x67\xb0\x4a\
-\x19\xe2\xcb\x7a\xa7\x35\xb0\xe7\xe4\x82\xa1\xa5\xd4\x98\xa8\x8a\
-\xca\x82\xc1\x55\xaf\xcd\xc0\x1d\xdd\x45\xe8\x5e\x86\xdd\x04\xf5\
-\x93\x32\x48\x27\x05\xbf\xcf\x91\xcf\xc0\xa9\x91\xed\x6a\x1a\x7b\
-\xa4\xcc\x70\x4d\xbd\xb1\x98\xa0\xe9\x82\x91\x9a\x36\x75\x31\x6a\
-\x0a\x31\x29\x2a\x4f\x4b\x8a\xa7\x0c\x89\x73\x9a\x22\x6b\x6c\x5a\
-\x2e\x49\x20\x6a\xad\x10\x1b\x6d\x45\xed\x8c\x7b\xa9\xee\x55\x14\
-\x6c\x20\x92\x21\xb4\xb6\xb7\x71\x49\xf6\x52\xb5\x21\x9b\x33\xcf\
-\x6d\xd6\xf6\xa6\x4c\x2d\xea\x74\x9d\x1e\x44\xd7\xba\x12\xc5\x0e\
-\x15\x6b\x50\xc2\xa1\x3b\x0c\x59\x2d\xae\x8b\x09\x0e\x59\x3f\xea\
-\xc3\x81\x83\xad\x48\x7d\x4a\x8a\x6f\x50\x03\x30\x03\xd3\x1a\x74\
-\x9a\x99\x4b\x79\x9f\x46\x5d\x9f\x07\xe6\xf5\xb0\xcb\x26\xc8\x46\
-\x83\xdd\x20\x5e\xba\xb4\x98\xa3\x44\x2a\x51\x12\xb8\x48\x44\x93\
-\xa8\x8b\x34\xc8\x82\xab\x64\x51\xe8\x33\x78\x71\xf0\x77\x57\xc1\
-\x37\x34\xf0\x92\x32\xbb\x49\x94\x70\x94\xb4\x64\x8c\x7f\x97\x08\
-\xa7\xe9\xfd\x86\x0d\xd8\x4c\xc6\x11\x9c\x15\x16\x55\x55\x33\x85\
-\xa8\xa6\x02\xcf\x92\x0a\x7f\x05\xa2\xae\x86\x30\x2f\x9b\xb3\x42\
-\xcc\x0a\xd9\x4c\xc1\x10\x13\x30\x31\x35\x2e\x60\xa7\x53\x98\x5d\
-\x76\xa5\x89\x83\x15\x00\x09\x59\xb7\x68\x6f\x14\x92\x8a\x24\xc2\
-\x1e\x9f\x82\xbf\xba\x94\xd0\xe6\x24\x61\x3a\x65\x9a\x5c\x15\xe8\
-\xf1\x94\xa0\x08\x9f\x62\x13\xa1\x72\x6b\x46\x5d\xf0\xef\x30\x38\
-\xbe\x01\xa2\x28\x1a\x63\x91\x8d\x16\x43\x5a\x52\x52\x85\xe6\x2e\
-\x61\x78\x7c\x00\xe2\x14\x9e\x49\x5e\x0f\x61\x07\x95\xfd\x31\x62\
-\xf7\xb9\xa3\xeb\x24\x80\xd0\xc9\xae\x90\xb2\x54\xb3\xb0\xd5\x13\
-\x0b\x5e\xbd\x39\xb2\x76\x06\xa3\xe4\x1d\xd6\x4c\x92\x8a\xb8\xc0\
-\x5b\x30\x89\xbf\x5c\xf0\xf1\x35\x9e\x72\x35\x88\x57\x9b\xfb\x27\
-\x69\x64\x7a\x4e\xb6\x0d\x9d\x66\xcd\x69\x5e\x97\xf9\x5a\x98\x7f\
-\x52\x21\x88\x79\xd2\x6e\xd9\x1e\xa0\x22\x3c\x0b\x23\x48\x0a\x07\
-\xb1\x1b\x82\x95\x28\x70\x16\x27\x21\x83\x40\x64\xc1\x3a\xc5\x74\
-\xd4\xcb\x48\xc6\x4e\x74\xc2\xb3\x9a\x06\x1a\x3d\x03\x5e\x52\x30\
-\x35\x3a\x0f\xce\x58\x8d\xc0\xa4\x62\x49\xc7\x96\x2e\x13\xcd\x87\
-\x15\xd8\x9a\x84\x08\x16\x04\x37\x28\x09\x67\xbb\x10\x36\x32\xcd\
-\xd8\x35\x87\xc4\xaa\x5c\x12\xec\x7a\xdb\xe9\x14\x43\x8e\xf2\x55\
-\x98\x23\x28\x0b\xa7\x3c\x63\x01\xc7\x83\x95\xf0\x20\x7f\xc2\x8e\
-\xc7\x2f\xe8\x4f\xe9\xe4\xdb\x1e\x01\x22\x00\xc1\x90\xa2\x1d\xc1\
-\xa0\xb5\xc8\xf0\x51\xd7\xd5\x42\x30\x18\x01\x8d\xe9\x10\x06\x75\
-\xe9\xaa\x0e\xf8\xa8\x1b\x7f\xd4\x27\x9b\x06\xfc\x7e\x3a\x2f\x66\
-\x08\x80\xfb\xc0\x49\x16\x13\x33\x0d\xec\xe3\xc6\x77\xb9\x18\x75\
-\x18\x43\x60\x9e\xe6\x6e\x9b\x83\x24\x4d\xeb\x26\xf9\x25\x36\x2a\
-\xbc\xcb\xcf\x90\xa0\x57\x76\xb8\xec\xd0\xe0\xf0\x64\xb7\x30\xa1\
-\x4b\x86\x64\xf2\x6c\xa0\x86\x89\x7a\x06\xd1\xa8\x6d\x05\x83\xfc\
-\x98\xc7\x21\xe1\xba\x4c\x02\x1d\xd6\xb0\xe5\xed\xe3\x4e\x61\xf1\
-\x89\xb1\xa7\x89\x14\x95\x29\x7b\x50\x59\x4c\xea\xec\x19\x31\xb8\
-\xe7\xd2\x9c\xc7\xdd\x92\x6b\x4f\x09\x2e\x3a\x57\xf4\x74\x0e\x03\
-\x56\x49\x66\x36\x27\x4b\xf7\x8d\x88\xd3\x5c\x67\x58\x67\x25\xd3\
-\xb2\x95\x74\x31\x59\xf7\x88\x34\xc3\xb3\x85\x76\x4e\x95\x88\x66\
-\xa0\x73\x24\x82\x53\x18\x9a\x75\x23\xd2\x9c\xa4\x30\x45\x22\x0e\
-\xfd\x26\xe2\xdf\xf5\x4c\x56\x97\xeb\x3c\x83\x23\x9a\x18\xcb\xeb\
-\x3b\x57\x40\x36\x20\x92\x72\x81\x98\x89\x7a\x67\x61\xae\x09\xf8\
-\x1f\x13\xfb\x8e\x8a\x6a\x4a\x54\x84\xd6\x59\x33\xa1\xf0\x62\xdf\
-\xe5\x2e\xe4\x92\x30\xe9\x19\x86\x58\x28\x4d\x2c\x19\x9b\xf1\xa4\
-\xe5\x4c\x6f\x46\x35\x55\xe3\xa6\x52\x11\x6b\xff\x36\x89\x30\xb0\
-\xb5\xfd\xd5\x76\xa9\xa3\x38\xbc\xea\xd7\xe6\x79\xde\xa7\x3e\x8b\
-\x84\xc1\x04\xc5\x15\x84\xc0\x0e\xcf\xbc\x0f\xe1\xa2\x5c\x84\x2c\
-\xa7\x64\x47\xf9\x40\x04\xa7\x2c\x0a\xd1\x3e\x9c\x80\xdb\x7a\x57\
-\x3f\x9a\x52\x4c\x19\x6f\xe3\x11\x49\x91\xa2\x3c\xc7\xe8\xf4\x45\
-\x6e\x55\x25\x4f\xc7\x31\x66\x25\x4c\xd8\x8a\xb0\x13\x4c\x38\x8a\
-\x4c\x95\x63\xd2\xbc\xa0\x8a\x09\x5a\xe8\xf1\xcc\x3a\xd8\x9a\x13\
-\x95\x4b\xd6\x34\xed\x65\x1d\xd3\xf2\x4f\xc7\x95\x66\x8e\xe8\xec\
-\xe0\x9c\xa5\x29\x14\xfe\x87\x1b\x18\x31\xf5\x3c\xdb\x13\xe4\x13\
-\x67\xde\xea\x9b\xa7\x62\xf4\x13\xef\x91\xb4\xac\x35\xed\x81\x59\
-\xaf\xc2\x64\xfd\xe3\x90\xc1\xe6\xf1\x2c\x82\x2b\xc5\x98\x5d\x18\
-\xb2\x97\x18\x53\x9b\x94\xe3\xb3\x3c\x72\x13\xc4\xc5\x09\xc4\xbb\
-\xbe\x41\x58\xb3\xcd\x20\x1d\xf5\xd2\xe2\x99\x40\xa6\xce\xb8\x9a\
-\x4c\xe1\x19\x33\x30\x47\x9e\x62\xbd\x6b\xf3\xb8\xaa\x2c\x08\x38\
-\x80\x23\x91\xac\x10\x15\x55\x61\x5a\x12\x70\xb2\x13\x13\x44\x08\
-\x0b\x04\x53\x4e\xf0\x64\x37\x93\xc5\x5a\xd4\x4a\x3a\x65\x17\xd6\
-\x68\x98\x9a\x56\xf3\xb4\x9f\x2d\x8e\xe1\xf5\xee\x0c\x83\x2b\x06\
-\x33\x29\x8c\xe5\x6c\x69\xf2\x58\x2e\x8e\xb9\x53\x09\x73\x0e\xc6\
-\xa2\x10\xe7\xc5\x0b\x64\x2c\x06\x8c\xa5\x07\x8e\x91\x64\xc5\x99\
-\xce\xb8\x0c\xcd\xa4\x7b\x69\x06\xa9\x05\x48\xd6\x54\xa2\x44\xda\
-\x54\x0f\x45\x47\x84\xd6\x46\x98\x35\xe7\xb5\x74\x12\x93\xe6\x18\
-\x42\x28\x51\x2f\x90\xe5\xd9\x7f\x12\xcb\xce\x28\x9f\x65\x7b\x93\
-\x27\xdb\x99\xa0\xbf\x30\xd6\x03\xe0\x64\x34\x47\xba\x5a\x3e\x21\
-\xab\x57\x72\xf7\x9f\x49\x47\x1a\xed\x88\xbb\x27\x20\xc7\xe5\xe0\
-\xe2\x02\x29\x5e\x81\x99\xcc\x79\x90\xc6\x1c\x4f\x50\x41\xb0\x7e\
-\xa1\x1a\x57\x26\x85\x5d\xe2\x9c\x34\xa3\xe9\xbc\xea\x50\x83\x15\
-\x88\xb3\x41\x0c\x53\xf4\x87\x08\xdc\x0a\x54\x0a\x4b\x82\x96\x4d\
-\x2c\x98\xb3\xe0\xc7\x49\x4c\x22\xf4\xe6\x2f\x07\x06\x2d\x31\x1a\
-\x8c\xc3\x2d\x9b\xe4\x86\xa7\x35\x44\x8e\x99\x5a\x61\x06\xcd\x3f\
-\x49\xaa\x2c\xdc\xd0\xc5\x81\x09\xb2\x33\xd3\x95\x41\x3b\xa6\xa2\
-\x54\x84\x5e\x85\x1f\x35\x4e\xd2\xd8\x1a\xa8\xc9\x8e\x6c\x14\xb8\
-\xc0\xbe\x84\x5b\x01\x0d\x33\x2e\x03\xe7\x2d\xb4\xbc\xd0\x01\xbf\
-\x87\xbd\x0a\x0a\xf6\xfe\x31\x29\xd1\xfa\x00\x77\x03\xec\xcf\xec\
-\x15\x4c\x65\x9b\xbb\x4f\x38\xa3\x90\x49\x0d\xd4\x67\x54\x02\xdb\
-\x88\x5c\x95\x02\x73\xce\x13\x99\xa5\x2b\x05\x69\x87\xc1\x94\x23\
-\x22\x22\x16\x26\x3f\x87\x8b\x58\xd9\x8a\x33\xef\xf1\x45\xa2\x22\
-\x77\x9a\xeb\x9c\x88\x99\x2d\xc2\x3d\xf4\xae\x22\xe4\x04\x12\x80\
-\x73\xcb\x04\xd9\xb1\x8a\xe8\xae\x27\x34\x68\xc9\xab\x27\x11\xab\
-\xac\xa2\x52\x7a\x8c\x60\x64\x25\x4f\x02\x50\xf0\x39\x9f\xa7\xba\
-\xd3\x43\x29\x93\x2a\x82\x6b\x21\xb9\x2a\x92\x84\x59\xe8\xf9\x8a\
-\xc8\x35\x4e\x52\x0c\x1b\x04\x3d\xe5\x89\xeb\x50\xab\x8d\x91\x54\
-\x32\xa9\xe9\xd8\xc5\x52\x07\x91\xae\xb5\x77\xcc\x8b\x73\x6d\xe7\
-\x9e\x5b\x50\xf9\xdd\x41\x71\xe9\x4e\x51\x49\xc1\xf3\xf8\x0c\x42\
-\x9b\x11\x74\xbc\x5b\x72\xbd\xcd\x4e\xb2\xa8\x6c\xa4\xee\xdf\x29\
-\x6b\x4a\x9e\x83\xa2\x5e\xd0\xa7\x39\x12\x92\x31\x0b\xb8\x4b\xd4\
-\x55\x59\xe5\x25\xa6\x8d\x68\x9c\xeb\xa5\x03\x05\x38\xe8\x10\xea\
-\x23\x7e\x02\x6f\x69\x8c\x2d\xef\x9a\xe5\xd7\xdd\x1a\xc8\xa6\x6d\
-\x90\x2a\x5e\xe6\x2c\xdb\x1e\x18\xe7\x17\x49\xd1\xfb\xe8\x89\x50\
-\xa0\x7b\x42\xc2\x9b\x82\x61\x6a\xbc\x8c\xa9\x9e\xe1\x41\x24\xbb\
-\x37\xa3\x38\xb3\xe0\x8c\xf2\x72\xe0\x9c\x83\x73\x97\xa8\x50\xb4\
-\x79\x1e\x01\x67\x7a\xa9\xf2\x63\xf8\x49\xfe\x71\x17\xac\xdf\x26\
-\x92\xc5\xb0\x65\xd3\xec\x82\x69\x94\xc9\xd6\x59\x3f\xd6\x9c\x75\
-\x38\x26\x6c\x12\xb2\x8a\xa8\x0a\xa4\xf1\x05\x4d\x63\x15\xae\x00\
-\xca\x86\x10\x24\x75\x3f\x5c\xe8\x8b\xf5\x09\x26\xc4\x88\xf8\x13\
-\xef\x52\x9f\x83\xc6\x72\x8b\x46\x36\x85\x42\xf1\x6b\x31\x3e\x46\
-\xb6\x2a\x8d\x1c\xa9\xb6\xe6\x9c\x4c\x2b\x56\xd2\xcc\x1e\x2f\xcf\
-\x32\xb2\xaa\xa6\x87\xd4\x61\x12\xf6\x92\xa5\x0d\x61\xd2\x0b\xd6\
-\x07\x84\xaa\x02\xbb\xa4\xcc\x58\x94\x0b\x3d\x2b\x4f\x50\x1d\x65\
-\x6c\x1c\x0e\x76\x90\xa3\x3b\x96\xa7\x74\xbf\x80\x2b\x5f\xe8\x02\
-\x3b\xde\x9d\x9a\x85\x40\x48\x80\xbd\x50\x48\xa9\x86\x88\x13\x1c\
-\x1a\x9c\x1b\x1d\x82\x83\xe9\x0b\xdc\xb9\x5e\x51\xd0\x29\x7d\x28\
-\xfb\x90\xbe\x91\x10\xc2\xd5\x50\xab\x18\x4a\xab\x61\x96\x53\x0e\
-\x5b\x07\x86\xb8\x08\xc5\x74\x14\x85\x53\xa6\x36\x33\xd3\x23\x70\
-\x09\x38\x15\x6b\x00\xbc\xf1\x14\xb8\x4f\x43\x26\x79\x78\x1f\xae\
-\x3f\x6c\x11\x28\x21\xa1\x3d\x1f\x27\x2b\xc0\xd1\xe9\x44\x74\xb4\
-\x2a\x32\x63\x4f\x8d\xe1\xab\x86\x4e\x4b\x18\xd7\x63\x92\x9e\x87\
-\x3b\xb2\x13\xdb\x5d\x34\x31\xc6\xe2\xb2\xc9\x56\x5b\x64\x49\x4b\
-\x4b\x5e\xaa\x6b\x1d\x42\xa3\xe9\x46\x92\xd8\xb8\x9c\xd3\xa5\x53\
-\x3b\x04\x4e\x0a\x28\x17\x24\x4f\x17\xda\x58\x1c\x33\x1e\xb4\x6b\
-\x46\xb4\xf9\x22\x48\x6f\x43\xc3\x24\x27\xa2\x41\x89\xb3\x3f\x29\
-\x66\x85\xb2\x3a\xf9\xcc\xc8\x3c\x45\xd7\x62\x0b\x09\x2b\x6d\xb6\
-\xda\x33\x2c\x08\x11\x53\xd4\xcd\xe3\x58\xf6\x22\x36\x19\x3e\x99\
-\x82\x77\x1a\x1e\x99\x82\xb7\x9b\x62\xa6\xe4\xbd\xe7\xf0\xa8\xd0\
-\x1a\x69\x92\xd0\xa2\x31\x31\x6d\x4d\x92\x19\x05\x08\x92\x5e\x24\
-\x61\x54\x4c\x92\xf2\xdc\x52\xd1\x79\xa2\x9f\x69\xf0\x69\x21\x39\
-\xf2\x1c\x59\xdd\xa4\x95\xfb\x3a\x57\xb8\x15\x35\x33\xb5\xd7\xaa\
-\xf1\x39\x49\x57\xc4\xa4\xd0\xda\xdc\x96\x87\x70\x3f\x39\xcc\x15\
-\xad\xb4\x3a\xbb\xf9\x28\xbb\xf9\x6a\x09\xf5\xec\x10\x41\xab\x71\
-\x73\x36\xdd\x86\xe5\x49\xbe\xd0\x6e\x26\x4f\x02\xcb\xb3\xf2\xa4\
-\xa8\xcb\x69\x67\x0d\x75\xb1\x02\x73\xe8\xb9\x94\xba\x65\xeb\x93\
-\x2c\x77\x99\xa1\xc0\x96\x49\x33\x87\x69\x5c\xf4\x02\x0e\x0a\x3c\
-\x71\xf3\x25\x64\x9e\x88\x45\x9d\x7b\x32\x35\x0c\x86\x84\x40\x3c\
-\x87\x49\x2c\x6c\xce\xaa\xa8\xd0\xce\xba\x04\x5e\x5e\xb6\x17\xb4\
-\x5f\xc2\x27\xed\xad\x09\xa3\x8d\xca\xc2\x83\x62\x4b\x8e\x63\x96\
-\x5d\x46\xc8\xa1\x6b\xfb\x67\x0f\xba\x85\x1c\xc5\xb8\x63\xae\x70\
-\x2c\xad\x40\xc2\x38\x93\x9e\x26\x31\x7c\xd4\x8d\xa7\x4c\x7c\xa0\
-\xe4\x58\x6f\x0f\x8a\x79\x53\x68\xef\x29\xd8\xc5\xbe\x2e\x56\xcb\
-\x68\xc6\xd3\x95\x57\x02\x36\x7a\x77\x2e\x7a\x37\x17\xbd\x91\x34\
-\x72\xd0\xea\xa8\x4d\x88\xd9\x29\x29\x11\x72\x24\xc6\x25\xb4\xca\
-\xca\xac\x6d\xe3\x93\x5d\xcf\xca\xab\x22\xf3\xe0\x68\x98\x43\x72\
-\x77\x72\x9e\x2d\x48\x4b\xe3\x56\x83\x1f\xa9\xcd\x3b\x04\x91\xb7\
-\x09\xc9\x13\xb7\x29\xcb\xaf\xe5\x2a\x7a\x4d\xfa\x48\x9d\xea\x3a\
-\x97\x5a\x3d\x09\x6d\x70\x2f\x1a\x8e\x08\x65\x87\x3c\x7d\x03\xa2\
-\x15\xc7\x78\xa2\x2f\x67\x3b\x1b\x91\xa3\x1d\xd8\x66\x27\xdd\xe6\
-\x68\x9f\xf8\x70\x04\x93\xdf\x0b\x79\xe1\xe6\x3b\x17\xf1\x44\xcc\
-\x8d\xc4\xdc\xbb\x9a\x43\x4c\x57\x33\x5f\x2c\x9c\xea\xa9\x27\x0e\
-\x6e\x0e\xa6\xd5\x31\xc9\x75\x55\xab\x26\xc5\x44\xd2\x28\x60\x49\
-\x79\x35\x47\x8e\xf0\xf2\xb8\x70\x2f\xc4\xcd\x99\x02\x5f\x11\x3d\
-\x51\x8c\xc9\xa6\x5b\xd2\x26\x2d\x37\xcf\x91\x4f\xb1\xd6\xef\x49\
-\xaa\x83\xb4\x22\x64\x6a\x68\xd6\x99\x51\xba\xfc\x63\x9f\xfb\xc6\
-\xc0\xb0\xd9\x25\x68\x48\x97\x83\x68\x99\x4d\x68\x8d\xf5\xe5\x5d\
-\x0b\x6e\x45\x86\xb3\x1c\xfc\xb2\x08\xc7\x9e\x75\x2b\x0f\x6c\x45\
-\x43\xb0\x18\x2c\xfb\x41\x5d\xea\x10\x5a\x87\xf6\xb7\xe5\x11\x4f\
-\x01\xde\xa9\x31\x8d\x9b\xae\xd3\x1d\xaf\x83\xe2\x11\x2c\xcc\x47\
-\xf1\x28\xac\x72\x55\xd2\x5c\x09\xd5\xe2\x1e\xa3\x94\xa4\x46\x17\
-\xa8\x9c\xf2\xd1\x15\xb2\xdc\x9f\xe1\x59\xd0\x5c\x92\x71\x82\x6c\
-\x65\x93\x47\xbb\x0e\x02\x9b\x11\xd2\xf1\x62\x29\xa2\x1d\xed\x0f\
-\x8f\xf4\x13\xdd\x2b\x84\xc4\x94\x45\x22\xe5\x08\x76\x03\xc3\x53\
-\x40\x22\x65\x14\x40\x22\xaf\x43\xe6\xeb\x42\xb6\xa5\x65\x4f\xa6\
-\x2a\xcb\x94\xf8\xe2\x1e\x24\x39\x0b\xb5\x4e\x2c\xf2\x98\x65\x25\
-\xb8\x43\x81\x5d\xc8\xba\x89\x59\xdc\x9c\xda\xaa\x8b\x31\x19\xd2\
-\xbf\xfc\xa4\x8b\xf5\xbe\x7c\x7d\x9d\xcc\x3a\x72\x62\x4e\xb4\x27\
-\x25\xa6\x35\x86\x47\x25\x9f\x47\xe6\xe1\x9e\x68\xa7\xcc\x9f\x6d\
-\x81\x65\x7c\xbe\xf8\x8b\x75\xee\x7c\x73\x8f\x10\x6a\x09\x32\x6d\
-\x9a\x99\xd2\xfe\x35\x67\x7a\x15\xc2\xed\xf6\xe3\xba\x1c\x97\x55\
-\x51\x71\xb8\x44\x32\x9c\x43\x8f\x59\x8a\x29\xeb\x2e\x01\x4b\x2b\
-\x80\x69\x45\xac\xa3\x31\x4f\x3a\xf8\xa6\x9c\x62\xe5\x12\xf4\xec\
-\x96\x49\x78\x7a\x71\x9d\x07\x62\x4b\xab\xea\xee\x49\xe4\x3c\x30\
-\x2a\x5c\xd9\x8b\x93\x1a\xde\x7e\xc7\xea\xb2\x85\x93\x56\x52\xcf\
-\xa5\xa9\x8b\x41\x4e\x06\x65\x36\xdf\xc5\xd5\x90\x79\x7c\x55\x47\
-\x68\x0d\x4b\xaa\x69\xe5\xbb\x5e\x83\x76\x14\x3c\x28\x71\xaa\xb6\
-\xaf\x67\x86\x01\x97\xca\x1d\xa3\x98\xb0\x38\x1b\xf7\xcc\x1c\x4f\
-\x93\x3e\xdc\xa7\x75\x04\x2a\x86\xb4\xff\xc1\x5a\x36\x01\x18\x36\
-\x9f\x4d\xb8\x39\x52\x53\x71\x83\x72\xc6\x23\x09\x91\x89\x11\x3e\
-\xc7\x7e\x92\xc0\xda\x5d\x91\xfe\xb0\x66\xc8\x2a\x5f\x07\x4e\xe0\
-\xf5\x4b\xcf\x31\x1a\xdd\xf7\x60\xdb\x9e\x1c\x3b\x70\x1e\x95\xf5\
-\xde\x7d\xcb\xf1\xee\xcb\xc5\xae\x01\x4f\xd4\xe9\xa2\x16\x15\x83\
-\x9d\xf9\xf5\x61\x05\x6f\xdb\x66\xea\xae\x8e\x4d\x9b\x4b\x31\x00\
-\x1b\xb6\x88\x3d\x81\x3d\x85\xad\xa2\xac\xe6\xb1\xfd\xec\x4d\x3e\
-\xbb\x51\xd1\xce\x70\x32\xcd\x8a\x5c\x0f\x50\xd0\x5d\x59\x4f\x0a\
-\xdd\x39\x9a\x2e\xa2\xec\xeb\xb4\x5e\x5a\x7e\x52\xa6\x17\xb8\x08\
-\x25\x3f\xdf\xa3\xc4\xe2\x36\x2c\xcf\xe3\x34\xd9\x37\x79\x93\x62\
-\x14\xef\x2f\x85\x38\x9e\x13\x72\x5b\x98\x63\x28\x45\x5e\x20\xf6\
-\xa4\xd4\xe9\xaa\xac\xb9\xf5\xf7\x5c\x05\x26\x75\x78\xda\xde\x9e\
-\x5f\x83\xb3\xc5\xe1\x3a\x88\x6d\xe7\x84\x74\x41\x6a\x85\x6f\x89\
-\xe2\x22\x7a\x92\x4b\xb0\x92\x10\x8c\x58\xf5\x6a\x4f\x62\xc7\xd3\
-\x47\xce\xe1\x30\xdd\x03\xee\x12\xfc\xd9\x04\x71\x17\x78\x26\xf0\
-\xcb\xb3\xf8\x45\xb5\xa6\x7b\xd2\x59\x4c\x73\x3a\x67\x4b\x71\x6f\
-\x4f\xe7\x78\x14\xbb\x7c\x41\x50\xd9\xba\x1a\x20\xdb\xd7\xb0\xb9\
-\x63\xba\xf5\xb8\x73\x67\x9c\xce\x2c\x12\x44\x0f\x75\x2b\x8f\x66\
-\x17\x02\xe7\x18\x09\x39\xaa\x6b\x42\x9e\x85\x68\x00\x72\xa6\xe5\
-\x60\xd3\xa5\x7f\xa6\x17\x65\xd8\x94\xe8\x6e\x65\xe4\x09\x1f\x0a\
-\x2f\x1e\x15\x66\xbd\xb9\x27\x5c\x2e\xdb\xcf\x88\x36\x7f\x3c\xc6\
-\x9b\x33\x86\xed\x7b\x30\xe5\xa2\x6d\xd7\x9b\x5e\x00\xd3\xcb\x6b\
-\xba\x93\x05\x04\x52\xd9\x41\x9f\xe3\x15\x02\x9c\xed\x67\x1d\x6d\
-\xff\xa6\x07\x71\x8b\x0a\xb8\x4e\xe0\xcb\x0c\x3c\xc7\xe8\xcb\x1a\
-\xa3\x0b\xb9\x5f\xfc\x2b\xc4\xb7\x2f\x1b\xd3\x3a\x84\x2e\xa1\x18\
-\x0f\x5f\xe8\xf0\x85\x28\x67\x03\x1d\xbe\x08\x15\xcd\x8d\x2e\xf4\
-\x1c\x6e\x3c\xa3\x0b\x3a\x5a\xa4\xa3\x98\x15\x3d\xe1\xd2\xee\x3e\
-\x2e\x69\x77\x1f\xaf\xb4\xbb\x4f\xa4\xb4\xbb\xf3\x49\xbb\xbb\x48\
-\x69\x07\x49\xa2\x8d\xbb\xdd\x6c\xff\xea\x1b\xd3\x22\x49\x39\x4f\
-\x0c\x5c\xec\x2b\x3f\x38\x19\x41\x9e\x7b\x08\x5c\xde\x71\xdd\x22\
-\xc2\xd6\x43\xc6\x92\x72\x44\xcb\xe3\x74\x17\x7d\x81\x81\x13\xdf\
-\x2c\xee\x0a\x03\x87\xc9\x49\x94\x75\xc9\x9e\xe9\x0b\xa1\x45\x2f\
-\x5b\xd8\x4b\x69\x79\x2b\x7d\xeb\xde\x98\x95\x93\x7c\xa1\x07\x33\
-\x95\x33\x9b\x88\x9f\x10\xe1\xe3\x15\x72\x90\x91\xbb\x99\xa7\x4b\
-\x69\xe9\x43\xf6\x04\xa3\xb5\x95\xb8\x90\x96\x3f\xeb\x6c\x22\x44\
-\x54\xf2\xb2\x86\x04\x69\x08\xd8\x9f\x55\x2e\xf1\x4f\x82\x37\xd7\
-\x12\x5c\x2a\x05\x9f\x6a\x64\x23\xfe\xd3\x4e\x35\x72\x83\xb7\x08\
-\x09\x92\x71\xf8\x44\xef\x8b\xda\x57\xdd\x2b\x23\xd1\x59\x5d\x93\
-\x62\x12\x3f\xfa\xf4\xd3\xb0\xc7\x5e\xa1\x48\xbe\x0a\x44\xc1\x25\
-\x3b\x4e\xe4\xbc\xe8\xc3\x98\xdc\x1d\xdd\xeb\x00\x9f\x97\x4b\xd6\
-\x16\x93\x42\x6e\x2e\xe2\xbc\xc7\xc5\xcf\xe6\x9e\xfa\xe4\xf7\xb3\
-\x02\x29\xf4\xd9\x39\x2a\x7b\x75\x3e\xab\xa1\xc5\x4a\x54\x33\x0d\
-\x2d\xde\x36\xcc\x7b\xd1\x11\xc7\x06\x0a\x3c\x4a\xca\x8d\xf1\x9d\
-\x2f\x1d\xa2\x2f\x79\x21\x26\x69\x07\x56\x7d\x62\xf4\xca\xb8\x4e\
-\x16\x3b\xf3\xf2\xa1\x25\x49\xfb\x5a\x45\x56\xfb\x18\x4b\x8f\x36\
-\xbc\x68\x64\xd1\xa3\x24\xf5\x66\x1a\x05\xc3\xa2\x3a\x27\x1a\x79\
-\x69\x7a\x75\x22\x49\xde\x9d\x48\x1e\x94\xea\x08\x77\x89\x8c\xd3\
-\x61\xfb\x0d\xb5\x44\x02\x7c\x0d\x0f\xfb\x6c\xb0\x07\xa7\xeb\x6e\
-\x25\x30\x6a\x6d\x75\xb2\x15\x18\xeb\x64\x29\x68\xb7\xb5\xe6\x38\
-\x60\x38\x25\x0c\x42\x34\xf5\x05\x48\x5d\xa5\xab\x52\xb2\x2e\x19\
-\xe0\xde\x0d\xdc\xc1\xd6\xc6\x1b\x18\x6f\x6e\x13\x60\x41\xb4\x83\
-\x57\x27\x9b\x92\x46\xf4\xce\x66\xc6\x1e\x64\x49\xff\xc4\xb0\xb0\
-\x49\x98\x94\x0c\x4d\x49\x91\x4b\xf7\x1c\xd2\x35\xe4\x52\x8e\x6c\
-\x35\x04\x33\x3b\xc0\x56\xdd\xea\xcb\x77\xc7\x3b\xd3\xca\xa6\x69\
-\x8d\xbc\x78\x49\xac\x18\x11\xd5\x78\x4a\x8c\x4b\x45\x8a\xa2\xe8\
-\x97\x64\x79\xd2\xc9\xf6\x16\x58\xc7\xf6\xb1\x1a\x35\x2a\xee\xa3\
-\xce\x80\xc7\x4f\x7b\x96\x46\x65\xbf\x67\xc4\x6d\x81\xaa\xf1\x45\
-\x29\xa1\x00\x85\xab\x73\xdc\x98\x6a\x61\xef\x09\xe1\x0e\xb3\x16\
-\x83\x8b\x8b\xef\x80\xc4\xad\xe3\x90\x16\xc7\x75\x16\x39\xae\x8a\
-\x2d\x0a\x07\x39\x94\xf1\xf7\x2d\x8c\xbd\xfa\xb1\xf3\x68\xe1\x69\
-\x45\x01\xb7\x0c\xdc\x11\xcf\x47\xbb\x88\xa2\x08\xd6\xc5\x6c\x11\
-\x38\xa7\x3d\xeb\xad\x88\xf6\xa3\xe3\xaa\x34\xdd\x3b\x79\x6a\x15\
-\xda\x25\xce\x81\x13\x50\x41\xb1\x74\x9e\x64\x0b\x6d\xec\xf3\x40\
-\x5f\x61\x25\x29\x86\x15\x1d\x28\x4c\xf0\xc2\xc8\x2b\x9a\x32\x4c\
-\x1a\xbc\x78\x6a\x0f\xdd\x0c\xd3\xda\x1c\x23\x11\x87\xdd\xf8\x3d\
-\x67\xd1\x66\xbd\xf1\xd2\x58\x52\x16\xe6\xf0\x95\x11\x01\xbf\x84\
-\x05\x7e\xe3\x1a\x6a\xb7\xc7\x10\xb4\x03\x39\x69\x85\xfb\x49\x22\
-\x63\xcb\xb5\xba\x0d\x65\x6a\x9a\x60\x24\x44\x85\xa7\x35\xe7\x65\
-\xee\x72\x8b\x1e\xf9\x95\xf7\xbb\x66\x98\xb0\x17\xdf\xf8\x76\xc4\
-\x56\x34\xb6\xa8\xd1\xad\x4b\x63\xcc\x88\x13\x8b\x89\xe0\xac\x3d\
-\x44\x47\xe9\xb7\x2c\x81\x6d\x22\xfc\x3e\xa2\x11\xd4\x65\x7b\x6a\
-\xcc\x85\xe3\x55\x4a\x4e\x11\xb8\x71\xd3\x40\x2e\xd4\x65\x8d\x6b\
-\xef\x30\xec\xa5\x37\x37\xf4\x1e\x12\x4d\xc4\xad\xa3\x4c\x93\xa4\
-\x5f\x76\xaf\x52\x0e\x61\x57\xe1\x35\x5a\x83\x60\xa6\x7b\x95\xb8\
-\xa6\xcb\xe6\x6c\xc2\x5b\x7e\xf9\xed\xd5\x0d\x6b\x9d\x6b\x53\xbb\
-\x4a\x32\x8f\x5c\x73\xaa\xb6\x5a\x6e\xed\x8e\xaa\x1c\x9a\x8e\x36\
-\x7e\x3f\x7d\xeb\x0b\x7e\xb0\x16\xdf\x51\xc8\x4d\x2d\x0b\x69\x81\
-\x75\x45\x5d\x0e\xea\x62\xbd\xc1\xce\x52\x84\xf4\xfd\x17\x67\x27\
-\xbe\x24\x0c\x6a\x7a\x42\x34\xbd\x48\xb9\xbf\xf5\xc1\x75\xc8\x1e\
-\x34\x0e\x92\xca\x94\x3b\x91\xf3\x32\x87\x68\xd5\xca\x35\x2b\xaf\
-\x54\x5c\x4f\x9e\xea\xc9\xfd\x43\x1a\x6c\x8f\x27\x33\x25\xd2\x3c\
-\x7c\xf9\x23\x26\x98\xa8\x37\x67\x8b\xe8\xef\xae\x35\xec\x8b\x76\
-\x4c\x8f\xf4\x14\x70\x9e\xb0\xf4\xc1\xd9\x6e\x1d\x18\xd1\xe2\x82\
-\xb8\x4f\x36\x3c\xb1\x8f\xb7\x33\xdc\x95\x68\x13\x38\x06\xcd\xea\
-\x35\x66\x5d\x42\xb7\x3d\xb1\x09\x72\x73\x41\x9b\x11\xba\x39\xac\
-\x9d\x88\xde\x72\x0f\x99\x15\xb6\xfd\xb8\x22\x1f\xc7\xcb\x67\x42\
-\x86\x95\xe5\x2c\xfe\xa5\xa3\xb9\x24\x16\xf5\xe6\xd1\x5c\x32\x8b\
-\x7d\xfd\x68\x2e\xa5\x3a\xc0\xc3\xa2\x11\x10\xbd\xfb\x20\xb9\xeb\
-\xa3\x9b\x30\x8a\xd4\x9b\x5c\x12\x85\xae\x6c\x2e\xe6\xf1\x2c\xeb\
-\xbc\x75\x07\xf3\x38\x96\x35\x87\xc4\xe2\x96\x35\x87\xcc\xa2\x97\
-\xd5\x41\xe9\x5a\xf8\xa4\xb4\xa4\xe4\xff\x01\x5e\x5e\x65\xac\
+\x00\x71\x25\x78\x9c\xcd\x3d\x09\x74\x1c\xc5\x95\xa5\x63\x46\xa3\
+\xd1\xe8\xb0\x24\x0b\x63\x8c\xdd\x18\x5b\x48\xb2\x91\x2d\xd9\x60\
+\x23\x6c\x83\x4e\x4b\xb6\x2e\x34\xf2\x45\x6c\xec\xd6\x4c\x4b\x6a\
+\x98\xe9\x1e\x77\xf7\x48\x96\x13\xb2\x84\x24\x18\xb2\x2c\x26\x80\
+\xc9\xb9\xe0\xec\x06\xc8\xb2\x66\x93\x6c\x82\xd7\x39\xcd\xc6\x2c\
+\x90\x10\xae\x9c\x1b\x20\xc7\x83\x85\x67\x82\x5f\xc8\x26\x10\x72\
+\x40\xb2\xbf\xaa\x7a\xa6\xab\x67\xba\x6b\x7a\x64\x9b\xb7\xe8\x99\
+\x2f\xcf\xf4\xff\xf5\xeb\x5f\xf5\xff\xaf\xaa\xf6\xba\x63\xd1\x79\
+\xdf\x7b\xe3\xb3\x87\x9e\xba\x60\xc1\xf1\x3d\x9f\xfb\xd6\xcf\x1f\
+\x40\x08\xf9\x64\x63\x77\xdf\x68\x07\x42\xc1\xdb\x11\xda\xf4\x28\
+\x42\x15\xcb\x10\x1a\x54\x10\x2a\xf8\x0a\x85\x55\x7f\xa3\x70\xf3\
+\xa5\x00\x3f\x02\x9f\x3f\x47\xe1\x9c\x66\x0a\x37\x3f\x88\xd0\xf6\
+\xaf\x22\x74\xde\x75\x14\x5e\x3e\x8d\x0a\x1f\x02\x3a\xbe\x23\xa8\
+\xe8\x9a\xeb\x11\xf2\x7f\x0c\x15\xdf\xf9\x30\x42\x81\xa7\x28\x5c\
+\x7b\x12\x15\xdf\xfd\x05\xf8\xfb\xbb\x14\x5e\x36\x9f\xc2\xf5\xc7\
+\x28\xec\x6a\x41\xc5\xc7\xae\x46\x68\x45\x39\x85\xdd\x8f\xa1\xe2\
+\x67\x8a\x81\x2f\xc0\xfb\xe9\x5f\xe1\xf3\xaf\x50\xd8\x73\x27\x2a\
+\x3e\xf9\x26\x42\x3b\x8e\x23\xdf\xb2\x1f\x01\x3f\xa7\x28\x6c\x9a\
+\x4b\xe1\xb2\x69\x0a\xdb\x56\x51\x78\xc5\xa3\x14\xf6\x27\x90\xaf\
+\x67\x08\xa1\x1a\x99\xc2\x3d\x6f\x23\xdf\xd6\x6e\x84\x0a\xf7\x51\
+\x38\xf7\x0f\x14\x8e\xd4\x21\x5f\x62\x33\x42\xf3\x97\x50\xd8\xf6\
+\x67\x0a\xc3\x27\x90\x4f\xbb\x05\x3e\xdf\x8a\x7c\x87\xe1\xb9\x2d\
+\x13\xa8\x04\x3f\x7f\xc1\x13\xa8\xfa\x5e\x90\x05\x7a\x92\xc2\x95\
+\x5f\xa4\xb0\xf7\xf3\xa8\xe9\x1b\xc0\x7f\xf1\xbb\xa8\xe9\xd9\xa5\
+\x20\x97\x36\xd4\x74\x6a\x25\xc0\x57\xd1\x32\x3d\x0a\xf2\x39\x1f\
+\xf5\xf5\x69\x08\x2d\x19\x45\x9b\x3f\xfa\x08\xc8\xe3\xf3\x14\x6e\
+\xe8\x45\x43\xe7\xbe\x85\xd0\xbc\xa3\x68\x64\xdf\x37\x61\x7e\x5f\
+\x44\x5b\x36\xc9\x08\x5d\x75\x17\xda\xb2\xe7\x10\xf0\x79\x9c\xc2\
+\x36\x15\x6d\x51\xee\x05\x7e\x87\xd1\xf6\x77\x41\x1e\x0b\x1e\xa1\
+\xb0\xe9\x2a\x0a\x97\x17\x51\x78\xf9\x11\x0a\xdb\x37\x50\x38\x7a\
+\x23\xda\xf1\x49\xe0\xe7\x7c\x05\xed\x04\x1d\xa1\xc2\xa7\x29\x5c\
+\xfb\x6d\x0a\xb7\x0d\xa1\x9d\xbd\x7f\x46\xa8\xb5\x8e\xc2\xcd\x13\
+\x68\xe7\xe1\x51\x78\xee\x5e\x0a\x17\x1e\xa0\xb0\xfd\x55\x0a\xb7\
+\x7c\x0a\xed\xfa\xed\x7d\x08\x09\xb7\x52\xb8\xfe\x72\x0a\xb7\xdd\
+\x84\xae\xf9\x11\xf0\x79\xce\xb5\x68\xec\xd4\xbf\x80\x1e\x36\xa0\
+\x83\x9d\xe7\x22\x74\xa9\x44\xe1\x55\x17\xa2\x3f\x88\x5f\x82\x79\
+\x7c\xa1\xa0\x31\xf9\x5d\x84\x2e\x1e\xa6\xb0\x73\x7b\xc1\xf2\x2b\
+\x13\xa0\xc7\x45\x05\x2b\xd6\x36\x02\x1f\xfd\x14\x6e\x7e\xa1\x60\
+\xc7\x09\xb0\xd5\xa5\x2f\x16\x5c\xbb\x64\x07\x42\xd5\x4f\x17\x68\
+\x07\x17\x82\x3d\x5d\x50\x70\xf0\xbb\xeb\x01\x4e\x15\x7c\x7c\xea\
+\x04\x42\x17\xf6\x16\x7c\xe2\xd3\xf0\xdc\xb2\x2f\x17\x3c\xb8\x68\
+\x0d\x42\x45\x2d\x14\xce\xd9\x45\x61\x44\xa3\x50\xea\x2b\xf8\xfa\
+\xc3\x9b\xc0\x76\x5f\x2f\xf8\xc1\xa2\x97\x00\x56\x16\x76\xfd\x7a\
+\x27\x42\xd7\x5c\x5f\x38\xb3\xa2\x14\xf0\x66\x0a\xf7\x57\xc2\x38\
+\x2b\x14\x0a\x7b\xda\x0b\x0f\x1e\x03\x3d\xac\x78\x9e\xc2\x8d\xdb\
+\x0a\x9f\xe8\x02\x7d\xad\x37\x0a\x7f\xf4\xea\x6b\x08\x35\xfc\x03\
+\x85\x63\x57\x14\x3e\x6f\xfc\x17\x42\xa1\x5f\x16\xbe\x56\xfb\x27\
+\x98\xd7\x31\x0a\x3b\x9f\x2a\x42\x0a\x8c\x77\x61\x4d\xd1\xe2\x27\
+\x5e\x46\xa8\x72\x7b\xd1\xb2\x67\xc1\x4e\xae\xfe\x5b\x51\xf8\x33\
+\xd7\x82\x3d\xbf\x5d\xb4\xab\xae\x1a\xfc\x71\xa6\x48\x99\xfc\x21\
+\xd8\xd5\x01\x0a\x2f\xfa\x4b\xd1\x87\x4e\xb4\x21\x74\xe5\x55\x45\
+\x9f\x38\xfe\x51\x84\x16\x1d\x2e\xba\x77\x07\x3c\xbf\xb3\xa7\xe8\
+\x95\xd5\x9d\x08\x95\xec\x2c\xfa\xeb\xa7\x5f\x01\xfd\xbf\x5d\xbc\
+\xf8\xfb\x3f\x43\x68\xcd\x47\x28\x0c\xbf\x5d\x5c\xff\x26\x3c\xb7\
+\xee\x53\xc5\x3d\x27\x60\x3e\x8b\x06\x8b\x63\x49\x90\x4b\xcd\x4f\
+\x8a\x6f\x3f\x0a\x7c\xef\xd9\x58\x7c\x3f\xb6\xe3\xae\x97\x8b\x1f\
+\xea\xe8\x43\xa8\xb9\x92\xc2\xae\x78\xf1\x6f\xb4\xc5\x60\x9f\xff\
+\xeb\x6b\xfc\x3d\xf8\xe1\xd5\xff\xe1\x5b\xfe\x45\x90\x4f\x41\x17\
+\x85\x55\x0a\x85\x9b\x3e\xe7\x5b\x35\x77\x0f\xc8\xab\xcc\xa7\xdc\
+\x02\x76\xb3\x66\x07\x85\xe1\xbf\xf7\xe9\xe3\xc0\xf7\xfb\x76\xfa\
+\xa6\xff\xf3\xeb\x60\x7f\xcd\x14\x5e\x79\xc4\x77\xf3\xe6\x5d\x60\
+\x7f\xeb\x7c\xb7\xf6\x80\x7c\xce\xbb\xc7\x77\x6b\xef\x25\xc0\xf7\
+\x62\xdf\xad\xdf\xfe\x1e\xf8\x49\x2b\x85\xd1\x3e\x0a\xc7\x05\xdf\
+\xdd\xb7\xae\x02\x79\x16\x50\x18\xbd\xd3\x77\xff\x23\x10\x5f\xde\
+\xf7\x63\xdf\x83\x4f\x1c\x47\x48\x3c\xe8\xfb\x86\x01\xfc\xd5\xdf\
+\xe9\x7b\x76\x0c\x3e\x5f\xf4\x33\x0a\xd7\x17\xf9\x5e\xfc\xc0\x9d\
+\x20\xf7\x02\xdf\x2f\x1e\x2b\x47\x68\xf1\x41\xdf\x5b\x47\x7d\x30\
+\x9f\xaf\xfa\x43\x9b\x6a\x10\x2a\x5d\xe3\x6f\xbf\x27\x08\xfa\x6a\
+\xa7\x70\x7b\x84\x42\xf1\x6b\xfe\xce\x1b\x9e\x87\xbf\x3f\xe4\xdf\
+\x6e\x80\xfd\x35\x3d\xe5\xdf\xfe\x05\xb0\xef\xba\x1b\x28\x1c\x79\
+\xc1\x7f\xf5\x62\x88\x7b\x15\xa3\xfe\x5d\xbb\x57\x83\xfd\xdd\xe4\
+\xdf\xfd\xc2\x7c\xf0\x7b\x44\x61\xf3\x3e\x0a\xbb\xcf\xf1\xdf\x8e\
+\xc2\x08\xb5\xf4\x50\xd8\xb7\xc5\x7f\xe8\x4b\xc3\x08\xad\xba\x8e\
+\xc2\x81\x6b\xfd\x77\x57\x5f\x06\x76\xfd\x38\x85\xfd\x47\xfc\x47\
+\xfe\x15\xe4\xb2\xf3\x2d\xff\x97\x7c\x20\xcf\xa5\x2d\xfe\xaf\x7f\
+\xf3\x7c\x98\x4f\xb5\xff\x3b\xdf\x8f\x81\x9c\xfe\xdb\xff\xdc\xd3\
+\xf7\x20\x54\x3b\xb7\xa4\x72\x1c\xe8\x17\x5e\x49\xe1\xa5\xdf\xa5\
+\xf0\xaa\x27\x4b\x6a\xaf\x81\x38\x53\xbe\xb9\xa4\x71\x23\xf8\x5b\
+\x75\x7d\xc9\xb2\xd1\xcf\x82\x7f\x3f\x50\x32\xa0\x83\x1e\x8b\xfe\
+\x9d\xc2\xab\x55\x0a\x23\xc7\x29\x94\xee\x2e\xd9\xfe\xe4\x49\xf8\
+\xfe\xb7\x14\x46\x0b\x29\x94\x7e\x56\x12\x7d\x00\xc6\x6d\xbc\xa9\
+\x84\xf8\xe9\x25\x0b\x29\x1c\x7a\xb8\xe4\xd0\x3d\x20\x3f\x7f\x6f\
+\xc9\xe1\xb7\x7e\x0d\x71\xea\x63\x25\xf7\x3d\x7b\x23\xf8\xf9\xf1\
+\x92\xd7\xdf\xc6\xfc\x9d\x0a\xd4\xfe\xe9\x57\x10\x77\x8e\x51\xb8\
+\x6e\x90\xc2\x8e\x65\x14\x6e\x79\x21\xd0\xba\x12\xc6\x3d\x6f\x65\
+\x60\xb3\x72\x21\xc4\x8b\x13\x14\x5e\xd4\x10\xd8\xfc\x10\x7c\x7f\
+\x81\x8f\xc2\x8b\xd4\xc0\xe8\x1f\x04\x18\xff\x27\x14\xee\xd9\x1b\
+\x10\x17\x41\xfc\x68\x78\x95\xc2\xb1\xe7\x03\x63\x7f\xfc\x1a\xc4\
+\x93\x0f\x05\x12\xdd\x58\xbf\x3f\x0c\xdc\x5e\x05\xfa\x6e\xbd\x8d\
+\xc2\xfe\xa6\xc0\x5d\x7b\x80\x4f\x74\x15\x85\x1b\xe7\x06\x0e\x2d\
+\x85\xb8\xbd\xfa\x21\x0a\x87\xd6\x04\x0e\x6d\x01\x78\xc9\x9b\x14\
+\x0e\xdf\x17\xf8\xcc\xea\xcf\xc3\x7c\x5e\x0a\x3c\x74\x1c\xec\x7f\
+\xd5\x83\x14\x0e\x1c\x0d\x9c\x78\x14\xfc\x64\xe9\x4d\x81\x27\x7f\
+\x08\xfa\x11\x7a\x03\x3f\x1d\x86\xb8\x8d\x6e\xa0\xb0\xb7\x27\xf0\
+\xd2\x72\xb0\xdf\xf2\x3b\x28\x6c\xfa\x58\x29\xba\xfb\x00\xf8\x79\
+\x4d\xe9\xe2\x67\x80\xee\x8a\x0d\x14\xf6\x14\x97\x1a\x6b\xc0\xef\
+\x6b\x1f\x28\xbd\xd5\x00\xbf\x38\xff\xe2\xd2\xfb\x5b\x8e\x20\xb4\
+\xeb\x70\xe9\xc9\xd1\x77\x20\x4e\xdc\x5f\xfa\xda\xb5\x9f\x02\x7b\
+\xf9\x01\x85\x9b\x86\x4b\xdf\xac\xfb\x20\xc4\x87\xf9\xa5\x7f\xed\
+\x04\x3d\xbe\xef\x93\xc1\xc2\x47\xc1\x5f\x16\x6e\x0a\x56\xec\x07\
+\xbb\xdc\xbd\x29\xd8\x55\x03\x71\xa0\xee\x99\xa0\xd4\x0c\xf6\x58\
+\xd7\x4c\xe1\xc8\x81\xa0\x74\x17\xf8\x73\xc7\x93\xc1\x5b\x6e\x06\
+\x3b\xab\x5f\x1b\x7c\xe4\x0e\x90\xd3\xda\x7d\x14\x6e\x7d\x27\xf8\
+\xd2\xca\xff\x01\x3f\x9e\xa1\xb0\xea\xab\x14\x6e\x7a\x2d\xf8\x72\
+\x29\xac\xab\xc1\xc5\xc1\xd7\xc7\x21\x4e\x94\x3c\x1d\x3c\xf5\xeb\
+\x9b\xe1\xb9\x42\x0a\xab\xce\xa3\xb0\xef\x2f\x41\xe2\x47\x95\x0f\
+\x96\xd5\x9d\x04\xfb\xef\x79\xbc\xec\x9c\x16\x88\x6b\x35\xe7\x97\
+\x9d\xfb\xe2\x0c\xac\x7b\x1b\x28\xdc\xf8\x44\xd9\xb9\xa7\x20\x1e\
+\x5d\xf6\x72\xd9\xba\x5e\xb0\x9b\x35\xdf\xa4\x70\x6b\x7d\xd9\x6d\
+\x1f\xd5\xc1\xcf\x16\x95\x7d\xfc\xf7\xc0\xdf\x9e\x23\x65\xff\xfc\
+\x62\x08\xe4\xf1\x4e\xd9\xa3\x07\x20\x8e\x95\xff\xb8\xec\xd1\x5f\
+\x80\x78\x77\xff\xbe\xec\x8d\x0f\xff\x1c\xe6\xfb\x78\x68\xe9\x20\
+\x8c\x77\xae\x1c\x5a\x5d\x0e\x7e\xb9\xa6\x84\xc2\xf0\xf2\x50\x57\
+\x33\xc4\x9f\xb1\xbb\x28\x8c\x7e\x3f\xd4\xa3\x1c\x06\xbb\x6b\x0b\
+\xf5\xa8\x18\xce\x84\xfa\xff\x29\x09\xeb\xac\x1a\x1a\x7b\x1c\x08\
+\x16\xfe\x2e\x64\xec\x85\x75\x6c\xc9\xc9\x50\xb2\xf0\xdb\xc0\xef\
+\x9d\xa1\x03\x9f\x5b\x00\x72\x9a\x09\x7d\xb2\x0b\xd6\xa9\x05\xd7\
+\x50\xb8\xbb\x2c\xf4\x8f\xdb\x81\xaf\xb9\x57\x86\x1e\x78\x0d\xe2\
+\xed\x65\x5b\x29\x5c\xff\x76\xe8\xe1\xa7\xc0\x2f\x97\x3c\x10\x7a\
+\xe2\x1d\x58\x37\xaf\xfc\x63\xe8\x85\x03\x9f\x86\x78\x1d\x0d\xfd\
+\xfc\x3b\x45\x90\x0f\xbc\x5e\x3e\xe7\xcf\x73\x21\xce\xbd\x42\x61\
+\xfb\x7e\x0a\x47\xbf\x51\x7e\xcb\xf0\x39\x60\x37\x95\x14\xee\x2c\
+\xa7\x70\xf7\xb7\xca\x0f\x3f\x07\x7a\x9a\x77\x7e\xf9\x7d\xaf\x40\
+\x3c\x6e\xb9\x83\xc2\xbe\x7f\x2b\x7f\xec\x59\xb0\xd7\x55\x02\x85\
+\x03\xd5\x15\xc5\x47\x81\xef\xe2\x69\x0a\x1b\xbb\x29\xdc\x79\x94\
+\xc2\xc8\x25\x14\x4a\x95\x15\x5d\x07\xe7\x81\x5e\x5e\xa9\xe8\xeb\
+\x1b\x81\xe7\x8f\x54\xa8\x5f\x86\x1c\xae\xec\xb9\x8a\x0f\xf4\xee\
+\x07\x7e\x8b\x2a\x0e\x5f\x07\xf9\xd9\xae\xf5\x15\x5f\x8e\x7c\x0b\
+\xe2\xd7\x87\x2b\x4b\x3e\x02\xf1\xe2\x82\xdf\x55\xae\xbf\x1d\xf8\
+\x28\x78\x83\xc2\xda\xbd\x14\x0e\x8e\x56\x0e\x3d\x06\x76\xbb\xb6\
+\x9a\xc2\xad\xb7\x54\xde\x11\x82\xf5\xe4\x92\x1b\x29\x1c\xae\xaf\
+\x3c\x84\xe1\xea\xcb\x29\x1c\x3c\x56\x79\xe8\x65\x18\x77\xcb\x92\
+\xca\xfb\x77\x80\x3d\xac\x3c\x45\x61\xef\x6f\x2a\xbf\xf7\x41\xb0\
+\xe7\xe6\x67\x28\xec\x7e\x7f\xe5\x2f\xe3\x7f\x07\xeb\xdf\x3d\x95\
+\xbf\x54\x40\xdf\x17\x6c\xa4\xf0\xa2\xa3\x95\x2f\xad\x04\xbf\x0d\
+\xbe\x51\xf9\xee\x57\xc0\x9f\xe7\xdf\x01\x8b\xeb\xf8\xb5\x20\x59\
+\xd4\x80\xba\x90\x8c\xc6\xe1\x47\x42\x1a\xfc\x51\xd0\x7e\x24\x22\
+\x01\x45\xe1\xd3\x08\x52\x91\x41\xa0\x88\xda\x02\x24\x0c\xc3\x9f\
+\xda\x2e\x39\x32\xa9\x1a\x72\x44\xe8\x92\xc7\xc7\x25\x4d\x52\x22\
+\x52\x5b\x09\xfe\xb6\x00\x13\xac\x46\xed\x40\x28\x0e\xa8\x8a\x49\
+\xc2\x42\x0d\xf4\x8a\x5a\x5c\x55\xe4\x88\xf5\xf8\x92\xac\xc7\x05\
+\x18\x2d\x06\x3f\x49\xf8\x64\x02\x7e\x37\x90\x9a\x26\x50\x9d\x22\
+\x20\x84\x0d\x4d\x32\x22\x93\x52\xd4\x22\x55\x97\x41\x4a\x06\xd4\
+\x5f\x31\xa3\x87\x52\xc8\xb2\x31\xc3\x30\x2c\xa0\x61\xf2\x68\x04\
+\x4d\x9a\xf3\x16\x50\x2f\x8c\x3e\x01\x3f\x32\x90\xd2\xd3\x04\xca\
+\x7b\x93\x13\x13\xb2\xa2\x0b\xc3\x32\x0c\xcd\x0e\xdc\x07\x34\xba\
+\x00\xaf\x9f\x60\x48\xc0\x35\xc8\x32\x8d\x17\xec\x1b\xee\x12\xfa\
+\x65\x45\x12\x35\x0b\x69\x7e\x1a\x09\x8b\x5b\x27\x42\x8e\x11\x74\
+\x6b\xba\x65\x18\x31\x6c\x48\x89\x04\x3b\x4f\x3f\x60\x8e\xa0\xc1\
+\xf4\x53\x45\x7d\x23\x83\xf6\x6f\x47\x51\x17\xf3\xed\x68\x97\xf5\
+\xed\x72\xc0\x4c\x12\x19\x61\x65\xd3\xb1\xc7\xe0\xff\x0a\x4c\x9c\
+\xf2\x61\x90\x6f\x0c\xf8\x11\xd3\x34\xaa\x06\x45\x4d\x53\xa7\xc7\
+\x44\x25\x2a\x0c\xaa\xb2\x2e\x59\x04\xe7\xc1\x60\x32\x4a\x10\xbd\
+\x69\x0c\x69\x4b\xec\x65\x04\x43\x18\x9d\x49\xb0\x66\x52\x81\x06\
+\xe1\x29\x1d\x7e\x92\xb6\x29\x17\x0f\xaa\x8a\xc4\x5a\x53\x98\xc8\
+\x24\x09\x0f\xaa\xf0\x5b\x94\x11\x6b\x20\x2c\x2b\x49\x5d\x95\x19\
+\xd1\x04\xd3\xdc\x58\xe3\xfb\x32\x46\x9e\x87\x3a\x09\x8f\x98\xcb\
+\x18\x4c\x7a\x3f\x60\x60\x93\xb1\x08\x97\x75\xaa\x9a\x26\xc5\x44\
+\x43\x56\x15\x8c\x57\x22\x46\xc6\x87\x63\xaa\x61\x9a\x0b\x76\x18\
+\xac\x2b\x15\x0c\x44\x4d\x9b\x0c\xe6\x32\x01\x7c\x1a\x96\xbd\xf5\
+\x29\x89\xa4\x01\x5e\x22\xc6\xd4\x89\x2c\x3a\x75\xa0\x09\x6c\x76\
+\xd8\x54\xa2\x84\x4e\x03\xcc\xb1\x31\x8d\x5d\xd2\x2f\x4e\x08\x0d\
+\x7a\x63\x16\x22\xe5\x3f\x96\x56\x61\x2c\x65\x73\x96\xbd\x61\x5b\
+\x13\x3a\xd5\x98\xaa\x65\x61\x2f\x00\x81\x26\x4c\xc9\xa7\x28\xf4\
+\xbb\x50\xd8\x26\x47\x8d\xc9\x2c\x0a\x0b\x79\x14\x58\xbd\x5b\x34\
+\xda\xb2\x88\x54\xa3\x1e\x13\x85\x5a\x1c\x8b\x58\xb2\x4d\x56\xa2\
+\xea\x74\x36\xd2\x42\x54\x0f\x2e\x9e\x80\x9f\x98\x19\x95\x04\x42\
+\x26\x46\x48\x58\x36\x54\x5e\xdf\x9e\x48\xc4\x66\x84\x1e\x39\x66\
+\x48\x44\x04\x73\x44\xf8\x40\x8e\x10\x8d\x52\xea\x26\x17\xf5\x68\
+\x00\x26\x11\x25\x21\x90\x90\xb4\xcc\xa6\xbe\x3b\x2a\x1b\x1c\xe4\
+\x20\x20\xd3\xd1\x25\x06\x09\xc6\x94\x38\x48\x15\x80\xb4\x91\x84\
+\x59\x1c\x6e\xad\xd1\x4a\xeb\x37\x4a\x8a\xa4\x89\x06\x0f\xb9\x0a\
+\x90\x87\x88\x6b\xca\x84\x84\x6c\x79\x0d\xa0\xf3\x78\x0d\x11\xc9\
+\xc9\xd8\x3c\x19\x39\xf9\xea\x7b\xa5\x58\xc2\x0d\xed\x6f\xf0\x1f\
+\xf3\x28\xd6\x02\x67\x84\x5a\x18\x61\x94\x28\x52\x07\x51\xaa\x24\
+\x10\x5b\xd3\x0b\xd4\x0f\x6b\x6a\x44\xd2\x75\x4f\x83\x15\x37\xbf\
+\x7f\xe5\xf5\x5c\x39\x8c\x12\x8f\xc5\x4e\xd3\x0e\x0a\x14\x2c\xd3\
+\x69\x1f\x10\x46\xcd\x00\xe2\x82\xbc\x92\xf8\xdd\x04\x88\xc2\xf2\
+\xbc\x04\x9a\x21\xc6\x9c\x34\xe3\xa0\x42\xfc\x1b\x7f\x06\x5a\x4a\
+\x13\x9f\xdb\x3e\xa6\x82\x3f\x27\x66\x74\x35\xa9\x44\x45\x45\x8c\
+\xcd\xe8\x5c\xf3\x5a\x0d\xdc\xd1\x55\x84\xae\x65\x38\x4c\xd0\x38\
+\x29\x83\x74\x92\xf0\xfb\x14\xf9\x0c\x82\x1a\x59\xae\xc6\x70\x44\
+\x4a\x0f\x37\xaf\x3d\x1a\x15\x54\x4d\xd0\x93\x63\x86\x26\x46\x0c\
+\x21\x2a\x45\xe4\x31\x29\xe6\x2a\x43\x12\x9c\x46\x89\x8e\x0d\x33\
+\x24\x09\xc4\xac\x63\xc4\x47\x1b\x50\x13\x13\x5e\xca\xdb\x63\x31\
+\xec\x20\x92\x2e\x34\x34\x35\x72\x49\xb6\x53\xb3\x21\x8b\x33\x2f\
+\x6c\x56\xb6\x27\x0d\x35\x62\x0f\x9d\x2e\x44\x17\x3b\x12\xc5\x01\
+\x15\x5b\x50\xdc\x66\x3b\x0c\x59\x75\x42\x13\xe3\x1c\xb2\x7e\xd4\
+\x81\x13\x07\xcb\x90\x3a\x62\x49\xbe\x43\x75\xc3\x0c\x0c\x73\xd0\
+\x31\x66\x2e\xc5\x1d\x2a\x0d\x7d\x2e\x98\xb7\xc1\x2a\x1b\x27\x0b\
+\x0d\x0e\x83\x58\x75\x29\x31\x47\x88\x54\x22\x24\x71\x91\x88\x25\
+\xd1\x10\xa9\x13\x85\x2b\x44\x29\xf4\x19\xac\x1c\xfc\xdd\x5e\xf8\
+\x86\x26\x5e\x52\x7a\x35\x89\x10\x8e\x12\xa6\x8c\xf1\xef\x12\xe1\
+\x34\xb5\xde\xb0\x09\x9b\xc1\x04\x82\x35\x9d\xa2\xa2\xa8\x86\x10\
+\x51\x15\xe0\x59\x52\xe0\x8f\x40\xcc\x55\x17\xa6\x65\x63\x52\x88\
+\x9a\x29\x9b\x21\xe8\x62\x1c\x26\xa6\x4c\x08\x38\xe8\x78\xf3\xcb\
+\x96\x14\x71\xf0\x02\x20\x21\x6b\x26\xed\xe5\x42\x22\x26\x89\xb0\
+\xc6\x27\xe1\x8f\x26\xc5\xd5\x29\x49\x18\x4b\x1a\x06\xd7\x04\xda\
+\x5c\x25\x28\xc2\xa7\xd8\x45\xa8\xdc\x96\xa2\x16\xf8\x7f\x1f\x04\
+\xbe\x6e\x62\x28\x2a\xe3\x91\x75\x26\x43\x6a\x42\x52\x84\xa5\x2d\
+\x42\xdf\x50\x37\xe4\x29\x3c\x97\xbc\x0d\xd2\x0e\x2a\xfb\x93\xc4\
+\xef\xb3\x47\xd7\x48\x02\xa1\x91\x55\x21\x69\x9a\xa6\x37\xed\x89\
+\x9e\xb5\x37\x45\x74\xa7\x33\x46\xde\x6c\xce\x24\x11\x13\x67\x78\
+\x0a\x93\xf8\xea\x82\x8f\x6f\x70\x95\xab\x4e\xa2\xda\xd4\x59\xb2\
+\xc8\xd4\x9c\x2c\x1f\x5a\x61\xce\x69\x5a\x93\xf9\x56\x98\x7b\x52\
+\x21\xc8\x79\x52\x61\xd9\x1a\xa0\xa4\x73\x12\x46\x90\x62\x1c\xc4\
+\x56\x48\x56\x22\xc0\xd9\x04\x49\x19\x04\x22\x0b\x36\x28\xa6\xb2\
+\x5e\x46\x32\x56\xa1\xd3\x39\xa9\xaa\x60\xd1\xe3\x10\x25\x05\x43\
+\xa5\xf3\xe0\x8c\x55\x07\x4c\xc6\x4c\xe9\x58\xd2\x65\xb2\xf9\xce\
+\x18\x2c\x4d\x42\x18\x0b\x82\x9b\x94\x74\x66\x86\x10\x36\x33\x4d\
+\xfb\x35\x87\xc4\xc2\x6c\x12\xac\xbe\xad\x72\x8a\x21\x47\xf9\xf2\
+\x16\x08\x8a\x3a\x93\xae\xb9\x80\xed\xc1\x52\x78\x90\x3f\x61\xdb\
+\xe3\x57\x74\x25\x35\xf2\x6d\x9b\x00\x19\x80\xa0\x4b\x91\xe6\x60\
+\xd0\x54\x32\x7c\xd4\x72\xbd\x10\x0c\x86\xc1\x62\x9a\x85\x1e\x4d\
+\xda\xdb\x0c\x1f\xb5\xe2\x8f\x3a\x64\x43\x87\xdf\x57\xf1\x72\x86\
+\x00\x84\x0f\x5c\x64\x31\x39\x53\xf7\x3e\x6e\x7e\x97\x8d\x51\x85\
+\x31\x04\xe6\x69\xee\xb2\xd9\x43\xca\xb4\x56\x52\x5f\x62\xa7\xc2\
+\xab\xfc\x38\x49\x7a\x65\x5b\xc8\x0e\xf5\xf4\x8d\xb4\x0a\xc3\x9a\
+\xa4\x4b\x06\xcf\x07\x2a\x98\xac\xa7\x07\x0d\x58\x5e\xd0\xc3\xcf\
+\x79\x6c\x12\xae\x4a\x17\xd0\x9d\x2a\xf6\xbc\x7d\xdc\x29\xcc\xbe\
+\x30\x76\x75\x91\xbc\x2a\x65\x17\x2a\xb3\x29\x9d\x5d\x33\x06\xe7\
+\x5a\x9a\xf3\xb8\x53\x71\xed\x2a\xc1\x59\xd7\x8a\xae\xc1\xa1\xdb\
+\x6c\xc9\x4c\x66\x55\xe9\xbe\x7e\x71\x8c\x1b\x0c\xab\xcc\x62\x5a\
+\x36\x8b\x2e\xa6\xea\xee\x97\xc6\x79\xbe\xd0\xc4\xe9\x12\xd1\x0a\
+\x74\x8a\x64\x70\x31\x86\x66\x55\xbf\x34\x25\xc5\x98\x26\x11\x87\
+\xfe\x3c\x12\xdf\xb5\x74\x55\x97\x1d\x3c\x83\xfd\xaa\x18\xcd\x19\
+\x3b\x17\x40\x35\x20\x92\x76\x81\x98\xce\x7a\x27\x61\xae\x71\xf8\
+\x1b\x93\xfb\x0e\x88\x4a\x52\x8c\x09\x0d\x93\x46\x3c\xc6\xcb\x7d\
+\xe7\x3b\x90\x4b\xc0\xa4\xc7\x19\x62\xa1\x14\xb1\x44\x74\xdc\x95\
+\x96\xbd\xbc\x19\x50\x15\x95\x5b\x4a\x85\xcd\xf5\xdb\x20\xc2\xc0\
+\xde\xf6\x27\x2b\xa4\x0e\xe0\xf4\xaa\x4b\x9d\xe6\x45\x9f\xea\x0c\
+\x12\x3a\x93\x14\x97\x10\x02\x5b\x5c\xeb\x3e\x84\x9b\x72\x61\xa2\
+\x4e\xc9\xca\xf2\x81\x08\x2e\x59\x62\xc4\xfa\x70\x01\x6e\xd9\x5d\
+\xf5\x40\x32\x66\xc8\x78\x19\x0f\x4b\x31\x29\xc2\x0b\x8c\xf6\x58\
+\xe4\xd4\x55\x72\x0d\x1c\x83\x66\xc1\x84\xbd\x08\x07\xc1\xb8\xad\
+\xc9\x54\x3a\x28\x4d\x0b\x8a\x18\xa7\x8d\x1e\xd7\xaa\x83\xed\x39\
+\x51\xb9\x64\x4c\xd3\x52\xeb\xa0\x9a\x7b\x3a\x8e\x34\xb3\x44\x67\
+\x25\xe7\x2c\x4d\xc1\xfb\x7f\xdc\xc4\x88\xe9\xe7\x59\x91\x20\x97\
+\x38\x73\x76\xdf\x5c\x0d\xa3\x8b\x44\x8f\x84\xe9\xad\xa9\x08\xcc\
+\x46\x15\xa6\xea\x1f\x82\x0a\x36\x47\x64\x11\x1c\x29\x46\xad\xc6\
+\x90\xa5\x62\x4c\x6d\x44\x9e\x98\xe4\x91\x1b\x26\x21\x4e\x20\xd1\
+\xf5\x77\x84\x35\xcb\x0d\x52\x59\x2f\x6d\x9e\x09\x64\xea\x4c\xa8\
+\x49\x37\x9e\x31\x03\x53\xe4\x29\x36\xba\x2e\x1d\x52\x62\x33\x02\
+\x4e\xe0\x48\x26\x2b\x44\x44\x45\x18\x93\x04\x5c\xec\x44\x05\x11\
+\xd2\x02\xc1\x90\xe3\x3c\xd9\x8d\x67\xb0\x16\x31\x8b\x4e\xd9\x81\
+\x35\x9a\xa6\xa6\xcc\x3c\x15\x67\xf3\x63\xf8\x22\x67\x86\x21\x14\
+\x83\x9b\x78\x63\x39\x53\x9a\x3c\x96\xf3\x63\xee\x42\xc2\x9c\x8d\
+\xb1\x08\xe4\x79\x13\x1e\x19\x8b\x02\x63\xa9\x81\xa3\xa4\x58\xb1\
+\x97\x33\x0e\x43\x33\xe5\x5e\x8a\x41\xea\x01\x92\x39\x95\x08\x91\
+\x36\xb5\x43\xd1\x96\xa1\x35\x12\x66\x8d\x69\x35\x55\xc4\xa4\x38\
+\x86\x14\x4a\xd4\x3c\xb2\x3c\x79\x96\x58\xb6\x67\xf9\x2c\xdb\x17\
+\xbb\xb2\x9d\x4e\xfa\xbd\xb1\x1e\x80\x20\xa3\xda\xca\xd5\xe2\x61\
+\x59\xb9\x8e\xbb\xfe\x8c\xd8\xca\x68\x5b\xde\x3d\x0c\x35\x2e\x07\
+\x17\x37\x48\xb1\x06\xc6\xd3\xfb\x41\x2a\xb3\x3d\x41\x05\xc1\xc6\
+\x85\x72\xdc\x99\x14\xb6\x89\x53\xd2\xb8\xaa\xf1\xba\x43\xb5\x66\
+\x22\xce\x26\x31\x4c\xd3\x1f\x32\x70\x33\x51\xf1\x56\x04\xcd\x1d\
+\x9e\x31\x26\x21\x8e\x93\x9c\x44\x68\xcf\xdd\x0e\x0c\x9a\x62\xd4\
+\x99\x80\x5b\x34\xc2\x4d\x4f\x2b\x88\x1c\xd3\xbd\xc2\x34\x9a\x7f\
+\x84\x74\x59\xb8\xa9\x8b\x0d\x13\x64\x67\xa4\x3a\x83\x56\x4e\x45\
+\xa9\x08\xed\x31\x7e\xd6\x38\x42\x73\x6b\xa0\x26\xdb\xaa\x51\xe0\
+\x02\xc7\x12\x6e\x07\xb4\x93\x09\x19\xb8\x6e\xa1\xed\x85\x66\xf8\
+\xbd\xd3\xad\xa1\x60\xad\x1f\x23\x12\xed\x0f\x70\x17\xc0\xae\xf4\
+\x5a\xc1\x74\xb6\xb9\xeb\x84\x3d\x0b\x19\x51\xc1\x7c\x06\x24\xf0\
+\x8d\xf0\xde\x24\xb8\x73\x8e\xcc\x2c\xd5\x29\x48\x05\x0c\xa6\x1d\
+\x11\x16\xb1\x30\xf9\x35\x5c\xd8\xac\x56\xec\x75\x8f\x2f\x1c\x11\
+\xb9\xd3\x5c\x62\x47\x4c\x2f\x11\xce\xa9\x77\x19\x21\x27\x90\x04\
+\x9c\xdb\x26\xc8\xcc\x55\x44\x67\x3b\xa1\x49\x4b\x4e\x3b\x09\x9b\
+\x6d\x15\x85\xd2\x63\x04\x23\xc7\x72\x14\x00\x9e\xf7\xf9\x5c\xcd\
+\x9d\x6e\x4a\x19\xd4\x10\x1c\x1b\xc9\x65\xe1\x04\xcc\x42\xcb\xd5\
+\x44\xae\xb0\x93\x62\xd8\x20\xe8\x49\x57\x5c\x9b\x59\x2d\x0f\x27\
+\x13\x09\x55\xc3\x21\x96\x06\x88\x54\xaf\xbd\x79\x5a\x9c\x6a\xbc\
+\xfc\x72\x4f\xed\x77\x1b\xc5\x9a\xad\x62\x2c\x09\xcf\xe3\x3d\x08\
+\x75\x5c\xd0\xf0\x6a\xc9\x8d\x36\x5b\x89\x52\xd9\x4c\xdd\xbf\x55\
+\x56\x63\x39\x36\x8a\xda\xc1\x9e\xa6\x48\x4a\xc6\x28\x70\x9b\xa8\
+\x29\xb2\xc2\x2b\x4c\xeb\xd0\x10\x37\x4a\x07\x3c\x04\xe8\x10\xea\
+\x20\x71\x02\x2f\x69\x8c\x2f\x6f\x9b\xe4\xf7\xdd\x6a\xc9\xa2\xad\
+\x93\x2e\x5e\x7a\x2f\xdb\x1a\x18\xd7\x17\x09\xd1\x7d\xeb\x89\x50\
+\xa0\x6b\x42\xdc\x9d\x82\x6e\xa8\xbc\x8a\xa9\x9a\xe1\x41\x24\xab\
+\x37\x63\x38\x93\x10\x8c\x72\x72\x60\x9f\x83\x7d\x95\x28\x89\xa9\
+\xd3\x3c\x02\xf6\xf2\x52\xe1\xe7\xf0\x23\xfc\xed\x2e\xd0\xdf\xc5\
+\xa4\x8a\x61\xdb\xa6\x99\x0d\xd3\x08\x53\xad\xb3\x71\x6c\x69\xc6\
+\xe6\x98\x70\xb1\x90\xd1\x44\x8d\x41\x19\xef\x69\x1a\x0b\x71\x07\
+\x50\xd6\x85\x20\xe9\xfb\xe1\x46\x5f\xb4\x43\x30\x20\x47\xc4\x9f\
+\xb8\xb7\xfa\x6c\x34\xe6\x9b\x34\x32\x29\x78\xc5\xaf\xc4\xf8\x18\
+\xd9\xec\x34\x72\xa4\xda\x90\xb5\x33\x1d\x33\x8b\x66\x76\x7b\x79\
+\x92\x91\x55\x39\xdd\xa4\xee\x24\x69\x2f\x51\x6d\x08\x93\x9e\x31\
+\x3f\x20\x54\x63\xb0\x4a\xca\x8c\x47\x39\xd0\x33\xeb\x04\xc5\xd6\
+\xc6\xc6\xe9\x60\x33\xd9\xba\x63\x79\x4a\x9d\x17\x70\xe4\x0b\x5d\
+\x61\xe5\xbb\xa3\x93\x90\x08\x09\xb0\x16\x0a\x49\x45\x17\x71\x81\
+\x43\x93\x73\xbd\x59\xb0\x31\x7d\x85\x33\xd7\x0b\x3c\xed\xd2\x87\
+\x32\x37\xe9\xeb\x08\x21\xdc\x0d\x35\x9b\xa1\xb4\x1b\x66\x06\xe5\
+\x4e\x73\xc3\x10\x37\xa1\x98\x13\x45\x9d\x49\x43\x1d\x1f\x6f\x13\
+\xb8\x04\xec\x86\xd5\x0d\xd1\x78\x14\xc2\xa7\x2e\x93\x3a\xbc\x03\
+\xf7\x1f\xd6\x0b\x94\x90\xd0\x94\x8b\x93\x05\x10\xe8\x34\x22\x3a\
+\xda\x15\x19\xb7\xa6\xc6\xf0\x55\x41\xa7\x25\x0c\x69\x51\x49\xcb\
+\xc1\x1d\x59\x89\xad\x53\x34\x51\xc6\xe3\x32\xc9\x96\x9b\x64\xc9\
+\x91\x96\x9c\x54\x17\xdb\x84\x46\xcb\x8d\x04\xf1\x71\x39\xeb\x94\
+\x4e\x65\x2f\x04\x29\xa0\xec\x49\x9e\x0e\xb4\xb1\x38\xc6\x5d\x68\
+\x57\xf4\xab\xd3\x79\x90\xde\x84\xfa\x48\x4d\x44\x93\x12\xfb\xf9\
+\xa4\xa8\x99\xca\x6a\xe4\x33\x3d\xfd\x14\xd5\xc5\x7a\x92\x56\x5a\
+\x6c\x35\xa5\x59\x10\xc2\x86\xa8\x19\xa7\xa1\xf6\x3c\x16\x19\x3e\
+\x19\xcf\x2b\x0d\x8f\x8c\xe7\xe5\x26\x9f\x29\xb9\xaf\x39\x3c\x2a\
+\xb4\x47\x9a\x20\xb4\x68\x4e\x4c\x8f\x26\xc9\x8c\x01\x04\xc9\x59\
+\x24\x61\x40\x4c\x90\xf6\x5c\x8d\x68\xdf\xd1\x4f\x1f\xf0\xa9\x27\
+\x35\xf2\x14\xd1\x6e\xc2\xac\x7d\xed\x1a\x6e\x40\x4b\x99\xde\x6b\
+\xd9\xd0\x94\xa4\xc5\xc4\x84\xd0\xb0\xb4\x31\x07\xe1\x2e\xb2\x99\
+\x2b\x9a\x65\x75\xe6\xe1\xa3\xcc\xc3\x57\x73\x68\x64\x87\x0c\x5a\
+\x99\x30\x26\x53\xc7\xb0\x5c\xc9\x7b\x3d\xcd\xe4\x4a\x60\x7e\x46\
+\x9d\x14\x71\xd8\xed\xac\xa0\x21\x56\x60\x36\x3d\x6b\x68\x58\x36\
+\x3f\xc9\x08\x97\x69\x0a\x6c\x9b\x34\xbd\x99\xc6\x45\xf7\xb0\x51\
+\xe0\x8a\x9b\xab\x20\x73\x45\xcc\x6b\xdf\x93\xe9\x61\x30\x24\x04\
+\x12\x39\x0c\xe2\x61\x53\x66\x47\x85\x9e\xac\x8b\x63\xf5\xb2\x67\
+\x41\xbb\x24\xbc\xd3\xde\x10\xd7\x1b\xa9\x2c\x5c\x28\xd6\x67\x05\
+\x66\xd9\x61\x84\x2c\xba\x56\x7c\x76\xa1\xeb\x65\x2b\xc6\x19\x73\
+\x81\x4d\xb5\x02\x49\xe3\x0c\xba\x9b\xc4\xf0\x51\x35\x94\x34\xf0\
+\x86\x92\x4d\xdf\x2e\x14\x73\x96\xd0\xee\x53\xb0\x9a\x7d\x2d\xac\
+\x95\xd1\x8a\xa7\x25\xa7\x04\x2c\xf4\xd6\x6c\xf4\x56\x2e\x7a\x1d\
+\x39\xc8\x41\xbb\xa3\x16\x21\x66\xa5\xa4\x44\xc8\x96\x18\x97\xd0\
+\x42\xb3\xb2\xb6\x9c\x4f\x76\xdc\x2b\x2f\x0b\x4f\x43\xa0\x61\x36\
+\xc9\x9d\xc9\xad\x43\xfd\x24\xd3\x9a\x20\x39\xd5\x7e\xdb\x3e\x19\
+\xbb\x90\x35\x90\xfc\x9a\x9a\x92\x4e\x3a\x35\x32\x1b\x7f\xf0\xea\
+\x34\x8d\x8f\x4e\x0a\x0d\x9d\x92\x62\xd0\xf8\xe3\x8f\x5a\xe3\x34\
+\x7b\x1e\xa7\x17\xbe\xb3\x28\x57\x30\x94\x7b\xf7\x67\x91\xbd\x94\
+\x6c\xcc\xa6\x3b\x0a\x4c\x5b\x94\x46\x60\xca\x30\x26\x1b\x85\x62\
+\x0d\x8b\x7e\x18\x30\x2c\xf2\xf3\xf0\xb6\x32\xd4\x1f\x8a\x41\xbb\
+\x0f\x42\x03\xe4\xdc\xe1\xe1\xfe\xac\x81\xce\xe0\xb9\x73\x96\x6c\
+\x5d\x46\xa0\x37\x3d\xdf\x32\x8b\xd4\x09\x03\xe2\xfa\x99\xd8\xd5\
+\x24\xb7\xc3\x87\xf1\x70\x4a\x2c\xdb\x0c\xaa\xb8\x5b\xd4\xb2\x86\
+\xab\x80\xc0\xbf\xd2\x41\xca\x25\x3d\x2b\x1d\xc5\xbb\x20\xdd\x01\
+\x63\x0f\x0d\x65\xe9\x08\x9f\x6e\x48\xc2\xfc\x66\x1c\x89\x04\xd0\
+\x46\x40\x83\xe8\x61\xf1\xb6\x51\x94\x95\xcc\xc7\x5a\xb3\x54\x29\
+\x66\x9d\xb4\x77\x53\xe3\x39\xe9\x63\x02\x7c\x2d\x6e\x70\x09\xb8\
+\x4e\x23\xf1\xec\x7d\x9e\x75\xae\x3f\x21\x46\xf0\xa9\x34\x17\xb3\
+\xcf\xfb\x8c\x3f\x8b\xbc\xd2\x51\xfa\xd9\x59\x71\xb6\x46\x48\x76\
+\x4c\x0f\x9d\x38\xaa\x24\xf3\x16\x83\x23\x5d\xe6\xb8\x04\xa6\xc6\
+\xde\x85\xb0\xdb\x48\x98\x24\xb0\x09\x2e\x8d\x52\x42\x23\x6c\xe6\
+\x8a\x76\xfc\xd4\xe9\x88\x06\xe2\x08\x51\xb3\xa7\x62\xd8\x24\x5e\
+\x8e\xcf\x47\x34\x68\x22\x20\x2a\x4e\x8e\x60\x2d\x7b\xe4\x80\x04\
+\x1b\x9e\xfb\x46\x06\xad\xd3\xfc\x2c\xd6\x7c\x7a\x3a\xc2\x74\x3b\
+\x2c\x07\x8d\x50\xb0\x39\x60\xdf\x28\x8c\x1b\x97\x23\x9a\x2a\x64\
+\x8f\x5b\x0b\x14\xa8\x35\x59\x07\x4c\x99\x3e\x64\x9f\x21\x51\xef\
+\xd5\xbd\xa9\x36\xbb\x28\x71\x70\x36\x28\x4e\xf2\xd4\x6c\x16\x59\
+\xcb\xfc\x30\x31\x2f\x8a\x75\x27\x11\xc0\x24\x9c\xf4\x3a\xe2\x21\
+\x34\x67\x46\x7f\xdb\x75\x0e\x8e\xbf\x2f\xa1\x5b\xf1\xb4\x28\xf2\
+\x1a\xc2\x3b\x32\xee\x92\xb4\x20\xe7\x33\x91\x5e\x1c\x6c\xee\xa0\
+\xda\x2c\xb4\x08\x39\xdc\xcc\xeb\x88\x5e\xf4\x5e\x4b\x47\xe4\x6b\
+\x3f\x3b\x86\x6a\x59\x0c\xb8\xc6\x50\x3a\x40\xb8\xf9\xbd\x16\x63\
+\x6b\xbe\x62\x6c\x3d\x5d\x31\xb6\x9e\xa6\x18\x5b\x73\x89\xb1\x35\
+\xb7\x18\xf3\xbf\x88\x64\x77\xf3\x11\x94\x71\xae\x9d\x69\xc5\x88\
+\xa4\x35\x6a\x51\xaa\x19\x9e\x14\xc9\x51\x67\x7a\xd0\x5d\x9f\x94\
+\x13\x59\x14\x83\x10\x91\x32\xf1\xfc\x04\x2f\xeb\xd1\x5a\x18\x5c\
+\x34\xf7\x9e\x69\x25\x1a\x67\x04\x50\x3a\x22\xc6\x13\x8e\xe9\xca\
+\x72\xd7\x72\x87\xb7\xd6\x56\xe6\x58\x62\x57\x67\x29\x4b\x67\xf6\
+\x43\xac\x83\x50\x2e\xea\x4a\xed\x92\xe4\x50\x17\xee\x4d\xb2\xb7\
+\xfc\xd8\xe3\xc4\x19\x45\xbe\x79\xd5\x2f\x55\xe4\xdb\x85\xcc\xbb\
+\xef\xc5\x3e\xe9\x7a\x35\xa0\x66\xc2\xbc\x78\x43\xac\xc3\x56\xa0\
+\xe4\xbc\x1c\xe0\x8a\x3b\xcf\x39\x0d\x65\x7b\x62\xb6\x44\xb4\x8d\
+\x4b\x8d\x97\x96\xfa\x70\x5a\x2a\x70\xd1\xe7\xb3\x37\x8e\xec\xde\
+\x61\xb1\x93\xba\x7e\x64\x9d\xc4\xe2\x08\x26\x77\x77\xc0\x0d\x37\
+\xd7\x79\x25\x57\xc4\xec\x0e\xa9\xb3\x93\x87\x18\x27\xe7\x8b\x85\
+\x73\xaa\xc1\x15\xa7\x2e\xed\xa9\x92\xa3\x56\xcb\xb0\xaf\xea\x1e\
+\x54\xca\x3b\x0b\xc0\x11\x5e\x8e\xd6\x8a\x1b\xe2\x6a\xc7\xec\x28\
+\xc7\xb9\x7e\xa6\x94\x4e\x5d\x15\x19\x31\xdb\x2f\x1c\xf9\xe4\x5b\
+\x95\xbb\x92\x6a\xce\x23\x0c\xb1\x2a\xa8\xcd\x0e\x40\x39\x75\xc1\
+\xdd\x29\xe5\xa8\x83\xbf\x5d\xc9\xf1\x67\xcd\xdc\x9f\x31\x57\x53\
+\xb6\x55\xaa\x49\x74\x0d\xcd\x21\x1e\x0f\xd1\xa9\x2e\x85\x9b\xda\
+\x3f\x3f\xdd\x00\xc5\x23\xe8\x2d\x46\xf1\x28\x2c\xe4\xd5\xc6\xec\
+\x4e\x85\xbd\x3a\xce\xc9\x99\x90\x11\xfe\x74\xd7\x83\x06\x73\xd2\
+\x41\x90\x3d\x71\xc0\xa3\x5d\x05\x2b\x70\xbf\x59\xf1\x10\x43\xb4\
+\xd2\xf8\xbe\xfe\x2e\x62\x7b\x5e\x48\xa4\x8a\xa6\xa4\xad\x54\x0a\
+\x90\x52\x29\xa9\x7b\x20\x91\x33\x20\xf3\x6d\x21\xd3\xd3\x32\x27\
+\x53\x96\xe1\x4a\x7c\x71\xa7\xf2\x1e\xc7\x02\x94\xed\x51\xd2\x2c\
+\x2a\x5d\x84\xe6\x24\x9d\x6f\xf4\xe5\xdb\x2b\x4e\xf8\x6c\xdd\x27\
+\x26\xe3\x92\x98\x23\xeb\x3c\x2a\xb9\x22\x32\x0f\xf7\x4c\x07\x65\
+\xfe\x6c\x3d\x1e\xaf\xe1\x8b\x3f\xdf\xe0\xce\x77\xf7\x30\xa1\x16\
+\x27\xd3\xa6\x3b\x46\xf4\x5e\x89\x7d\xdb\x23\x84\xaf\xc1\x0e\x69\
+\xf2\x84\xac\x88\x31\x5b\x48\x24\xc3\xd9\xec\x98\xa5\x98\x34\xef\
+\xf8\xb2\xb4\x02\x98\x56\xd8\x3c\xb2\xe6\x4a\xa7\x9a\xa4\xa6\x34\
+\xad\xa6\x67\x2a\x99\x8d\x88\x76\xbc\xff\xaa\x40\x60\xa4\xa7\x61\
+\x5c\x89\x9c\xcd\x3e\xb0\xeb\xa0\x67\xb0\x29\xec\x3a\x46\x3e\x69\
+\x71\x26\xee\x59\xed\x2e\xbb\x8e\xea\x27\x1b\x4b\xd6\x6d\x25\x7f\
+\xa7\xaa\xcb\x0a\xdf\x06\xce\x60\x7b\xda\x75\x8c\xfc\x7b\xd5\x1c\
+\x93\xf5\xd0\xb8\x76\xc5\xf6\xd2\xc5\x76\x45\x9e\x75\x4b\xdb\x95\
+\x22\xa7\xbf\xcd\xf1\xfd\xcc\x45\x3e\xf3\x02\x91\x55\xe1\xa4\x2f\
+\x11\x71\x23\x80\xa7\x77\xd8\xb8\x52\x38\x5b\xcd\x77\xd7\x01\xdf\
+\x93\x4e\xbc\xeb\xe8\x67\xe4\x2d\x3e\x1c\x47\xc9\xb3\xe9\xef\x4a\
+\xe9\xcc\xee\x00\x78\x16\x47\xbe\xdb\x01\x1c\x67\xcb\x7f\x6f\xc0\
+\x95\xd8\xe9\xdc\xef\xe4\x70\x38\xbb\xdd\x07\x8e\xf2\xf3\xba\x32\
+\xea\x4a\x67\x36\x97\x46\x39\x4b\x8a\xf3\xb5\x51\x4e\x44\xf1\xba\
+\xa1\xc2\x1d\xd3\xe9\xee\x29\x77\xc6\xf9\x6f\xc7\xb8\x92\xcb\x6b\
+\x6f\x86\x93\x3e\x78\x6f\x1e\x79\xf3\xde\x59\x6e\xf2\xe4\xe5\xbc\
+\x79\xec\xf8\x78\xf2\x5d\x8f\xdb\x3f\xae\xb4\xfe\x5f\xec\x05\xb9\
+\x72\x77\x06\x5f\x32\xe6\x3a\xc6\x7b\xb3\xf9\x74\xda\xc3\x9f\xd6\
+\x4e\x54\x1e\xd9\xc5\x99\xd9\x96\x7a\xef\xa4\xed\xb8\x47\xe5\x79\
+\xf8\xb3\xb2\x61\x35\x6b\x69\xcf\x76\xf7\xca\x75\xc0\x20\x29\xb4\
+\xf1\x2d\x14\x2b\xbe\xfa\x06\xd5\x70\x42\xce\x91\x03\xe7\xbb\x03\
+\xc6\xa9\x08\x72\xdc\x0f\xe6\xf2\x8e\xfb\x16\x61\xb6\x1f\x32\x98\
+\x90\xc3\x6a\x8e\xa0\x3b\xeb\x8b\xc5\x9c\xfc\x66\x76\x57\x8b\x39\
+\x4c\x9e\x89\x4d\x42\x8e\xe8\xb8\x3b\x86\x9c\x7a\x29\xf7\x46\x46\
+\xf6\x62\xee\x7d\xcb\x91\x63\x70\x23\x66\x54\xa7\x77\x03\x69\xc3\
+\xc1\xb0\xdd\x10\x84\x68\xae\xc6\xb9\x54\x3c\xef\x6a\x64\x22\x9e\
+\xb5\x5d\x8d\xec\xe4\x2d\x4c\x92\x64\x9c\x3e\xd1\xf7\xb8\x58\xaf\
+\xa0\x2a\x0d\x47\x26\x35\x55\x8a\x4a\xfc\xec\xd3\x4f\xd3\x1e\x4b\
+\x43\xe1\x5c\x1d\x08\xcf\x2d\x3b\x4e\xe6\x3c\xeb\xcd\x98\xec\x15\
+\xfd\x4c\xed\x34\x73\xb4\x79\xb6\xb6\x9d\x39\x01\x62\xb6\x7b\xd0\
+\x1c\x1f\xe6\x6d\x48\x73\x7c\xc0\xe3\x56\x52\x76\x8e\x6f\x7f\x19\
+\x28\x7d\xf9\x22\x71\x49\x2b\xb1\xea\x10\x23\xd7\x4d\x68\x44\xd9\
+\xe9\x97\x82\xce\x49\x58\xd7\x9d\x19\x7a\x8b\x33\xe8\xd1\x83\xe8\
+\x2a\x51\x7a\x84\x94\xde\xcc\x05\x9e\x4e\x51\x99\x12\xf5\x9c\x34\
+\xdd\x6e\x08\xb0\x71\x2e\xe3\x86\x80\x0b\xa5\x2a\xc2\x5d\x3c\x1d\
+\x74\xd8\x7b\x40\x6a\x3c\x0e\xb1\x86\x87\xbd\x16\xfc\xc1\x1e\xba\
+\x1b\x08\x8c\x98\x4b\x9d\x6c\x26\xc6\x1a\x51\x05\xbd\x05\xa9\xda\
+\x36\x18\xce\xeb\x04\x21\x1a\xda\x0c\x94\xae\xd2\xde\xa4\xac\x49\
+\x3a\x84\x77\x1d\xdf\x2c\x69\xe4\x0d\x8c\x17\xb7\x61\xf0\x20\x7a\
+\xb3\x4e\x23\x8b\x92\x4a\xec\xce\x62\xc6\x1a\x64\x4e\xd7\x70\x9f\
+\x70\xb1\x30\x22\xe9\x6a\x2c\x49\x5e\x86\xc5\x21\x5d\x41\x2e\xcb\
+\xcb\xe6\x45\x3d\x66\x05\xd8\xa8\x99\xf7\x65\x9d\xf1\x2e\x35\xab\
+\x69\xda\x23\xcf\x5f\x12\x0b\xfa\x45\x65\x22\x29\x4e\x48\x79\x8a\
+\x22\xef\x97\xd7\xba\xd2\xc9\x8c\x16\xd8\xc6\xf6\xb1\x16\x35\x20\
+\xee\xa3\xc1\x80\xc7\x4f\x53\x86\x45\x65\xbe\xff\xcf\x49\x41\xe5\
+\xf8\x05\x06\x82\x07\x83\xab\xb2\xbd\xc9\xa0\x9e\xbd\xbf\x8f\x6f\
+\x7e\xd4\xeb\x5c\x5c\x7c\x37\x7b\xc2\xdc\x0e\xa9\xb7\x5d\x33\x97\
+\x27\x14\xb1\x3e\xc6\x41\x0e\xa5\xe3\x7d\x3d\xe3\xaf\x7e\x1c\x3c\
+\xea\x79\x56\xe1\xe1\xf6\xaf\x33\xe2\x06\xb4\x8d\x18\x8a\x60\xbe\
+\x30\x49\x04\xce\xe9\x5d\xd2\x06\x44\xef\x89\xe2\xae\x34\x5d\x3b\
+\x79\x66\x15\xda\x26\x4e\x41\x10\x50\xc0\xb0\x34\x9e\x64\xbd\x5e\
+\xb8\x71\x41\x5f\x60\x16\x29\xba\x99\x1d\xc4\x98\xe4\x85\x91\x57\
+\x24\xa9\x1b\x34\x79\x71\xb5\x1e\xba\x18\xa6\xac\x39\x4a\x32\x0e\
+\xeb\x42\xe6\x94\x49\x9b\x8d\xc6\x35\xd1\x84\x2c\x4c\xe1\xab\xdc\
+\x02\x7e\x39\x22\xfc\xc6\x75\xd4\x56\x97\x21\xe8\xcd\xc0\x84\x99\
+\xee\x27\x88\x8c\xcd\xd0\xea\x34\x94\xa1\xaa\x82\x1e\x17\x63\x3c\
+\xab\x59\x97\x7e\xc7\x92\xe8\x52\x5f\xb9\xbf\x03\x92\x49\x7b\xf1\
+\x9b\x98\x6c\xb9\x15\xcd\x2d\x2a\x34\xf3\x65\x0e\xcc\x88\xc3\xb3\
+\xc9\xe0\xcc\x35\x44\x43\xa9\xb7\x9f\x82\x6f\x22\xfc\x9e\xd0\x7e\
+\xd4\x62\x45\x6a\xcc\x85\xed\x15\xa7\x76\x11\x38\x71\x53\x4b\x5e\
+\x74\x91\x31\xae\xb5\xc2\xb0\x2f\xa3\x70\x42\x6f\x23\xd9\xc4\x84\
+\xb9\x95\x69\x90\xf2\xcb\x3a\xab\x94\x45\xd8\x51\x78\x75\xe6\x20\
+\x98\xe9\xf6\xd8\x84\xaa\xc9\xc6\x64\xdc\x5d\x7e\xb9\xfd\xd5\x09\
+\x6b\x89\xe3\x65\x53\x85\x54\x1e\xd9\xee\x54\x6e\x5e\x85\xb3\x4e\
+\x54\x65\xd1\xb4\x5d\xaf\xf5\xd3\xb7\x31\xe2\x07\x2b\xf1\xdd\xe1\
+\xec\xd2\xd2\xcb\xd5\x34\x47\xd4\xf9\x60\x2e\xe6\x9b\xa5\x4d\x43\
+\x48\xdd\x4b\xb7\xdf\x90\x95\x84\x1e\x55\x8b\x8b\x86\x1b\x29\xe7\
+\xb7\xb1\x39\x0e\xd9\x86\x86\x40\x52\xe9\x76\x27\xb2\x5f\xb2\x16\
+\xcd\x5e\xb9\x6a\xd6\x95\x31\xc7\x9d\xa7\x6a\xf2\x5e\x10\x9a\x6c\
+\x0f\x25\xd2\x2d\xd2\x1c\x7c\xf9\xc3\x06\xb8\xa8\x3b\x67\xb3\xb8\
+\x77\x59\xa9\x5b\x2f\xc0\x60\xee\x2e\x8e\x02\xe7\x71\xd3\x1e\xec\
+\xd7\x20\x03\xfd\xea\x84\x20\xee\x93\x75\x57\xec\xd3\xbd\xb1\xe9\
+\x48\x74\x1e\x04\x06\xd5\xbc\x03\xc8\x86\x84\x56\x6b\x62\xc3\xe4\
+\x46\xb1\x3a\x2e\xb4\x72\x58\x3b\x13\x77\x3e\x5d\x64\xe6\x6d\xf9\
+\x71\x44\x3e\x8d\x97\x42\x86\x74\xb3\xca\x99\xfd\x3f\x06\x90\x4d\
+\x62\x56\xff\x22\x40\x36\x99\xd9\xfe\xb3\x00\xd9\x94\xaa\x00\x0f\
+\x8b\x46\x40\xf4\x4e\xb2\xe4\x6c\x8f\x4e\xc2\xc8\xd3\x6e\xb2\x49\
+\x78\xd5\x6c\x36\xe6\xe9\xa8\x75\xda\x7c\x37\xca\x69\xa8\x35\x8b\
+\xc4\xec\xd4\x9a\x45\x66\xd6\x6a\xb5\x51\xba\x19\x3e\x29\x2c\x28\
+\xf8\x3f\x74\xd8\xd5\xe4\
 \x00\x00\x00\xeb\
 \x3c\
 \xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\xa7\
 \x00\x00\x00\x05\x66\x72\x5f\x46\x52\x42\x00\x00\x00\x18\x00\x04\
 \xcf\x04\x00\x00\x00\x70\x00\x2a\xd0\x25\x00\x00\x00\x00\x00\x2a\
 \xec\x30\x00\x00\x00\x3b\x69\x00\x00\x00\xa8\x03\x00\x00\x00\x10\
 \x00\x26\x00\x46\x00\x69\x00\x63\x00\x68\x00\x69\x00\x65\x00\x72\
@@ -1585,113 +1603,116 @@
 \x69\x00\x64\x00\x65\x08\x00\x00\x00\x00\x06\x00\x00\x00\x05\x26\
 \x48\x65\x6c\x70\x07\x00\x00\x00\x11\x61\x70\x70\x6c\x69\x63\x61\
 \x74\x69\x6f\x6e\x57\x69\x6e\x64\x6f\x77\x01\x03\x00\x00\x00\x0e\
 \x00\x51\x00\x75\x00\x69\x00\x74\x00\x74\x00\x65\x00\x72\x08\x00\
 \x00\x00\x00\x06\x00\x00\x00\x04\x45\x78\x69\x74\x07\x00\x00\x00\
 \x11\x61\x70\x70\x6c\x69\x63\x61\x74\x69\x6f\x6e\x57\x69\x6e\x64\
 \x6f\x77\x01\x88\x00\x00\x00\x02\x03\x01\
-\x00\x00\x00\x10\
-\x3c\
-\xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\
 \x00\x00\x00\x2c\
 \x3c\
 \xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\xa7\
 \x00\x00\x00\x05\x72\x75\x5f\x52\x55\x88\x00\x00\x00\x0d\x11\x01\
 \xfd\x29\x0b\xff\x14\x02\x04\xfd\x2c\x0a\x13\
+\x00\x00\x00\x10\
+\x3c\
+\xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\
+\x00\x00\x00\x10\
+\x3c\
+\xb8\x64\x18\xca\xef\x9c\x95\xcd\x21\x1c\xbf\x60\xa1\xbd\xdd\
 "
 
 qt_resource_name = b"\
-\x00\x22\
-\x00\x30\xb0\xe7\
-\x00\x6a\
-\x00\x6f\x00\x68\x00\x6e\x00\x6e\x00\x79\x00\x5f\x00\x61\x00\x75\x00\x74\x00\x6f\x00\x6d\x00\x61\x00\x74\x00\x69\x00\x63\x00\x5f\
-\x00\x63\x00\x72\x00\x61\x00\x73\x00\x68\x00\x69\x00\x6e\x00\x67\x00\x5f\x00\x77\x00\x61\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\
-\x00\x67\
 \x00\x08\
 \x0f\x07\x57\x47\
 \x00\x65\
 \x00\x78\x00\x69\x00\x74\x00\x2e\x00\x73\x00\x76\x00\x67\
 \x00\x0c\
 \x0d\xfc\x11\x13\
 \x00\x74\
 \x00\x72\x00\x61\x00\x6e\x00\x73\x00\x6c\x00\x61\x00\x74\x00\x69\x00\x6f\x00\x6e\x00\x73\
+\x00\x22\
+\x00\x30\xb0\xe7\
+\x00\x6a\
+\x00\x6f\x00\x68\x00\x6e\x00\x6e\x00\x79\x00\x5f\x00\x61\x00\x75\x00\x74\x00\x6f\x00\x6d\x00\x61\x00\x74\x00\x69\x00\x63\x00\x5f\
+\x00\x63\x00\x72\x00\x61\x00\x73\x00\x68\x00\x69\x00\x6e\x00\x67\x00\x5f\x00\x77\x00\x61\x00\x76\x00\x65\x00\x2e\x00\x73\x00\x76\
+\x00\x67\
 \x00\x15\
 \x09\xe6\xdc\xbd\
 \x00\x70\
 \x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x65\
 \x00\x73\x00\x2e\x00\x71\x00\x6d\
 \x00\x18\
 \x0f\xa6\x69\x3d\
 \x00\x70\
 \x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x65\
 \x00\x6e\x00\x5f\x00\x47\x00\x42\x00\x2e\x00\x71\x00\x6d\
 \x00\x15\
-\x09\xe1\x0c\xbd\
-\x00\x70\
-\x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x65\
-\x00\x6c\x00\x2e\x00\x71\x00\x6d\
-\x00\x15\
 \x0a\x1a\x8c\xbd\
 \x00\x70\
 \x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x69\
 \x00\x74\x00\x2e\x00\x71\x00\x6d\
 \x00\x15\
 \x09\xe7\xac\xbd\
 \x00\x70\
 \x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x66\
 \x00\x72\x00\x2e\x00\x71\x00\x6d\
 \x00\x15\
-\x09\xe0\xbc\xbd\
-\x00\x70\
-\x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x64\
-\x00\x65\x00\x2e\x00\x71\x00\x6d\
-\x00\x15\
 \x09\xd3\xbc\xbd\
 \x00\x70\
 \x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x72\
 \x00\x75\x00\x2e\x00\x71\x00\x6d\
+\x00\x15\
+\x09\xe1\x0c\xbd\
+\x00\x70\
+\x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x65\
+\x00\x6c\x00\x2e\x00\x71\x00\x6d\
+\x00\x15\
+\x09\xe0\xbc\xbd\
+\x00\x70\
+\x00\x79\x00\x73\x00\x6f\x00\x75\x00\x6e\x00\x64\x00\x61\x00\x6e\x00\x61\x00\x6c\x00\x79\x00\x73\x00\x65\x00\x72\x00\x5f\x00\x64\
+\x00\x65\x00\x2e\x00\x71\x00\x6d\
 "
 
 qt_resource_struct_v1 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x00\x60\x00\x02\x00\x00\x00\x07\x00\x00\x00\x04\
-\x00\x00\x00\x4a\x00\x01\x00\x00\x00\x01\x00\x00\x37\x43\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x62\x02\
-\x00\x00\x01\x74\x00\x00\x00\x00\x00\x01\x00\x00\x61\xee\
-\x00\x00\x00\xe4\x00\x00\x00\x00\x00\x01\x00\x00\x45\xc7\
+\x00\x00\x00\x34\x00\x00\x00\x00\x00\x01\x00\x00\x0d\xf2\
+\x00\x00\x00\x16\x00\x02\x00\x00\x00\x07\x00\x00\x00\x04\
+\x00\x00\x00\x00\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x63\x21\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x63\x65\
+\x00\x00\x01\x74\x00\x00\x00\x00\x00\x01\x00\x00\x63\x51\
 \x00\x00\x00\x7e\x00\x00\x00\x00\x00\x01\x00\x00\x45\x35\
-\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x60\xff\
-\x00\x00\x01\x14\x00\x01\x00\x00\x00\x01\x00\x00\x45\xdb\
+\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00\x62\x32\
+\x00\x00\x00\xe4\x00\x01\x00\x00\x00\x01\x00\x00\x45\xc7\
 \x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\x45\x49\
 "
 
 qt_resource_struct_v2 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x00\x34\x00\x00\x00\x00\x00\x01\x00\x00\x0d\xf2\
 \x00\x00\x01\x28\xee\x1a\x52\x30\
-\x00\x00\x00\x60\x00\x02\x00\x00\x00\x07\x00\x00\x00\x04\
+\x00\x00\x00\x16\x00\x02\x00\x00\x00\x07\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x4a\x00\x01\x00\x00\x00\x01\x00\x00\x37\x43\
+\x00\x00\x00\x00\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x33\x5e\x96\xe0\x50\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x62\x02\
-\x00\x00\x01\x88\x81\xed\x73\x7f\
-\x00\x00\x01\x74\x00\x00\x00\x00\x00\x01\x00\x00\x61\xee\
-\x00\x00\x01\x88\x81\xed\x73\x7b\
-\x00\x00\x00\xe4\x00\x00\x00\x00\x00\x01\x00\x00\x45\xc7\
-\x00\x00\x01\x88\x81\xed\x73\x71\
+\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x63\x21\
+\x00\x00\x01\x88\x9d\x18\x9f\xb4\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x63\x65\
+\x00\x00\x01\x88\x9d\x18\x9f\xb0\
+\x00\x00\x01\x74\x00\x00\x00\x00\x00\x01\x00\x00\x63\x51\
+\x00\x00\x01\x88\x9d\x18\x9f\xa8\
 \x00\x00\x00\x7e\x00\x00\x00\x00\x00\x01\x00\x00\x45\x35\
-\x00\x00\x01\x88\x81\xed\x73\x76\
-\x00\x00\x01\x44\x00\x00\x00\x00\x00\x01\x00\x00\x60\xff\
-\x00\x00\x01\x88\x81\xed\x73\x67\
-\x00\x00\x01\x14\x00\x01\x00\x00\x00\x01\x00\x00\x45\xdb\
-\x00\x00\x01\x88\x81\xed\x73\x62\
+\x00\x00\x01\x88\x9d\x18\x9f\xac\
+\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00\x62\x32\
+\x00\x00\x01\x88\x9d\x18\x9f\xa0\
+\x00\x00\x00\xe4\x00\x01\x00\x00\x00\x01\x00\x00\x45\xc7\
+\x00\x00\x01\x88\x9d\x18\x9f\x9c\
 \x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\x45\x49\
-\x00\x00\x01\x88\x81\xed\x73\x6c\
+\x00\x00\x01\x88\x9d\x18\x9f\xa4\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
 else:
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/random_id.py` & `pysoundanalyser-0.3.4/pysoundanalyser/random_id.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/sndlib.py` & `pysoundanalyser-0.3.4/pysoundanalyser/sndlib.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/threaded_plotters.py` & `pysoundanalyser-0.3.4/pysoundanalyser/threaded_plotters.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/utilities_open_manual.py` & `pysoundanalyser-0.3.4/pysoundanalyser/utilities_open_manual.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/utility_functions.py` & `pysoundanalyser-0.3.4/pysoundanalyser/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/wavpy.py` & `pysoundanalyser-0.3.4/pysoundanalyser/wavpy.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/wavpy_sndf.py` & `pysoundanalyser-0.3.4/pysoundanalyser/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_acf_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_acf_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_autocorrelogram_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_autocorrelogram_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_generic_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_generic_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_spectrogram_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_spectrogram_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_spectrum_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_spectrum_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser/win_waveform_plot.py` & `pysoundanalyser-0.3.4/pysoundanalyser/win_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser.egg-info/PKG-INFO` & `pysoundanalyser-0.3.4/pysoundanalyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.2
+Version: 0.3.4
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysoundanalyser-0.3.2/pysoundanalyser.egg-info/SOURCES.txt` & `pysoundanalyser-0.3.4/pysoundanalyser.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,42 @@
 CREDITS.txt
 INSTALL.txt
 MANIFEST.in
 README.md
 pyproject.toml
 pysoundanalyser.desktop
 resources.qrc
+setup_cx.py
 icons/exit.svg
 icons/johnny_automatic_crashing_wave.ico
 icons/johnny_automatic_crashing_wave.png
 icons/johnny_automatic_crashing_wave.svg
 prep-release/launchpad_build.py
 prep-release/make_deb.py
 prep-release/minor_minor_number.txt
 prep-release/mkupdate_pyqt5.sh
 prep-release/mkupdate_pyqt6.sh
+prep-release/pypi_build.sh
 prep-release/pysoundanalyser.pro
 prep-release/pysoundanalyser_de.ts
 prep-release/pysoundanalyser_el.ts
 prep-release/pysoundanalyser_en_GB.ts
 prep-release/pysoundanalyser_es.ts
 prep-release/pysoundanalyser_fr.ts
 prep-release/pysoundanalyser_it.ts
 prep-release/pysoundanalyser_ru.ts
 prep-release/release.py
 prep-release/switch_pyqt5.py
 prep-release/switch_pyqt6.py
 prep-release/uploadToWebsite.py
+prep-release/win_installer_readme.md
+prep-release/win_launch_iss_compiler.bat
+prep-release/win_launch_iss_compiler.sh
+prep-release/win_pysoundanalyser.iss
+prep-release/winbuild.py
 prep-release/debian/changelog
 prep-release/debian/compat
 prep-release/debian/control
 prep-release/debian/copyright
 prep-release/debian/docs
 prep-release/debian/links
 prep-release/debian/rules
```

### Comparing `pysoundanalyser-0.3.2/resources.qrc` & `pysoundanalyser-0.3.4/resources.qrc`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/translations/pysoundanalyser_it.qm` & `pysoundanalyser-0.3.4/translations/pysoundanalyser_it.qm`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.2/translations/pysoundanalyser_it_IT.qm` & `pysoundanalyser-0.3.4/translations/pysoundanalyser_it_IT.qm`

 * *Files identical despite different names*

