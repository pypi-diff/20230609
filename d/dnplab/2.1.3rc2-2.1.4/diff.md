# Comparing `tmp/dnplab-2.1.3rc2.tar.gz` & `tmp/dnplab-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-6lsc1l8v\dnplab-2.1.3rc2.tar", last modified: Fri Jun  2 19:19:45 2023, max compression
+gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-kdsuuzks\dnplab-2.1.4.tar", last modified: Fri Jun  9 16:57:33 2023, max compression
```

## Comparing `dnplab-2.1.3rc2.tar` & `dnplab-2.1.4.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.789973 dnplab-2.1.3rc2/
--rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     2379 2023-06-02 19:19:45.789973 dnplab-2.1.3rc2/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.735520 dnplab-2.1.3rc2/dnplab/
--rw-rw-rw-   0        0        0      636 2023-05-31 16:23:12.000000 dnplab-2.1.3rc2/dnplab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.746907 dnplab-2.1.3rc2/dnplab/analysis/
--rw-rw-rw-   0        0        0      170 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/analysis/__init__.py
--rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/analysis/hydration.py
--rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/analysis/relaxation_fit.py
--rw-rw-rw-   0        0        0     3739 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/analysis/simulate_enhancement_profiles.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.747903 dnplab-2.1.3rc2/dnplab/config/
--rw-rw-rw-   0        0        0     2380 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/dnplab/config/dnplab.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.749897 dnplab-2.1.3rc2/dnplab/constants/
--rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/dnplab/constants/__init__.py
--rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/constants/constants.py
--rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/constants/mrProperties.py
--rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/constants/radicalProperties.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.753887 dnplab-2.1.3rc2/dnplab/core/
--rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/dnplab/core/__init__.py
--rw-rw-rw-   0        0        0    36820 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/dnplab/core/base.py
--rw-rw-rw-   0        0        0     6793 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/core/coord.py
--rw-rw-rw-   0        0        0     7769 2023-05-31 16:23:12.000000 dnplab-2.1.3rc2/dnplab/core/data.py
--rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/core/ufunc.py
--rw-rw-rw-   0        0        0     3106 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/core/util.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.754884 dnplab-2.1.3rc2/dnplab/fitting/
--rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/dnplab/fitting/__init__.py
--rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/fitting/general.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.766896 dnplab-2.1.3rc2/dnplab/io/
--rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/__init__.py
--rw-rw-rw-   0        0        0    15036 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/bes3t.py
--rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/io/cnsi.py
--rw-rw-rw-   0        0        0     5932 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/io/delta.py
--rw-rw-rw-   0        0        0     5740 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/h5.py
--rw-rw-rw-   0        0        0     6862 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/io/load.py
--rw-rw-rw-   0        0        0     3269 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/io/load_csv.py
--rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/io/power.py
--rw-rw-rw-   0        0        0    10252 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/io/prospa.py
--rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/io/random.py
--rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/save.py
--rw-rw-rw-   0        0        0     5027 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/io/specman.py
--rw-rw-rw-   0        0        0     2799 2023-05-31 16:23:10.000000 dnplab-2.1.3rc2/dnplab/io/tnmr.py
--rw-rw-rw-   0        0        0    20255 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/io/topspin.py
--rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/vna.py
--rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/vnmrj.py
--rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/io/winepr.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.768890 dnplab-2.1.3rc2/dnplab/math/
--rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.3rc2/dnplab/math/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/math/lineshape.py
--rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/math/relaxation.py
--rw-rw-rw-   0        0        0     3985 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/dnplab/math/window.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.771881 dnplab-2.1.3rc2/dnplab/plotting/
--rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/dnplab/plotting/__init__.py
--rw-rw-rw-   0        0        0     9309 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/dnplab/plotting/general.py
--rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/plotting/image.py
--rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/plotting/stack_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.777870 dnplab-2.1.3rc2/dnplab/processing/
--rw-rw-rw-   0        0        0      270 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/dnplab/processing/__init__.py
--rw-rw-rw-   0        0        0     7427 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/processing/align.py
--rw-rw-rw-   0        0        0     2828 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/processing/apodization.py
--rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/processing/conversion.py
--rw-rw-rw-   0        0        0     5159 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/processing/fft.py
--rw-rw-rw-   0        0        0     9442 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/dnplab/processing/helpers.py
--rw-rw-rw-   0        0        0     3607 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/processing/integration.py
--rw-rw-rw-   0        0        0     2080 2023-03-16 14:57:24.000000 dnplab-2.1.3rc2/dnplab/processing/offset.py
--rw-rw-rw-   0        0        0     9313 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/processing/phase.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.778863 dnplab-2.1.3rc2/dnplab/reporting/
--rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/dnplab/reporting/__init__.py
--rw-rw-rw-   0        0        0       26 2023-06-02 19:11:14.000000 dnplab-2.1.3rc2/dnplab/version.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.780857 dnplab-2.1.3rc2/dnplab/widgets/
--rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/widgets/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/dnplab/widgets/align_widget.py
--rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/dnplab/widgets/phase_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.743914 dnplab-2.1.3rc2/dnplab.egg-info/
--rw-rw-rw-   0        0        0     2379 2023-06-02 19:19:45.000000 dnplab-2.1.3rc2/dnplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1887 2023-06-02 19:19:45.000000 dnplab-2.1.3rc2/dnplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:19:45.000000 dnplab-2.1.3rc2/dnplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 19:19:45.000000 dnplab-2.1.3rc2/dnplab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-02 19:19:45.000000 dnplab-2.1.3rc2/dnplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:19:45.789973 dnplab-2.1.3rc2/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-06-02 16:43:25.000000 dnplab-2.1.3rc2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:19:45.788189 dnplab-2.1.3rc2/unittests/
--rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/unittests/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-05-31 16:23:12.000000 dnplab-2.1.3rc2/unittests/test_data_class.py
--rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/unittests/test_dnp_nmr.py
--rw-rw-rw-   0        0        0     3676 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/unittests/test_dnp_tools.py
--rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/unittests/test_general_fit.py
--rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/unittests/test_hydration.py
--rw-rw-rw-   0        0        0    10320 2023-04-28 19:23:06.000000 dnplab-2.1.3rc2/unittests/test_io.py
--rw-rw-rw-   0        0        0     1884 2022-08-30 17:05:30.000000 dnplab-2.1.3rc2/unittests/test_load.py
--rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.3rc2/unittests/test_nddata_core.py
--rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/unittests/test_save.py
--rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.3rc2/unittests/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.247744 dnplab-2.1.4/
+-rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2376 2023-06-09 16:57:33.246746 dnplab-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.185615 dnplab-2.1.4/dnplab/
+-rw-rw-rw-   0        0        0      636 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.199576 dnplab-2.1.4/dnplab/analysis/
+-rw-rw-rw-   0        0        0      170 2023-04-28 19:23:06.000000 dnplab-2.1.4/dnplab/analysis/__init__.py
+-rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/analysis/hydration.py
+-rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/analysis/relaxation_fit.py
+-rw-rw-rw-   0        0        0     3739 2023-04-28 19:23:06.000000 dnplab-2.1.4/dnplab/analysis/simulate_enhancement_profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.201571 dnplab-2.1.4/dnplab/config/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/config/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/config/config.py
+-rw-rw-rw-   0        0        0     7868 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/config/dnplab.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.204563 dnplab-2.1.4/dnplab/constants/
+-rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.4/dnplab/constants/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/constants/constants.py
+-rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/constants/mrProperties.py
+-rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/constants/radicalProperties.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.210550 dnplab-2.1.4/dnplab/core/
+-rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.4/dnplab/core/__init__.py
+-rw-rw-rw-   0        0        0    38601 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/core/base.py
+-rw-rw-rw-   0        0        0     6815 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/core/coord.py
+-rw-rw-rw-   0        0        0    10720 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/core/data.py
+-rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/core/ufunc.py
+-rw-rw-rw-   0        0        0     3332 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/core/util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.212541 dnplab-2.1.4/dnplab/fitting/
+-rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.4/dnplab/fitting/__init__.py
+-rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/fitting/general.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.224126 dnplab-2.1.4/dnplab/io/
+-rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/io/__init__.py
+-rw-rw-rw-   0        0        0    15086 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/bes3t.py
+-rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/io/cnsi.py
+-rw-rw-rw-   0        0        0     5943 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/delta.py
+-rw-rw-rw-   0        0        0     7003 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/h5.py
+-rw-rw-rw-   0        0        0     9976 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/load.py
+-rw-rw-rw-   0        0        0     3269 2023-04-28 19:23:06.000000 dnplab-2.1.4/dnplab/io/load_csv.py
+-rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/io/power.py
+-rw-rw-rw-   0        0        0    10272 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/prospa.py
+-rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/io/random.py
+-rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/io/save.py
+-rw-rw-rw-   0        0        0     5027 2023-04-28 19:23:06.000000 dnplab-2.1.4/dnplab/io/specman.py
+-rw-rw-rw-   0        0        0     2799 2023-05-31 16:23:10.000000 dnplab-2.1.4/dnplab/io/tnmr.py
+-rw-rw-rw-   0        0        0    20381 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/io/topspin.py
+-rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/io/vna.py
+-rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/io/vnmrj.py
+-rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/io/winepr.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.227118 dnplab-2.1.4/dnplab/math/
+-rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.4/dnplab/math/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/math/lineshape.py
+-rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/math/relaxation.py
+-rw-rw-rw-   0        0        0     4007 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/math/window.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.229112 dnplab-2.1.4/dnplab/plotting/
+-rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.4/dnplab/plotting/__init__.py
+-rw-rw-rw-   0        0        0     9311 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/plotting/general.py
+-rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/plotting/image.py
+-rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.4/dnplab/plotting/stack_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.236273 dnplab-2.1.4/dnplab/processing/
+-rw-rw-rw-   0        0        0      294 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/align.py
+-rw-rw-rw-   0        0        0     3129 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/apodization.py
+-rw-rw-rw-   0        0        0      651 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/average.py
+-rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/processing/conversion.py
+-rw-rw-rw-   0        0        0     5181 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/fft.py
+-rw-rw-rw-   0        0        0    10082 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/helpers.py
+-rw-rw-rw-   0        0        0     3605 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/integration.py
+-rw-rw-rw-   0        0        0     2301 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/offset.py
+-rw-rw-rw-   0        0        0     9277 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/processing/phase.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.236273 dnplab-2.1.4/dnplab/reporting/
+-rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.4/dnplab/reporting/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-09 16:57:10.000000 dnplab-2.1.4/dnplab/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.238268 dnplab-2.1.4/dnplab/widgets/
+-rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.4/dnplab/widgets/align_widget.py
+-rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.4/dnplab/widgets/phase_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.196585 dnplab-2.1.4/dnplab.egg-info/
+-rw-rw-rw-   0        0        0     2376 2023-06-09 16:57:33.000000 dnplab-2.1.4/dnplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1966 2023-06-09 16:57:33.000000 dnplab-2.1.4/dnplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 16:57:33.000000 dnplab-2.1.4/dnplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-09 16:57:33.000000 dnplab-2.1.4/dnplab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 16:57:33.000000 dnplab-2.1.4/dnplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 16:57:33.247744 dnplab-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-06-09 16:57:10.000000 dnplab-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 16:57:33.245750 dnplab-2.1.4/unittests/
+-rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.4/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-06-09 16:57:10.000000 dnplab-2.1.4/unittests/test_data_class.py
+-rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.4/unittests/test_dnp_nmr.py
+-rw-rw-rw-   0        0        0     3676 2023-04-28 19:23:06.000000 dnplab-2.1.4/unittests/test_dnp_tools.py
+-rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.4/unittests/test_general_fit.py
+-rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.4/unittests/test_hydration.py
+-rw-rw-rw-   0        0        0    10356 2023-06-09 16:57:10.000000 dnplab-2.1.4/unittests/test_io.py
+-rw-rw-rw-   0        0        0     1892 2023-06-09 16:57:10.000000 dnplab-2.1.4/unittests/test_load.py
+-rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.4/unittests/test_nddata_core.py
+-rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.4/unittests/test_save.py
+-rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.4/unittests/testing.py
```

### Comparing `dnplab-2.1.3rc2/LICENSE.txt` & `dnplab-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/PKG-INFO` & `dnplab-2.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.3rc2
+Version: 2.1.4
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.3rc2/README.md` & `dnplab-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/__init__.py` & `dnplab-2.1.4/dnplab/__init__.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/analysis/hydration.py` & `dnplab-2.1.4/dnplab/analysis/hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/analysis/relaxation_fit.py` & `dnplab-2.1.4/dnplab/analysis/relaxation_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/analysis/simulate_enhancement_profiles.py` & `dnplab-2.1.4/dnplab/analysis/simulate_enhancement_profiles.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/constants/mrProperties.py` & `dnplab-2.1.4/dnplab/constants/mrProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/constants/radicalProperties.py` & `dnplab-2.1.4/dnplab/constants/radicalProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/core/base.py` & `dnplab-2.1.4/dnplab/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import operator
 import numpy as _np
 import warnings
 from copy import deepcopy
 from collections import OrderedDict
 from .coord import Coords
 import logging
+import warnings
 
 from ..version import __version__
 
 version = __version__
 
 
 def _replaceClassWithAttribute(replace_class, args, kwargs, target_attr="_values"):
@@ -62,15 +63,22 @@
         error (numpy.ndarray): If not None, error for values which are propagated during mathematical operations
         proc_attrs (list): List of processing steps
     """
 
     __array_priority__ = 1000  # radd, rsub, ... should return nddata object
 
     def __init__(
-        self, values=_np.r_[[]], dims=[], coords=[], attrs={}, error=None, **kwargs
+        self,
+        values=_np.r_[[]],
+        dims=[],
+        coords=[],
+        attrs={},
+        dnp_attrs={},
+        error=None,
+        **kwargs
     ):
         self.version = version
 
         # if values is list, convert to numpy array
         if isinstance(values, list):
             values = _np.array(values)
 
@@ -85,14 +93,21 @@
         self._coords = Coords(dims, coords)
 
         if isinstance(attrs, dict):
             self._attrs = attrs
         else:
             raise TypeError('attrs must be type "dict" not %s' % str(type(attrs)))
 
+        if isinstance(dnp_attrs, dict):
+            self._attrs = attrs
+        else:
+            raise TypeError(
+                'dnp_attrs must be type "dict" not %s' % str(type(dnp_attrs))
+            )
+
         if isinstance(error, _np.ndarray) or (error == None):
             self._error = error
         else:
             raise TypeError(
                 'error must be type "numpy.ndarray" or "None" not %s' % str(type(error))
             )
 
@@ -100,15 +115,23 @@
             proc_attrs = kwargs["proc_attrs"]
             if isinstance(proc_attrs, list):
                 self._proc_attrs = proc_attrs
             else:
                 raise TypeError
 
         if not self._self_consistent():
-            warnings.warn("Dimensions not consistent")
+            warnings.warn("Data Object Dimensions are not consistent.")
+            if not self._check_dims(self.dims):
+                warnings.warn(
+                    "Dims Check Failed. Dims must be list of strings. Length of dims should match number of dimensions in values."
+                )
+            if not self._check_coords(self._coords):
+                warnings.warn(
+                    "Coords Check Failed. Each coord should be a numpy array matching the length of each dimension in values."
+                )
 
     @property
     def __version__(self):
         return self._nddata_core_version
 
     def _check_dims(self, dims):
         """Check that list is a list of strings with no duplicates
@@ -122,47 +145,69 @@
 
         # test that all members are strings
         all_strings = all([isinstance(dims[x], str) for x in range(len(dims))])
 
         # test if any duplicates exist
         any_duplicates = len(dims) == len(set(dims))
 
-        return all_strings and any_duplicates
+        # Test if number of dims matches number of dimensions
+        if self.size != 0:  # Case where array is not empty
+            shape_check = len(self.values.shape) == len(self.dims)
+        else:  # Case where array is empty
+            shape_check = len(self.dims) == 0
+
+        return all_strings and any_duplicates and shape_check
 
     def _check_coords(self, coords):
         """Check that coords is list of 1d numpy arrays
 
         Args:
             coords: coords object to check if valid coords
 
         Returns:
             bool: True if valid coords. False, otherwise.
         """
 
+        # Check that coords is list of 1d numpy arrays
         for coord in coords:
             if isinstance(coord, _np.ndarray):
                 if len(coord.shape) == 1:
                     pass
                 else:
                     return False
             else:
                 return False
 
+        shape = self.values.shape
+
+        # Check Shapes are consistent
+        if len(shape) != len(coords):
+            return False
+
+        # Check that each coord length matches shape of each dimension in values
+        for coord_ix, coord in enumerate(coords):
+            if len(coord) != shape[coord_ix]:
+                return False
+
         return True
 
     def _check_error(self, error):
         """Check that error attribute is numpy array and it's size matches values
 
         Args:
             error: Object to check if valid error
 
         Returns:
             bool: True if valid error. False otherwise.
         """
 
+        # Error is type None if it doesn't exist
+        if error is None:
+            return True
+
         check_type = isinstance(error, _np.ndarray)
 
         if check_type:
             check_size = error.size == self._values.size
         else:
             check_size = False
 
@@ -176,15 +221,15 @@
         """
 
         if self._values.size == 0:
             coords_check = len(self._coords) == 0
         else:
             coords_check = list(self._values.shape) == list(self.coords.shape)
 
-        dims_check = len(self.values.shape) == len(self.dims)
+        dims_check = self._check_dims(self.dims)
 
         return coords_check and dims_check
 
     def _attrs_valid(self):
         """Verify attrs attribute is valid. All values in attrs must be list, numpy.ndarray, int, float, complex, or str.
 
         Returns:
@@ -415,15 +460,18 @@
 
         Returns:
             int: Index value of dim
         """
         if dim in self.dims:
             return self.coords.index(dim)
         else:
-            raise ValueError("%s not in %s" % (dim, self.dims))
+            raise ValueError(
+                'The dimension "%s" is not in dims. Available dimensions are: %s'
+                % (dim, self.dims)
+            )
 
     def __truediv__(self, b):
         if isinstance(b, ABCData):
             a, b = self.align(b)
 
             a.values = a.values / b.values
 
@@ -732,14 +780,15 @@
         """
         a = self.copy()
         index = a.index(dim)
         a.values = a.values.sum(index)
         if a.error is not None:
             a.error = a.error.std(index)
         a.coords.pop(dim)
+        DeprecationWarning("Method '.sum()' will be removed on September 1st, 2023 ")
         return a
 
     def align(self, b):
         """Align two data objects for numerical operations
 
         Args:
             b: Object to align with self
```

### Comparing `dnplab-2.1.3rc2/dnplab/core/coord.py` & `dnplab-2.1.4/dnplab/core/coord.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             if isinstance(coord, (range, list)):
                 coords[index] = _np.array(coord)
 
         if self._check_dims(dims):
             self._dims = deepcopy(dims)
         else:
             raise TypeError(
-                "dims must be list of str, you provided types {0}".format(
+                "dims must be list of unique strings (type str), you provided types {0}".format(
                     [type(k) for k in dims]
                 )
             )
 
         if self._check_coords(coords):
             self._coords = deepcopy(coords)
         else:
```

### Comparing `dnplab-2.1.3rc2/dnplab/core/ufunc.py` & `dnplab-2.1.4/dnplab/core/ufunc.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/core/util.py` & `dnplab-2.1.4/dnplab/core/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,64 +37,67 @@
                 this_shape,
                 shape,
             )
 
     dims = data_list[0].dims
     coords = data_list[0].coords.coords
     attrs = data_list[0].attrs
+    dnplab_attrs = data_list[0].dnplab_attrs
 
     values = _np.stack(values_list, axis=-1)
 
     dims.append(dim)
 
     if coord is None:
         coords.append(_np.arange(len(data_list)))
     else:
         coords.append(coord)
 
-    data = DNPData(values, dims, coords, attrs)
+    data = DNPData(values, dims, coords, attrs, dnplab_attrs)
 
     return data
 
 
-def update_axis(data, new_dims, start_stop, spacing="lin", verbose=False):
+def update_axis(data, start_stop, dim=0, new_dims=0, spacing="lin", verbose=False):
     """Update axis
 
     Update dimensions (dims) and axis (coords) of a dnpDate object. The name of the dims will be replaced with the name giving in new_dims. The variable start_stop defines the values of the new coords. This can be either a tuple (start values, stop value) or a vector with values. If the start and stop value is provided, either a linear axis (spacing = "lin", default) or a logarithmically space (spacing = "log") will be created. The new axis will replace the coords in the dnpdata object.
 
     The function is currently implemented for 1D objects only.
 
     Args:
-        data (DNPData): dnpData objetc
-        new_dims (str): Name of the new dimension. If None the name will not be changed.
-        start_stop(tuple or vector): Coords for new dimension
-        spacing (str): "lin" for linear spaced axis or "log" for logarithmically spaced axis
+        data (DNPData):                 dnpData object
+        start_stop(tuple or vector):    Coords for new dimension
+        dim (int):                      Dimension to act on
+        new_dims (str):                 Name of the new dimension. If None the name will not be changed.
+        spacing (str):                  "lin" for linear spaced axis or "log" for logarithmically spaced axis
 
     Returns:
         data (DNPData): concatenated data object
     """
 
     out = data.copy()
+    data_shape = _np.shape(out.values)
 
     if new_dims == None:
-        new_dims = out.dims[0]
+        new_dims = out.dims[dim]
 
-    out.rename(out.dims[0], new_dims)
+    out.rename(out.dims[dim], new_dims)
 
     if verbose == True:
         print("New dims name:", new_dims)
 
     if len(start_stop) == 2:
         if spacing == "lin":
             out.coords[new_dims] = _np.linspace(
-                start_stop[0], start_stop[1], len(out.values)
+                start_stop[0], start_stop[1], data_shape[dim]
             )
 
         elif spacing == "log":
             out.coords[new_dims] = _np.logspace(
-                start_stop[0], start_stop[1], len(out.values)
+                start_stop[0], start_stop[1], data_shape[dim]
             )
 
     elif len(start_stop) > 2:
         out.coords[new_dims] = start_stop
 
     return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/fitting/general.py` & `dnplab-2.1.4/dnplab/fitting/general.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/bes3t.py` & `dnplab-2.1.4/dnplab/io/bes3t.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,21 @@
         if os.path.isfile(path + ".YGF"):
             path_ygf = path + ".YGF"
 
     else:
         raise TypeError("data file must be .DTA, .DSC, .YGF, or .ZGF")
 
     attrs = load_dsc(path_dsc)
+
     values, dims, coords, attrs = load_dta(
         path_dta, path_xgf, path_ygf, path_zgf, attrs
     )
-
-    # Assign data/spectrum type
+    attrs["spectrometer_format"] = "xepr"
     attrs["experiment_type"] = "epr_spectrum"
+    attrs["nrScans"] = attrs["nscans"]
 
     bes3t_data = DNPData(values, dims, coords, attrs)
 
     return bes3t_data
 
 
 def load_dsc(path):
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/cnsi.py` & `dnplab-2.1.4/dnplab/io/cnsi.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/delta.py` & `dnplab-2.1.4/dnplab/io/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as _np
+import re
 from struct import unpack
 from .. import DNPData
 
 
 def import_delta(path):
     """Import Delta data and return DNPData object
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/h5.py` & `dnplab-2.1.4/dnplab/io/h5.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     return dnp_dict
 
 
 def read_dnpdata(dnpdata_group):
     coords = []
     dims = []
     attrs = {}
+    dnplab_attrs = {}
+    proc_attrs = {}
     values = dnpdata_group["values"][:]
     version = dnpdata_group.attrs["dnplab_version"]
 
     for index in range(len(_np.shape(values))):
         dim_key = dnpdata_group["values"].dims[index].keys()[0]  # assumes 1 key only
         coords.append(dnpdata_group["values"].dims[index][dim_key][:])
         dims.append(dim_key)
@@ -61,22 +63,34 @@
             ix = replace_types.index(v)
             v = python_types[ix]
         attrs[k] = v
     for k in dnpdata_group["attrs"]:
         v = dnpdata_group["attrs"][k][:]
         attrs[k] = v
 
-    data = DNPData(values, dims, coords, attrs)
+    if "dnplab_attrs" in dnpdata_group.keys():
+        for k in dnpdata_group["dnplab_attrs"].attrs.keys():
+            v = dnpdata_group["dnplab_attrs"].attrs[k]
+            if v in replace_types:
+                ix = replace_types.index(v)
+                v = python_types[ix]
+            dnplab_attrs[k] = v
+        for k in dnpdata_group["dnplab_attrs"]:
+            v = dnpdata_group["dnplab_attrs"][k][:]
+            dnplab_attrs[k] = v
+
+    data = DNPData(values, dims, coords, attrs, dnplab_attrs)
 
     if "proc_attrs" in dnpdata_group.keys():
         proc_attrs = []
         for k in dnpdata_group["proc_attrs"].keys():
             proc_attrs_name = k.split(":", 1)[1]
             proc_attrs_dict = dict(dnpdata_group["proc_attrs"][k].attrs)
             data.add_proc_attrs(proc_attrs_name, proc_attrs_dict)
+
     return data
 
 
 def read_dict(dnpdata_group):
     data = dict(dnpdata_group["attrs"].attrs)
     return data
 
@@ -95,26 +109,30 @@
     else:
         mode = "w-"
 
     keysList = dataDict.keys()
 
     f = h5py.File(path, mode)
 
-    for key in keysList:
-        dnpDataObject = dataDict[key]
-
-        dnpDataGroup = f.create_group(key, track_order=True)
-        if isinstance(dnpDataObject, DNPData):
-            write_dnpdata(dnpDataGroup, dnpDataObject)
-        elif isinstance(dnpDataObject, dict):
-            write_dict(dnpDataGroup, dnpDataObject)
-        else:
-            warnings.warn("Could not write key: %s" % str(key))
-
-    f.close()
+    try:
+        for key in keysList:
+            dnpDataObject = dataDict[key]
+            dnpDataGroup = f.create_group(key, track_order=True)
+            if isinstance(dnpDataObject, DNPData):
+                write_dnpdata(dnpDataGroup, dnpDataObject)
+            elif isinstance(dnpDataObject, dict):
+                write_dict(dnpDataGroup, dnpDataObject)
+            else:
+                warnings.warn("Could not write key: %s" % str(key))
+
+        f.close()
+
+    except:
+        f.close()
+        raise Warning("h5 close due to error")
 
 
 def write_dnpdata(dnpDataGroup, dnpDataObject):
     """Takes file/group and writes dnpData object to it
 
     Args:
         dnpDataGroup: h5 group to save data to
@@ -131,26 +149,41 @@
         label = dnpDataObject.dims[ix]
         this_axes = dnpDataObject.coords[ix]
         dims_group.create_dataset(label, data=this_axes)
         dims_group[label].make_scale(label)
 
         dnp_dataset.dims[ix].attach_scale(dims_group[label])
 
-    # Save Parameters
+    # Save Experiment Attributes
     for key in dnpDataObject.attrs:
         value = dnpDataObject.attrs[key]
 
         if isinstance(value, _np.ndarray):
             attrs_group.create_dataset(key, data=value)
         else:
             if value in python_types:
                 ix = python_types.index(value)
                 value = replace_types[ix]
             attrs_group.attrs[key] = value
 
+    # Save DNPLab Attributes
+    if hasattr(dnpDataObject, "dnplab_attrs"):
+        dnplab_attrs_group = dnpDataGroup.create_group("dnplab_attrs", track_order=True)
+
+        for key in dnpDataObject.dnplab_attrs:
+            value = dnpDataObject.dnplab_attrs[key]
+
+            if isinstance(value, _np.ndarray):
+                dnplab_attrs_group.create_dataset(key, data=value)
+            else:
+                if value in python_types:
+                    ix = python_types.index(value)
+                    value = replace_types[ix]
+                dnplab_attrs_group.attrs[key] = value
+
     # Save proc_steps
     if hasattr(dnpDataObject, "proc_attrs"):
         proc_attrs = dnpDataObject.proc_attrs
         proc_attrs_group = dnpDataGroup.create_group("proc_attrs", track_order=True)
         for ix in range(len(proc_attrs)):
             proc_step_name = proc_attrs[ix][0]
             proc_dict = proc_attrs[ix][1]
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/load.py` & `dnplab-2.1.4/dnplab/io/load.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 from . import *
+import re
 
 from ..core.util import concat
+from ..config.config import DNPLAB_CONFIG
 
 
-def load(path, data_type=None, dim=None, coord=[], verbose=False, *args, **kwargs):
+def load(path, data_format=None, dim=None, coord=[], verbose=False, *args, **kwargs):
     """Import data from different spectrometer formats
 
     Args:
         path (str, list): Path to data directory or list of directories
-        data_type (str): Type of spectrometer data to import (optional). Allowed values: "prospa", "topspin", "delta", "vnmrj", "tnmr", "specman", "xenon", "xepr", "winepr", "esp", "h5", "power", "vna", "cnsi_powers"
+        data_format (str): format of spectrometer data to import (optional). Allowed values: "prospa", "topspin", "delta", "vnmrj", "tnmr", "specman", "xenon", "xepr", "winepr", "esp", "h5", "power", "vna", "cnsi_powers"
         dim (str): If giving directories as list, name of dimension to concatenate data along
         coord (numpy.ndarray): If giving directories as list, coordinates of new dimension
         verbose (bool): If true, print debugging output
         args: Args passed to spectrometer specific import function
         kwargs: Key word args passed to spectrometer specific import function
 
     Returns:
@@ -37,105 +39,111 @@
             )
 
         data_list = []
         if dim is None:
             dim = "unnamed"
         for filename in path:
             data = load_file(
-                filename, data_type=data_type, verbose=verbose, *args, **kwargs
+                filename, data_format=data_format, verbose=verbose, *args, **kwargs
             )
             data_list.append(data)
         # coord could be empty list
         if len(coord) == 0:
             coord = None  # to not break concat call signature
 
-        return concat(data_list, dim=dim, coord=coord)
+        data = concat(data_list, dim=dim, coord=coord)
+
+        return data
 
     else:
-        return load_file(path, data_type=data_type, verbose=verbose, *args, **kwargs)
+        return load_file(
+            path, data_format=data_format, verbose=verbose, *args, **kwargs
+        )
 
 
-def load_file(path, data_type=None, verbose=False, *args, **kwargs):
+def load_file(path, data_format=None, verbose=False, *args, **kwargs):
     """Import data from different spectrometer formats
 
     Args:
         path (str): Path to data directory or file
-        data_type (str): Type of spectrometer data to import (optional). Allowed values: "prospa", "topspin", "delta", "vnmrj", "tnmr", "specman", "xenon", "xepr", "winepr", "esp", "h5", "power", "vna", "cnsi_powers"
+        data_format (str): Format of spectrometer data to import (optional). Allowed values: "prospa", "topspin", "delta", "vnmrj", "tnmr", "specman", "xenon", "xepr", "winepr", "esp", "h5", "power", "vna", "cnsi_powers"
         verbose (bool): If true, print additional debug outputs
         args: Arguments passed to spectrometer specific import function
         kwargs: Key word arguments passed to spectrometer specific import function
 
     Returns:
         data (dnpData): Data object
     """
 
     path = os.path.normpath(path)
     if os.path.isdir(path) and path[-1] != os.sep:
         path = path + os.sep
 
-    if data_type == None:
-        data_type = autodetect(path, verbose=verbose)
-
-    if data_type == "prospa":
-        return prospa.import_prospa(path, *args, **kwargs)
+    if data_format == None:
+        data_format = autodetect(path, verbose=verbose)
 
-    elif data_type == "topspin":
-        return topspin.import_topspin(path, verbose=verbose, *args, **kwargs)
+    if data_format == "prospa":
+        data = prospa.import_prospa(path, *args, **kwargs)
 
-    elif data_type == "topspin pdata":
-        # import_topspin should also handle this type, this is a workaround
-        return topspin.load_pdata(path, verbose=verbose, *args, **kwargs)
+    elif data_format == "topspin":
+        data = topspin.import_topspin(path, verbose=verbose, *args, **kwargs)
 
-    elif data_type == "topspin dir":
-        return topspin.import_topspin_dir(path, *args, **kwargs)
+    elif data_format == "topspin pdata":
+        # import_topspin should also handle this format, this is a workaround
+        data = topspin.load_pdata(path, verbose=verbose, *args, **kwargs)
 
-    elif data_type == "delta":
-        return delta.import_delta(path, *args, **kwargs)
+    elif data_format == "delta":
+        data = delta.import_delta(path, *args, **kwargs)
 
-    elif data_type == "vnmrj":
-        return vnmrj.import_vnmrj(path, *args, **kwargs)
+    elif data_format == "vnmrj":
+        data = vnmrj.import_vnmrj(path, *args, **kwargs)
 
-    elif data_type == "tnmr":
-        return tnmr.import_tnmr(path, *args, **kwargs)
+    elif data_format == "tnmr":
+        data = tnmr.import_tnmr(path, *args, **kwargs)
 
-    elif data_type == "specman":
-        return specman.import_specman(path, *args, **kwargs)
+    elif data_format == "specman":
+        data = specman.import_specman(path, *args, **kwargs)
 
-    elif data_type in ["xepr", "xenon"]:
-        return bes3t.import_bes3t(path, *args, **kwargs)
+    elif data_format in ["xepr", "xenon"]:
+        data = bes3t.import_bes3t(path, *args, **kwargs)
 
-    elif data_type in ["winepr", "esp"]:
-        return winepr.import_winepr(path, *args, **kwargs)
+    elif data_format in ["winepr", "esp"]:
+        data = winepr.import_winepr(path, *args, **kwargs)
 
-    elif data_type == "h5":
-        return h5.load_h5(path, *args, **kwargs)
+    elif data_format == "h5":
+        data = h5.load_h5(path, *args, **kwargs)
 
-    elif data_type == "power":
-        return power.importPower(path, *args, **kwargs)
+    elif data_format == "power":
+        data = power.import_power(path, *args, **kwargs)
 
-    elif data_type == "vna":
-        return vna.import_vna(path, *args, **kwargs)
+    elif data_format == "vna":
+        data = vna.import_vna(path, *args, **kwargs)
 
-    elif data_type == "cnsi_powers":
-        return cnsi.get_powers(path, *args, **kwargs)
+    elif data_format == "cnsi_powers":
+        data = cnsi.get_powers(path, *args, **kwargs)
 
     else:
-        raise ValueError("Invalid data type: %s" % data_type)
+        raise ValueError("Invalid data format: %s" % data_format)
+
+    if data_format not in ["h5", "power", "vna", "cnsi_powers"]:
+        data = _assign_dnplab_attrs(data, data_format)
+
+    return data
 
 
 # TODO rename to detect_file_format
 def autodetect(test_path, verbose=False):
-    """Automatically detect spectrometer format
+    """Automatically detect data format
 
     Args:
         test_path (str): Test directory
         verbose (bool): If true, print output for debugging
 
     Returns:
-        str: Spectrometer type as string
+        str: Data format as string
 
     """
 
     if verbose == True:
         print("current directory:", os.getcwd())
         print("data path:", test_path)
         abs_path = os.path.abspath(test_path)
@@ -148,47 +156,140 @@
             print("removed trailing separator:", os.sep)
 
     path_exten = os.path.splitext(test_path)[1]
     if path_exten != "" and verbose:
         print("Extension:", path_exten)
 
     if path_exten == ".DSC" or path_exten == ".DTA" or path_exten == ".YGF":
-        spectrometer_format = "xepr"
+        data_format = "xepr"
     elif path_exten in [".par", ".spc"]:
-        spectrometer_format = "winepr"
+        data_format = "winepr"
     elif path_exten in [".d01", ".exp"]:
-        spectrometer_format = "specman"
+        data_format = "specman"
     elif path_exten == ".jdf":
-        spectrometer_format = "delta"
+        data_format = "delta"
     elif (
         os.path.isdir(test_path)
         #        and ("fid" in os.listdir(test_path) or "ser" in os.listdir(test_path))
         and ("acqu" in os.listdir(test_path) or "acqus" in os.listdir(test_path))
     ):
-        spectrometer_format = "topspin"
+        data_format = "topspin"
     elif os.path.isdir(test_path) and (
         "proc" in os.listdir(test_path) or "procss" in os.listdir(test_path)
     ):
-        spectrometer_format = "topspin pdata"
+        data_format = "topspin pdata"
     elif os.path.isdir(test_path) and path_exten == ".fid":
-        spectrometer_format = "vnmrj"
+        data_format = "vnmrj"
     elif path_exten in [".1d", ".2d", ".3d", ".4d"]:
-        spectrometer_format = "prospa"
+        data_format = "prospa"
     elif path_exten == ".tnt":
-        spectrometer_format = "tnmr"
+        data_format = "tnmr"
     elif (
         os.path.isdir(test_path)
         and "acqu.par" in os.listdir(test_path)
         and "data.csv" in os.listdir(test_path)
     ):
-        spectrometer_format = "prospa"
+        data_format = "prospa"
     elif path_exten == ".h5":
-        spectrometer_format = "h5"
+        data_format = "h5"
     else:
         raise TypeError(
-            "No data type given and autodetect failed to detect format, please specify a format"
+            "No data format given and autodetect failed to detect format, please specify a format"
         )
 
     if verbose:
-        print("Spectrometer Format:", spectrometer_format)
+        print("Data Format:", data_format)
+
+    return data_format
+
+
+def _assign_dnplab_attrs(data, data_format):
+    """Load and assign experiment attributes to dnplab attributes
+
+    Args:
+        data (dnpData): Data object
+        data_format (str): Format of spectrometer data to import
+
+    Returns:
+        data (dnpData): Data object
+
+    """
+    if data_format == None:
+        raise TypeError(
+            "No data format given and autodetect failed to detect format, please specify a format"
+        )
+
+    else:
+        dnplab_attrs_data_info = DNPLAB_CONFIG.getlist(
+            "DNPLAB_ATTRS_COMMON", "dnplab_attrs_data_info"
+        )
+        dnplab_attrs_data_info = [x.strip() for x in dnplab_attrs_data_info]
+        dnplab_attrs_label = DNPLAB_CONFIG.get(
+            "DNPLAB_ATTRS_COMMON", "dnplab_attrs_label", fallback="DNPLAB_ATTRS"
+        )
+        dnplab_attrs_label += ":" + data_format
+        for key, val in DNPLAB_CONFIG[dnplab_attrs_label].items():
+            if val != "None":
+                try:
+                    if key not in dnplab_attrs_data_info:
+                        params = _convert_dnplab_attrs(data, val)
+                    else:
+                        params = val
+                    data.dnplab_attrs[key] = params
+                except:
+                    continue
+        return data
+
+
+def _convert_dnplab_attrs(data, exp_key):
+    """Load and calculate the value assigned to dnplab attributes
+
+    Args:
+        data (dnpData): Data object
+        exp_key (str): A string of experiment attributes possibly with multiplication sign and unit
+
+    Returns:
+        new_params (int or float): dnplab attributes values
+    """
+    if "," in exp_key:
+        [params, unit] = exp_key.split(",")
+        scaling_factor = _scale_dnplab_attrs(unit)
+    else:
+        params = exp_key
+        scaling_factor = 1
+
+    params_list = params.split("*")
+    new_params = 1
+    for key in params_list:
+        params = data.attrs["".join(key.split())]
+        if isinstance(params, str):
+            try:
+                new_params *= int(re.findall("\d+", params)[0])
+            except:
+                new_params *= float(
+                    re.findall("[+-]?\d+\.\d+", params)[0]
+                )  # remove unexpected characters
+        else:
+            new_params *= params
+    return new_params * scaling_factor
+
+
+def _scale_dnplab_attrs(unit):
+    """Scale all dnplab attributes value to SI unit
+
+    Args:
+        unit (str): an unit
+
+    Returns:
+        scaling_factor (float): scaling factor
+    """
+    scaling_letter = unit.strip()[0]
+    if scaling_letter == "m":
+        scaling_letter = "mm"  # for configuration purpose
+    scaling_letter = scaling_letter.lower()
+    if scaling_letter not in list(DNPLAB_CONFIG["SI_SCALING"].keys()):
+        print("Unit is wrong, force scaling factor to 1")
+        scaling_factor = 1
+    else:
+        scaling_factor = DNPLAB_CONFIG.get("SI_SCALING", scaling_letter, fallback=None)
 
-    return spectrometer_format
+    return float(scaling_factor)
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/load_csv.py` & `dnplab-2.1.4/dnplab/io/load_csv.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/power.py` & `dnplab-2.1.4/dnplab/io/power.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/prospa.py` & `dnplab-2.1.4/dnplab/io/prospa.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             data_filename = filesList[0]
             filename, extension = os.path.splitext(os.path.split(data_filename)[-1])
     else:
         raise OSError("%s not found" % path)
 
     try:
         attrs = import_par(os.path.join(path, parameters_filename))
+
     except:
         warnings.warn("No parameters file in directory")
         attrs = {}
 
     if extension == ".csv":
         # Import csv data
         x, data = import_csv(os.path.join(path, filename + extension))
@@ -55,23 +56,22 @@
         nmr_frequency = attrs["b1Freq"]
         try:
             nmr_frequency = float(nmr_frequency)
         except:
             nmr_frequency = float(nmr_frequency.replace("d", ""))
 
         attrs["nmr_frequency"] = nmr_frequency * 1e6
+        attrs["spectrometer_format"] = "prospa"
+        attrs["experiment_type"] = "nmr_spectrum"
 
     # Assume direct dimension is 1st dimension
     data_shape = _np.shape(_np.squeeze(data))
 
     dims, coords = prospa_coords(attrs, data_shape, experiment=experiment)
 
-    # Assign data/spectrum type
-    attrs["experiment_type"] = "nmr_spectrum"
-
     kea_data = DNPData(data, dims, coords, attrs)
 
     return kea_data
 
 
 def import_nd(path):
     """Import Kea binary 1d, 2d, 3d, 4d files
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/random.py` & `dnplab-2.1.4/dnplab/io/random.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/save.py` & `dnplab-2.1.4/dnplab/io/save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/specman.py` & `dnplab-2.1.4/dnplab/io/specman.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/tnmr.py` & `dnplab-2.1.4/dnplab/io/tnmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/topspin.py` & `dnplab-2.1.4/dnplab/io/topspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,18 @@
 
     # Add NMR Frequency to attrs
     topspin_data.attrs["nmr_frequency"] = acqus_params["SFO1"] * 1e6
 
     # Assign data/spectrum type
     topspin_data.attrs["experiment_type"] = "nmr_spectrum"
 
+    # Assign number of scans
+    if "acqu2s" in dir_list:
+        topspin_data.attrs["scans"] = int(acqu2s_params["TD"])
+
     # reorder so that 't2' is first
     topspin_data.reorder(["t2"])
 
     return topspin_data
 
 
 # Load topspin should also handle this
```

### Comparing `dnplab-2.1.3rc2/dnplab/io/vna.py` & `dnplab-2.1.4/dnplab/io/vna.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/vnmrj.py` & `dnplab-2.1.4/dnplab/io/vnmrj.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/io/winepr.py` & `dnplab-2.1.4/dnplab/io/winepr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/math/lineshape.py` & `dnplab-2.1.4/dnplab/math/lineshape.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/math/relaxation.py` & `dnplab-2.1.4/dnplab/math/relaxation.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/math/window.py` & `dnplab-2.1.4/dnplab/math/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         x (array_like): Vector of points
         lw (int or float): linewidth
 
     Returns:
         array: exponential window function
 
     .. math::
-        f(x) =  e^{-2t * lw}
+        \mathrm{exponential} =  e^{-\pi * x * lw}
     """
     return _np.exp(-pi * (x - x[0]) * lw)
 
 
 def gaussian(x, lw):
     r"""Calculate gaussian window function
 
@@ -61,15 +61,15 @@
         x (array_like): vector of points
         N(int): number of points to return in window function
 
     Returns:
         ndarray: hann window function
 
     .. math::
-        \mathrm{han} = 0.5 + 0.5\cos(\pi * n / (N-1))
+        \mathrm{hann} = 0.5 + 0.5\cos(\pi * n / (N-1))
     """
     N = _handle_array(x)
 
     return 0.5 + 0.5 * _np.cos(1.0 * pi * _np.arange(N) / (N - 1))
 
 
 def traf(x, lw):
```

### Comparing `dnplab-2.1.3rc2/dnplab/plotting/general.py` & `dnplab-2.1.4/dnplab/plotting/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,24 @@
         warn("experiment_type is None, falling back to plot function")
         plot(data, *args, **kwargs)
         return
 
     _plt.grid(True)
     _plt.title(title)
 
+    fancyplot_possiblesections = list(DNPLAB_CONFIG.sections())
+    fancyplot_label = DNPLAB_CONFIG.get(
+        "PLOTTING", "fancyplot_label", fallback="FANCY_PLOT"
+    )
+    fancyplot_sections = [
+        k.strip(fancyplot_label).strip(":")
+        for k in fancyplot_possiblesections
+        if k.startswith(fancyplot_label)
+    ]
+
     if data.attrs["experiment_type"] == "nmr_spectrum":
         if "dim" in kwargs:
             dim = kwargs.pop("dim")
         else:
             dim = data.dims[0]
         coord = data.coords[dim]
         data.unfold(dim)
@@ -157,25 +167,15 @@
             parameterString = "Freq: " + str(round(data.attrs["nmr_frequency"], 4))
 
             box_style = dict(boxstyle="round", facecolor="white", alpha=0.25)
             xmin, xmax, ymin, ymax = _plt.axis()
 
             _plt.text(xmin * 0.95, ymax / 10, parameterString, bbox=box_style)
 
-    fancyplot_possiblesections = list(DNPLAB_CONFIG.sections())
-    fancyplot_label = DNPLAB_CONFIG.get(
-        "PLOTTING", "fancyplot_label", fallback="FANCY_PLOT"
-    )
-    fancyplot_sections = [
-        k.strip(fancyplot_label).strip(":")
-        for k in fancyplot_possiblesections
-        if k.startswith(fancyplot_label)
-    ]
-
-    if data.attrs["experiment_type"] in fancyplot_sections:
+    elif data.attrs["experiment_type"] in fancyplot_sections:
         exp_type = fancyplot_label + ":" + data.attrs["experiment_type"]
         get_key = lambda x, fallback=None: DNPLAB_CONFIG.get(
             exp_type, x, fallback=fallback
         )
         get_float_key = lambda x, fallback=1: DNPLAB_CONFIG.getfloat(
             exp_type, x, fallback=fallback
         )
```

### Comparing `dnplab-2.1.3rc2/dnplab/plotting/image.py` & `dnplab-2.1.4/dnplab/plotting/image.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/plotting/stack_plot.py` & `dnplab-2.1.4/dnplab/plotting/stack_plot.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/processing/apodization.py` & `dnplab-2.1.4/dnplab/processing/apodization.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,31 +59,38 @@
         \mathrm{traf}           &=  (f1 * (f1 + f2)) / (f1^{2} + f2^{2}) &
 
                f1(t)   &=  \exp(-t * \pi * \mathrm{linewidth[0]}) &
 
                f2(t)   &=  \exp((t - T) * \pi * \mathrm{linewidth[1]}) &
     """
 
-    data = data.copy()
+    out = data.copy()
 
-    coord = data.coords[dim]
-    index = data.index(dim)
+    index = out.index(dim)
+    coord = out.coords[dim]
 
+    kind = str(kind).lower()  # kind of apodization is a lower case string
+
+    if kind not in _windows:
+        raise ValueError(
+            'Window function "%s" not valid. Available window functions are: %s.  See documentation for more details.'
+            % (kind, list(_windows.keys()))
+        )
     window = _windows[kind]
     apwin = window(coord, **kwargs)
 
-    data_shape = data.shape
+    out_shape = out.shape
 
-    new_shape = [1 if ix != index else data_shape[index] for ix in range(data.ndim)]
+    new_shape = [1 if ix != index else out_shape[index] for ix in range(out.ndim)]
     apwin = _np.reshape(apwin, new_shape)
 
-    data *= apwin
+    out *= apwin
 
     proc_parameters = {
         "kind": kind,
     }
     for key in kwargs:
         proc_parameters[key] = kwargs[key]
     proc_attr_name = "window"
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/processing/conversion.py` & `dnplab-2.1.4/dnplab/processing/conversion.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/processing/helpers.py` & `dnplab-2.1.4/dnplab/processing/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
     Returns:
         enhancements (DNPData): Enhancement values
     """
 
     enhancements = data.copy()
 
+    proc_parameters = {
+        "off_spectrum_index": off_spectrum_index,
+        "return_complex_values": return_complex_values,
+    }
+
     if not "experiment_type" in data.attrs.keys():
         raise KeyError("Experiment type not defined")
 
     if data.attrs["experiment_type"] != "integrals":
         raise ValueError("dnpdata object does not contain integrals.")
 
     if data.dims[0] == "Power":
@@ -40,14 +45,17 @@
         print("This is a DNP enhancement profile. Not implemented yet.")
 
     else:
         raise TypeError(
             "Integration axis not recognized. First dimension should be Power or B0."
         )
 
+    proc_attr_name = "calculate_enhancement"
+    enhancements.add_proc_attrs(proc_attr_name, proc_parameters)
+
     if return_complex_values == True:
         return enhancements
 
     elif return_complex_values == False:
         return enhancements.real
 
 
@@ -201,20 +209,29 @@
         polyorder (int): Polynomial order to fit samples
 
     Returns:
         data (DNPData): Data with Savitzky-Golay smoothing applied
     """
     out = data.copy()
 
+    proc_parameters = {
+        "dim": dim,
+        "window_length": window_length,
+        "polyorder": polyorder,
+    }
+
     out.unfold(dim)
 
     out.values = savgol_filter(out.values, window_length, polyorder, axis=0)
 
     out.fold()
 
+    proc_attr_name = "smooth"
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
+
     return out
 
 
 def left_shift(data, dim="t2", shift_points=0):
     """Remove points from the left
 
     Args:
@@ -222,24 +239,26 @@
         dim (str): Name of dimension to left shift, default is "t2"
         shift_points (int): Number of points to left shift, default is 0.
 
     Returns:
         data (DNPDdata): Shifted data object
     """
 
-    data = data[dim, shift_points:]
+    out = data.copy()
+
+    out = out[dim, shift_points:]
 
     proc_attr_name = "left_shift"
     proc_parameters = {
         "dim": dim,
         "points": shift_points,
     }
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
 
 
 def normalize(data, amplitude=True):
     """Normalize spectrum
 
     Args:
         data (DNPData): Data object
@@ -275,12 +294,19 @@
         old_ref (float): Value of old reference
         new_ref (float): New reference value
 
     Returns:
         DNPData: referenced data
     """
 
-    data = data.copy()
+    out = data.copy()
+
+    out.coords[dim] -= old_ref - new_ref
 
-    data.coords[dim] -= old_ref - new_ref
+    proc_attr_name = "reference"
+    proc_parameters = {
+        "dim": dim,
+        "old_ref": old_ref,
+        "new_ref": new_ref,
+    }
 
-    return data
+    return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/processing/integration.py` & `dnplab-2.1.4/dnplab/processing/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,39 +30,38 @@
         >>> dnp.plot(data)
         >>> dnp.plot(data_int)
         >>> show()
 
 
     """
 
-    data = data.copy()
+    out = data.copy()
 
     if regions == None:
-        index = data.index(dim)
-        data.values = cumtrapz(data.values, data.coords[dim], axis=index, initial=0)
+        index = out.index(dim)
+        out.values = cumtrapz(out.values, out.coords[dim], axis=index, initial=0)
 
         proc_attr_name = "cumlative_integrate"
         proc_parameters = {
             "dim": dim,
             "regions": regions,
         }
-        data.add_proc_attrs(proc_attr_name, proc_parameters)
-        return data
+        out.add_proc_attrs(proc_attr_name, proc_parameters)
+        return out
 
     else:
         data_list = []
         for region in regions:
-            data_list.append(cumulative_integrate(data[dim, region], dim))
-
-        proc_attr_name = "cumlative_integrate"
-        proc_parameters = {
-            "dim": dim,
-            "regions": regions,
-        }
-        data.add_proc_attrs(proc_attr_name, proc_parameters)
+            proc_attr_name = "cumlative_integrate"
+            proc_parameters = {
+                "dim": dim,
+                "regions": regions,
+            }
+            out.add_proc_attrs(proc_attr_name, proc_parameters)
+            data_list.append(cumulative_integrate(out[dim, region], dim))
 
         return data_list
 
 
 def integrate(data, dim="f2", regions=None):
     """Integrate data along given dimension. If no region is given, the integral is calculated over the entire range.
 
@@ -84,41 +83,41 @@
             >>> data = dnp.integrate(data, regions=[(4, 5)])
 
         Integrate two regions:
 
             >>> data = dnp.integrate(data, regions=[(1.1, 2.1), (4.5, 4.9)])
 
     """
-    data = data.copy()
-    data.attrs["experiment_type"] = "integrals"
+    out = data.copy()
+    out.attrs["experiment_type"] = "integrals"
 
-    index = data.index(dim)
+    index = out.index(dim)
     if regions == None:
-        data.values = _np.trapz(data.values, data.coords[dim], axis=index)
-        data.coords.pop(dim)
+        out.values = _np.trapz(out.values, out.coords[dim], axis=index)
+        out.coords.pop(dim)
 
         # if error_regions == None:
-        #     data.error = np.zeros(data.shape)
+        #     out.error = np.zeros(out.shape)
         #     print("add errors")
 
         # else:
-        #     signal = max(data.values)
-        #     noise = np.trapz(data.)
+        #     signal = max(out.values)
+        #     noise = np.trapz(out.)
 
     else:
         data_list = []
         for region in regions:
-            data_list.append(integrate(data[dim, region], dim))
+            data_list.append(integrate(out[dim, region], dim))
 
         x = _np.array(list(range(len(data_list))))
         dim_name = "integrals"
-        data = concat(data_list, dim_name, coord=x)
+        out = concat(data_list, dim_name, coord=x)
 
     proc_attr_name = "integrate"
     proc_parameters = {
         "dim": dim,
         "regions": regions,
     }
 
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/processing/offset.py` & `dnplab-2.1.4/dnplab/processing/offset.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 
         0th-order background removal (DC offset)
 
         >>> data = dnp.remove_background(data)
 
     """
 
+    out = data.copy()
+
     proc_parameters = {
         "dim": dim,
         "deg": deg,
         "regions": regions,
     }
 
-    fit = background(data, dim=dim, deg=deg, regions=regions)
-    data = data - fit
+    fit = background(out, dim=dim, deg=deg, regions=regions)
+    out = out - fit
 
     proc_attr_name = "remove_background"
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
 
 
 def background(data, dim="t2", deg=0, regions=None):
     """Remove background from data
 
     Args:
         data (DNPData): Data object
@@ -46,14 +48,21 @@
         regions (None, list): Background regions, by default entire region is background corrected. Regions can be specified as a list of tuples [(min, max), ...]
 
     Returns:
         DNPData: Background fit
     """
 
     out = data.copy()
+
+    proc_parameters = {
+        "dim": dim,
+        "deg": deg,
+        "regions": regions,
+    }
+
     out.unfold(dim)
 
     coord = out.coords[dim]
 
     if regions == None:
         fit_points = [True for x in coord]
     else:
@@ -67,8 +76,11 @@
     for ix in range(out.shape[1]):
         p = _np.polyfit(coord[fit_points], out.values[:, ix][fit_points], deg=deg)
         fit = _np.polyval(p, coord)
         out.values[:, ix] = fit
 
     out.fold()
 
+    proc_attr_name = "background"
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
+
     return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/processing/phase.py` & `dnplab-2.1.4/dnplab/processing/phase.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,52 +45,52 @@
 
         phased\_real          &= \mathrm{data.real} * \exp(-1j * \mathrm{phase}) &
 
         phased\_imag          &= \mathrm{data.imag} * \exp(-1j * \mathrm{phase}) &
 
     """
 
-    data = data.copy()
+    out = data.copy()
     if reference_slice == 0:
         raise ValueError(
             "please use indices from 1 to number of slices, i.e. use 1 instead of 0"
         )
 
-    shape_data = _np.shape(data.values)
-    index = data.dims.index(dim)
+    shape_data = _np.shape(out.values)
+    index = out.dims.index(dim)
 
     if phase is not None:
         method = "manual"
 
     if method == "manual":
         if order == "zero" and isinstance(phase, (int, float)):
-            data.attrs["phase0"] = phase
+            out.attrs["phase0"] = phase
         elif order == "zero" and not isinstance(phase, (int, float)):
             raise ValueError(
                 "for a zero order phase correction you must supply a single phase"
             )
         elif order == "first" and isinstance(phase, (int, float)):
-            data.attrs["phase0"] = phase
+            out.attrs["phase0"] = phase
             order = "zero"
             warn(
                 "method=manual and order=first but only a single phase was given, switching to order=zero"
             )
         elif (
             order == "first"
             and isinstance(phase, (list, _np.ndarray))
             and len(phase) == shape_data[index]
         ):
-            data.attrs["phase1"] = _np.array(phase)
+            out.attrs["phase1"] = _np.array(phase)
         else:
             raise ValueError(
                 "Invalid combination of phase order and phase value(s). Supply float for zero order, array or list for first order"
             )
     else:
         if isinstance(reference_range, (list, tuple)) and len(reference_range) == 2:
-            check_data = data[dim, (reference_range[0], reference_range[1])]
+            check_data = out[dim, (reference_range[0], reference_range[1])]
         else:
             check_data = data.copy()
             if reference_range is not None:
                 warn("reference_range must be None or list/tuple length=2")
 
         if reference_slice is not None:
             if len(shape_data) == 1:
@@ -99,15 +99,15 @@
                 warn("ignoring reference_slice, this is 1D data")
             else:
                 temp_data = check_data.values[:, reference_slice - 1]
         else:
             temp_data = check_data.values
 
         if method == "arctan":
-            data.attrs["phase0"] = _np.arctan(
+            out.attrs["phase0"] = _np.arctan(
                 _np.sum(_np.imag(temp_data.reshape(-1, 1)))
                 / _np.sum(_np.real(temp_data.reshape(-1, 1)))
             )
         elif method == "search":
             if pts_lim is not None:
                 if len(check_data.coords[dim]) > pts_lim:
                     phasing_x = _np.linspace(
@@ -116,16 +116,16 @@
                         int(pts_lim),
                     ).reshape(-1)
                     if len(check_data.dims) == 1:
                         temp_data = _np.interp(
                             phasing_x, check_data.coords[dim], check_data.values
                         ).reshape(-1)
                     else:
-                        ind_dim = list(set(data.dims) - set([dim]))[0]
-                        ind_shape = data.shape[data.index(ind_dim)]
+                        ind_dim = list(set(out.dims) - set([dim]))[0]
+                        ind_shape = out.shape[out.index(ind_dim)]
                         temp_data = _np.array(
                             [
                                 _np.interp(
                                     phasing_x,
                                     check_data.coords[dim],
                                     check_data[dim, :].values[:, indx],
                                 ).reshape(-1)
@@ -133,89 +133,89 @@
                             ]
                         ).reshape(pts_lim, ind_shape)
             phases_0 = _np.linspace(-pi / 2, pi / 2, 180).reshape(-1)
             rotated_data = (temp_data.reshape(-1, 1)) * _np.exp(-1j * phases_0)
             real_imag_ratio = (_np.real(rotated_data) ** 2).sum(axis=0) / (
                 (_np.imag(rotated_data) ** 2).sum(axis=0)
             )
-            data.attrs["phase0"] = phases_0[_np.argmax(real_imag_ratio)]
+            out.attrs["phase0"] = phases_0[_np.argmax(real_imag_ratio)]
         else:
             raise TypeError("Invalid autophase method")
 
     if order == "zero":
-        data.values *= _np.exp(-1j * data.attrs["phase0"])
+        out.values *= _np.exp(-1j * out.attrs["phase0"])
     elif order == "first":
         if method == "manual":
-            data.attrs["phase1"] = phase
+            out.attrs["phase1"] = phase
         else:
-            pivot_ratio = pivot / len(data.values)
-            data.attrs["phase1"] = _np.linspace(
-                data.attrs["phase0"] - delta * pivot_ratio,
-                data.attrs["phase0"] + delta * (1 - pivot_ratio),
-                len(data.values),
+            pivot_ratio = pivot / len(out.values)
+            out.attrs["phase1"] = _np.linspace(
+                out.attrs["phase0"] - delta * pivot_ratio,
+                out.attrs["phase0"] + delta * (1 - pivot_ratio),
+                len(out.values),
             )
-        data.values.T.dot(_np.exp(-1j * data.attrs["phase1"]))
+        out.values.T.dot(_np.exp(-1j * out.attrs["phase1"]))
 
     else:
         raise TypeError("Invalid order or order & phase pair")
 
     if force_positive:
-        if _np.sum(data.values) < 0:
-            data.values *= -1
+        if _np.sum(out.values) < 0:
+            out.values *= -1
 
     proc_parameters = {
         "method": method,
         "reference_range": reference_range,
         "reference_slice": reference_slice,
         "force_positive": force_positive,
         "order": order,
         "pivot": pivot,
         "delta": delta,
     }
     proc_attr_name = "autophase"
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
 
 
 def phase_cycle(data, dim, receiver_phase):
     """Apply phase cycle to data
 
     Args:
         all_data (dnpdata_collection, dnpdata): data to process
         dim (str): dimension to perform phase cycle
         receiver_phase (numpy.array, list): Receiver Phase 0 (x), 1 (y), 2 (-x), 3 (-y)
 
     Returns:
         dnpdata: data object after phase cycle applied
     """
 
-    data = data.copy()
+    out = data.copy()
 
-    if dim not in data.dims:
+    if dim not in out.dims:
         raise ValueError("dim not in dims")
 
-    coord = data.coords[dim]
+    coord = out.coords[dim]
     receiver_phase = _np.array(receiver_phase).ravel()
 
     proc_parameters = {"dim": dim, "receiver_phase": receiver_phase}
 
     receiver_phase = _np.tile(receiver_phase, int(coord.size / receiver_phase.size))
 
-    index = data.dims.index(dim)
+    index = out.dims.index(dim)
 
-    reshape_size = [1 for k in data.dims]
-    reshape_size[index] = len(data.coords[dim])
+    reshape_size = [1 for k in out.dims]
+    reshape_size[index] = len(out.coords[dim])
 
-    data *= _np.exp(-1j * (pi / 2.0) * receiver_phase.reshape(reshape_size))
+    out *= _np.exp(-1j * (pi / 2.0) * receiver_phase.reshape(reshape_size))
 
     proc_attr_name = "phasecycle"
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
-    return data
+    return out
 
 
 def phase(data, dim="f2", p0=0.0, p1=0.0, pivot=None):
     """Apply phase correction to DNPData object
 
     Args:
         data (DNPData): Data object to phase
@@ -265,10 +265,10 @@
     proc_parameters = {
         "p0": p0,
         "p1": p1,
         "pivot": pivot,
     }
 
     proc_attr_name = "phase_correction"
-    data.add_proc_attrs(proc_attr_name, proc_parameters)
+    out.add_proc_attrs(proc_attr_name, proc_parameters)
 
     return out
```

### Comparing `dnplab-2.1.3rc2/dnplab/widgets/align_widget.py` & `dnplab-2.1.4/dnplab/widgets/align_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab/widgets/phase_widget.py` & `dnplab-2.1.4/dnplab/widgets/phase_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/dnplab.egg-info/PKG-INFO` & `dnplab-2.1.4/dnplab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.3rc2
+Version: 2.1.4
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.3rc2/dnplab.egg-info/SOURCES.txt` & `dnplab-2.1.4/dnplab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 dnplab.egg-info/dependency_links.txt
 dnplab.egg-info/requires.txt
 dnplab.egg-info/top_level.txt
 dnplab/analysis/__init__.py
 dnplab/analysis/hydration.py
 dnplab/analysis/relaxation_fit.py
 dnplab/analysis/simulate_enhancement_profiles.py
+dnplab/config/__init__.py
+dnplab/config/config.py
 dnplab/config/dnplab.cfg
 dnplab/constants/__init__.py
 dnplab/constants/constants.py
 dnplab/constants/mrProperties.py
 dnplab/constants/radicalProperties.py
 dnplab/core/__init__.py
 dnplab/core/base.py
@@ -49,14 +51,15 @@
 dnplab/plotting/__init__.py
 dnplab/plotting/general.py
 dnplab/plotting/image.py
 dnplab/plotting/stack_plot.py
 dnplab/processing/__init__.py
 dnplab/processing/align.py
 dnplab/processing/apodization.py
+dnplab/processing/average.py
 dnplab/processing/conversion.py
 dnplab/processing/fft.py
 dnplab/processing/helpers.py
 dnplab/processing/integration.py
 dnplab/processing/offset.py
 dnplab/processing/phase.py
 dnplab/reporting/__init__.py
```

### Comparing `dnplab-2.1.3rc2/setup.py` & `dnplab-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_data_class.py` & `dnplab-2.1.4/unittests/test_data_class.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_dnp_nmr.py` & `dnplab-2.1.4/unittests/test_dnp_nmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_dnp_tools.py` & `dnplab-2.1.4/unittests/test_dnp_tools.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_general_fit.py` & `dnplab-2.1.4/unittests/test_general_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_hydration.py` & `dnplab-2.1.4/unittests/test_hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_io.py` & `dnplab-2.1.4/unittests/test_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 
 class import_topspin_tester(unittest.TestCase):
     def setUp(self):
         self.testdata = os.path.join(".", "data", "topspin")
 
     def test_import_topspin_exp1_is_fid(self):
-        data = dnp.load(os.path.join(self.testdata, str(1)), data_type="topspin")
+        data = dnp.load(os.path.join(self.testdata, str(1)), data_format="topspin")
         self.assertEqual(data.dims[0], "t2")
         self.assertEqual(data.values.size, 8148)
         self.assertAlmostEqual(data.attrs["nmr_frequency"], 14831413.270000001)
 
     def test_import_topspin_exp5_is_2d_phcyc(self):
-        data = dnp.load(os.path.join(self.testdata, str(5)), data_type="topspin")
+        data = dnp.load(os.path.join(self.testdata, str(5)), data_format="topspin")
         self.assertEqual(data.values.shape[0], 11913)
         self.assertEqual(data.dims, ["t2", "t1"])
         self.assertAlmostEqual(data.attrs["nmr_frequency"], 14831413.270000001)
 
     def test_import_topspin_exp28_is_2d(self):
-        data = dnp.load(os.path.join(self.testdata, str(28)), data_type="topspin")
+        data = dnp.load(os.path.join(self.testdata, str(28)), data_format="topspin")
         self.assertEqual(data.values.shape, (7923, 8))
         self.assertEqual(data.dims, ["t2", "t1"])
         self.assertAlmostEqual(data.attrs["nmr_frequency"], 14831413.270000001)
 
     def test_import_topspin_jcamp_dx(self):
         attrs = dnp.io.topspin.load_topspin_jcamp_dx(
             os.path.join(self.testdata, "1", "acqus")
@@ -40,15 +40,15 @@
     def setUp(self):
         self.test_data = os.path.join(".", "data", "prospa", "toluene_10mM_Tempone")
 
     def test_import_prospa_exp_is_1d(self):
         datas = [
             dnp.load(
                 os.path.join(self.test_data, "%i" % expNum, "data.csv"),
-                data_type="prospa",
+                data_format="prospa",
             )
             for expNum in [1, 21, 42]
         ]
         for i, data in enumerate(datas):
             self.assertEqual(data.values.shape, (16384,))
             self.assertEqual(data.dims, ["t2"])
             self.assertAlmostEqual(data.attrs["nmr_frequency"], 14244500.0)
@@ -68,130 +68,130 @@
             for s in [
                 "10mM_tempol_in_water_mw_40dBm.fid",
                 "10mM_tempol_in_water_mw_off.fid",
             ]
         ]
 
     def test_import_vnmrj_1d(self):
-        datas = [dnp.load(path=path, data_type="vnmrj") for path in self.test_data1Ds]
+        datas = [dnp.load(path=path, data_format="vnmrj") for path in self.test_data1Ds]
         for i, data in enumerate(datas):
             self.assertEqual(data.values.shape, (131072,))
             self.assertEqual(
                 data.dims,
                 [
                     "t2",
                 ],
             )
             self.assertAlmostEqual(data.attrs["nmr_frequency"], 14244283.4231)
         self.assertAlmostEqual(datas[0].values[365], (-20378767 + 2734659j))
         self.assertAlmostEqual(datas[1].values[365], (-950662 - 138458j))
 
     def test_import_vnmrj_2d(self):
-        datas = [dnp.load(path=path, data_type="vnmrj") for path in self.test_data2Ds]
+        datas = [dnp.load(path=path, data_format="vnmrj") for path in self.test_data2Ds]
         for i, data in enumerate(datas):
             self.assertEqual(data.values.shape, (131072, 5))
             self.assertEqual(data.dims, ["t2", "t1"])
             self.assertAlmostEqual(data.attrs["nmr_frequency"], 14244283.4231)
         self.assertAlmostEqual(datas[0].values[365, 3], (-1263136 - 1063328.5j))
 
 
 # class specman_import_tester(unittest.TestCase):
 #     def setUp(self):
 #         self.test_data_2D = os.path.join(".", "data", "specman", "test_specman2D.exp")
 #         self.test_data_4D = os.path.join(".", "data", "specman", "test_specman4D.d01")
 
 #     def test_import_specman_2D(self):
-#         data = dnp.load(self.test_data_2D, data_type="specman")
+#         data = dnp.load(self.test_data_2D, data_format="specman")
 #         self.assertEqual(data.dims, ["t2", "t1"])
 #         self.assertEqual(data.values.shape, (1500, 80))
 
 #     def test_import_specman_4D(self):
-#         data = dnp.load(self.test_data_4D, data_type="specman")
+#         data = dnp.load(self.test_data_4D, data_format="specman")
 #         self.assertEqual(data.dims, ["t2", "t1", "t0", "t"])
 #         self.assertEqual(data.values.shape, (1500, 40, 5, 3))
 
 
 class bes3t_import_tester(unittest.TestCase):
     def setUp(self):
         self.test_data_HYSCORE = os.path.join(".", "data", "bes3t", "HYSCORE.DSC")
         self.test_data_DEER = os.path.join(".", "data", "bes3t", "DEER.DSC")
         self.test_data_ESE = os.path.join(".", "data", "bes3t", "2D_ESE.DTA")
         self.test_data_1D = os.path.join(".", "data", "bes3t", "1D_CW.DTA")
         self.test_data_2D = os.path.join(".", "data", "bes3t", "2D_CW.YGF")
 
     def test_import_bes3t_HYSCORE(self):
-        data = dnp.load(self.test_data_HYSCORE, data_type="xepr")
+        data = dnp.load(self.test_data_HYSCORE, data_format="xepr")
         self.assertEqual(data.dims, ["t2", "t1"])
         self.assertEqual(data.values.shape, (175, 175))
         self.assertEqual(max(data.coords["t2"]), 3520.0)
         self.assertEqual(max(data.coords["t1"]), 3520.0)
 
     def test_import_bes3t_DEER(self):
-        data = dnp.load(self.test_data_DEER, data_type="xepr")
+        data = dnp.load(self.test_data_DEER, data_format="xepr")
         self.assertEqual(data.dims, ["t2"])
         self.assertEqual(data.values.shape, (504,))
         self.assertEqual(data.attrs["frequency"], 33.85)
 
     def test_import_bes3t_ESE(self):
-        data = dnp.load(self.test_data_ESE, data_type="xepr")
+        data = dnp.load(self.test_data_ESE, data_format="xepr")
         self.assertEqual(data.dims, ["t2", "t1"])
         self.assertEqual(data.values.shape, (512, 50))
         self.assertEqual(data.attrs["frequency"], 9.296)
 
     def test_import_bes3t_1D(self):
-        data = dnp.load(self.test_data_1D, data_type="xenon")
+        data = dnp.load(self.test_data_1D, data_format="xenon")
         self.assertEqual(data.dims, ["B0"])
         self.assertEqual(data.values.shape, (2250,))
         self.assertEqual(data.attrs["frequency"], 9.804448)
 
     def test_import_bes3t_2D(self):
-        data = dnp.load(self.test_data_2D, data_type="xenon")
+        data = dnp.load(self.test_data_2D, data_format="xenon")
         self.assertEqual(data.dims, ["B0", "t1"])
         self.assertEqual(data.values.shape, (1600, 100))
         self.assertEqual(data.attrs["frequency"], 9.627213)
 
 
 class winepr_import_tester(unittest.TestCase):
     def setUp(self):
         self.test_data_ESP = os.path.join(".", "data", "parspc", "ExampleESP.par")
         self.test_data_1D = os.path.join(".", "data", "parspc", "Example1D.spc")
         self.test_data_2D = os.path.join(".", "data", "parspc", "Example2D.spc")
 
     def test_import_winepr_ESP(self):
-        data = dnp.load(self.test_data_ESP, data_type="esp")
+        data = dnp.load(self.test_data_ESP, data_format="esp")
         self.assertEqual(data.dims, ["t2"])
         self.assertEqual(data.values.shape, (1024,))
         self.assertEqual(data.attrs["conversion_time"], 81.92)
 
     def test_import_winepr_1D(self):
-        data = dnp.load(self.test_data_1D, data_type="winepr")
+        data = dnp.load(self.test_data_1D, data_format="winepr")
         self.assertEqual(data.dims, ["B0"])
         self.assertEqual(data.values.shape, (512,))
         self.assertEqual(data.attrs["temperature"], 294.2)
 
     def test_import_winepr_2D(self):
-        data = dnp.load(self.test_data_2D, data_type="winepr")
+        data = dnp.load(self.test_data_2D, data_format="winepr")
         self.assertEqual(data.dims, ["B0", "t1"])
         self.assertEqual(data.values.shape, (1024, 15))
         self.assertEqual(data.attrs["frequency"], 9.79)
 
 
 class delta_import_tester(unittest.TestCase):
     def setUp(self):
         self.test_data_1D = os.path.join(".", "data", "delta", "50percCHCL3.jdf")
         self.test_data_2D = os.path.join(".", "data", "delta", "lineshape_drift.jdf")
 
     def test_import_delta_1D(self):
-        data = dnp.load(self.test_data_1D, data_type="delta")
+        data = dnp.load(self.test_data_1D, data_format="delta")
         self.assertEqual(data.dims, ["t2"])
         self.assertEqual(data.values.shape, (16384,))
         self.assertEqual(max(data.coords["t2"]), 0.262128)
 
     def test_import_delta_2D(self):
-        data = dnp.load(self.test_data_2D, data_type="delta")
+        data = dnp.load(self.test_data_2D, data_format="delta")
         self.assertEqual(data.dims, ["t2", "t1"])
         self.assertEqual(data.values.shape, (8192, 256))
         self.assertEqual(max(data.coords["t2"]), 0.5451929600000001)
         self.assertEqual(max(data.coords["t1"]), 11.953125)
 
 
 class csv_import_tester(unittest.TestCase):
```

### Comparing `dnplab-2.1.3rc2/unittests/test_load.py` & `dnplab-2.1.4/unittests/test_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,29 @@
             "./data/prospa/toluene_10mM_Tempone/9/data.1d",
             "./data/prospa/toluene_10mM_Tempone/10/data.1d",
         ]
         self.list_index = range(10)
         self.dim_name = "test_dim"
 
     def test_topspin(self):
-        data = dnp.load(os.path.join(self.topspin_dir, str(1)), data_type="topspin")
+        data = dnp.load(os.path.join(self.topspin_dir, str(1)), data_format="topspin")
         self.assertEqual(data.dims[0], "t2")
         self.assertEqual(data.values.size, 8148)
         self.assertAlmostEqual(data.attrs["nmr_frequency"], 14831413.270000001)
 
     def test_prospa(self):
-        dnp.load(os.path.join(self.prospa_dir, str(1), "data.csv"), data_type="prospa")
+        dnp.load(os.path.join(self.prospa_dir, str(1), "data.csv"), data_format="prospa")
 
     def test_vnmrj(self):
-        dnp.load(self.vnmrj_dir, data_type="vnmrj")
+        dnp.load(self.vnmrj_dir, data_format="vnmrj")
 
     def test_import_list(self):
         dnp.load(
             self.list_prospa_dir,
-            data_type="prospa",
+            data_format="prospa",
             dim=self.dim_name,
             coord=self.list_index,
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dnplab-2.1.3rc2/unittests/test_nddata_core.py` & `dnplab-2.1.4/unittests/test_nddata_core.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/test_save.py` & `dnplab-2.1.4/unittests/test_save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.3rc2/unittests/testing.py` & `dnplab-2.1.4/unittests/testing.py`

 * *Files identical despite different names*

