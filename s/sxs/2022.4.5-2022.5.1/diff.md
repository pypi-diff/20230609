# Comparing `tmp/sxs-2022.4.5.tar.gz` & `tmp/sxs-2022.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sxs-2022.4.5.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sxs-2022.4.5.tar` & `sxs-2022.5.1.tar`

### file list

```diff
@@ -1,85 +1,111 @@
--rw-r--r--   0        0        0     1080 2023-04-06 18:08:28.821729 sxs-2022.4.5/LICENSE
--rw-r--r--   0        0        0     5785 2023-04-06 18:08:28.821729 sxs-2022.4.5/README.md
--rw-r--r--   0        0        0     2653 2023-04-06 18:10:11.986228 sxs-2022.4.5/pyproject.toml
--rw-r--r--   0        0        0     2337 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/__init__.py
--rw-r--r--   0        0        0    14761 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/caltechdata/__init__.py
--rw-r--r--   0        0        0     4914 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/caltechdata/catalog.py
--rw-r--r--   0        0        0    21546 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/caltechdata/login.py
--rw-r--r--   0        0        0      205 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/catalog/__init__.py
--rw-r--r--   0        0        0    26481 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/catalog/catalog.py
--rw-r--r--   0        0        0     4734 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/catalog/create.py
--rw-r--r--   0        0        0    10830 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/catalog/description.py
--rw-r--r--   0        0        0    11405 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/handlers.py
--rw-r--r--   0        0        0    16277 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/horizons/__init__.py
--rw-r--r--   0        0        0     3642 2023-04-06 18:08:28.821729 sxs-2022.4.5/sxs/horizons/spec_horizons_h5.py
--rw-r--r--   0        0        0     6536 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/horizons/xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0      149 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/metadata/__init__.py
--rw-r--r--   0        0        0    27679 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/metadata/metadata.py
--rw-r--r--   0        0        0    25867 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/time_series.py
--rw-r--r--   0        0        0     4280 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/__init__.py
--rw-r--r--   0        0        0    13205 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/bitwise.py
--rw-r--r--   0        0        0     1336 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/decimation/__init__.py
--rw-r--r--   0        0        0     4335 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/decimation/greedy_spline.py
--rw-r--r--   0        0        0     5357 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/decimation/linear_bisection.py
--rw-r--r--   0        0        0     6272 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/decimation/peak_greed.py
--rw-r--r--   0        0        0     1881 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/decimation/suppression.py
--rw-r--r--   0        0        0      695 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/dicts.py
--rw-r--r--   0        0        0     4488 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/downloads.py
--rw-r--r--   0        0        0     4517 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/files.py
--rw-r--r--   0        0        0     2620 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/formats.py
--rw-r--r--   0        0        0     8431 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/inspire.py
--rw-r--r--   0        0        0     1085 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/__init__.py
--rw-r--r--   0        0        0    12386 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/comparisons.py
--rw-r--r--   0        0        0    10447 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/conversion.py
--rw-r--r--   0        0        0     3732 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/dataset.py
--rw-r--r--   0        0        0    10447 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/horizons.py
--rw-r--r--   0        0        0    12385 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/metadata.py
--rw-r--r--   0        0        0     2799 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/waveform_amp_phase.py
--rw-r--r--   0        0        0     1929 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/lvcnr/waveforms.py
--rw-r--r--   0        0        0      812 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/monotonicity.py
--rw-r--r--   0        0        0     1473 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/pretty_print.py
--rw-r--r--   0        0        0      391 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/__init__.py
--rw-r--r--   0        0        0     8591 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/ads.py
--rw-r--r--   0        0        0     4264 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/arxiv.py
--rw-r--r--   0        0        0     1657 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/fairchild_report.py
--rw-r--r--   0        0        0     8431 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/inspire.py
--rw-r--r--   0        0        0    31018 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/journal_abbreviations.py
--rw-r--r--   0        0        0      418 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/references/references.py
--rw-r--r--   0        0        0     6727 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/select.py
--rw-r--r--   0        0        0     9676 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/sxs_directories.py
--rw-r--r--   0        0        0     3026 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/sxs_identifiers.py
--rw-r--r--   0        0        0     1850 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/utilities/url.py
--rw-r--r--   0        0        0      962 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/__init__.py
--rw-r--r--   0        0        0    12394 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/alignment.py
--rw-r--r--   0        0        0      126 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/corotating_paired_xor.py
--rw-r--r--   0        0        0     7763 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/memory.py
--rw-r--r--   0        0        0     5253 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/mode_utilities.py
--rw-r--r--   0        0        0    20427 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/nrar.py
--rw-r--r--   0        0        0    24057 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py
--rw-r--r--   0        0        0     2345 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     9124 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/transformations.py
--rw-r--r--   0        0        0      180 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/waveform_grid.py
--rw-r--r--   0        0        0     1299 2023-04-06 18:08:28.825729 sxs-2022.4.5/sxs/waveforms/waveform_mixin.py
--rw-r--r--   0        0        0    44544 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/waveforms/waveform_modes.py
--rw-r--r--   0        0        0      182 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/waveforms/waveform_signal.py
--rw-r--r--   0        0        0    25890 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/__init__.py
--rw-r--r--   0        0        0      217 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/api/__init__.py
--rw-r--r--   0        0        0    36877 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/api/deposit.py
--rw-r--r--   0        0        0    18007 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/api/login.py
--rw-r--r--   0        0        0     3689 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/api/records.py
--rw-r--r--   0        0        0    28737 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/catalog.py
--rw-r--r--   0        0        0     2573 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/creators.py
--rw-r--r--   0        0        0     4491 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/simannex.py
--rw-r--r--   0        0        0     8381 2023-04-06 18:08:28.829729 sxs-2022.4.5/sxs/zenodo/surrogatemodeling.py
--rw-r--r--   0        0        0        1 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/__init__.py
--rw-r--r--   0        0        0     9174 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/conftest.py
--rw-r--r--   0        0        0     1462 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_catalog.py
--rw-r--r--   0        0        0     2098 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_horizons.py
--rw-r--r--   0        0        0     3135 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_loader.py
--rw-r--r--   0        0        0     1097 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_metadata.py
--rw-r--r--   0        0        0    13883 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_time_series.py
--rw-r--r--   0        0        0     1515 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_transformations.py
--rw-r--r--   0        0        0    10703 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_utilities.py
--rw-r--r--   0        0        0     7016 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_waveform_rotations.py
--rw-r--r--   0        0        0    11516 2023-04-06 18:08:28.829729 sxs-2022.4.5/tests/test_waveforms.py
--rw-r--r--   0        0        0     8468 1970-01-01 00:00:00.000000 sxs-2022.4.5/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2022.5.1/.codecov.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2022.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2022.5.1/CITATION.cff
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 sxs-2022.5.1/mkdocs.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2022.5.1/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sxs-2022.5.1/.github/scripts/parse_version.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 sxs-2022.5.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2022.5.1/.github/workflows/pr_rtd_link.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/mathematica.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/api/catalog.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/api/horizons.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/api/metadata.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/api/time_series.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/api/waveforms.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/html/main.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/javascript/mathjax.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/tutorials/00-Introduction.ipynb
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/tutorials/01-Metadata.ipynb
+-rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/tutorials/02-Catalog.ipynb
+-rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/tutorials/03-Horizons.ipynb
+-rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2022.5.1/docs/tutorials/04-Waveforms.ipynb
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/__version__.py
+-rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/handlers.py
+-rw-r--r--   0        0        0    26032 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/time_series.py
+-rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/caltechdata/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/caltechdata/catalog.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/caltechdata/login.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/catalog/__init__.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/catalog/catalog.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/catalog/create.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/catalog/description.py
+-rw-r--r--   0        0        0    16277 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/horizons/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/horizons/spec_horizons_h5.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/horizons/xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/metadata/__init__.py
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/metadata/metadata.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/__init__.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/bitwise.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/dicts.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/downloads.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/files.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/formats.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/inspire.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/monotonicity.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/pretty_print.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/select.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/sxs_directories.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/sxs_identifiers.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/url.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/decimation/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/decimation/greedy_spline.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/decimation/linear_bisection.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/decimation/peak_greed.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/decimation/suppression.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/__init__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/comparisons.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/conversion.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/dataset.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/horizons.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/metadata.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/waveform_amp_phase.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/lvcnr/waveforms.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/ads.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/arxiv.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/fairchild_report.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/inspire.py
+-rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/journal_abbreviations.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/utilities/references/references.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/__init__.py
+-rw-r--r--   0        0        0    12399 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/alignment.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/corotating_paired_xor.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/memory.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/mode_utilities.py
+-rw-r--r--   0        0        0    20427 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/nrar.py
+-rw-r--r--   0        0        0    24896 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/transformations.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/waveform_grid.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/waveform_mixin.py
+-rw-r--r--   0        0        0    44733 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/waveform_modes.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/waveforms/waveform_signal.py
+-rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/__init__.py
+-rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/catalog.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/creators.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/simannex.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/surrogatemodeling.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/api/__init__.py
+-rw-r--r--   0        0        0    36877 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/api/deposit.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/api/login.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2022.5.1/sxs/zenodo/api/records.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     9174 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_catalog.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_horizons.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_loader.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_metadata.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_time_series.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_transformations.py
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_waveform_rotations.py
+-rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 sxs-2022.5.1/tests/test_waveforms.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 sxs-2022.5.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2022.5.1/LICENSE
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 sxs-2022.5.1/README.md
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sxs-2022.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 sxs-2022.5.1/PKG-INFO
```

### Comparing `sxs-2022.4.5/LICENSE` & `sxs-2022.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/README.md` & `sxs-2022.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Documentation Status](https://readthedocs.org/projects/sxs/badge/?version=main)](https://sxs.readthedocs.io/en/main/?badge=main)
 [![PyPI Version](https://img.shields.io/pypi/v/sxs?color=)](https://pypi.org/project/sxs/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sxs.svg?color=)](https://anaconda.org/conda-forge/sxs)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sxs-collaboration/sxs/blob/main/LICENSE)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/moble/sxs_notebooks/master)
 
 
-# Simulating eXtreme Spacetimes python package
+# Simulating eXtreme Spacetimes package
 
 The `sxs` python package provides a high-level interface for using data
 produced by the SXS collaboration.  In particular, the function `sxs.load` can
 automatically find, download, and load data, returning objects that provide
 common interfaces to the various types of data, without forcing the user to
 worry about details like data formats or where to find the data.  It can also
 automatically select the newest or highest-resolution dataset for a given
```

### Comparing `sxs-2022.4.5/sxs/__init__.py` & `sxs-2022.5.1/sxs/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/caltechdata/__init__.py` & `sxs-2022.5.1/sxs/caltechdata/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/caltechdata/catalog.py` & `sxs-2022.5.1/sxs/caltechdata/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/caltechdata/login.py` & `sxs-2022.5.1/sxs/caltechdata/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/catalog/catalog.py` & `sxs-2022.5.1/sxs/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/catalog/create.py` & `sxs-2022.5.1/sxs/catalog/create.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/catalog/description.py` & `sxs-2022.5.1/sxs/catalog/description.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/handlers.py` & `sxs-2022.5.1/sxs/handlers.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/horizons/__init__.py` & `sxs-2022.5.1/sxs/horizons/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/horizons/spec_horizons_h5.py` & `sxs-2022.5.1/sxs/horizons/spec_horizons_h5.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/horizons/xor_multishuffle_bzip2.py` & `sxs-2022.5.1/sxs/horizons/xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/metadata/metadata.py` & `sxs-2022.5.1/sxs/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/time_series.py` & `sxs-2022.5.1/sxs/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""The `TimeSeries` object provides basic functionality for all time-series-like objects, including
+`WaveformModes`, the objects contained in `Horizons`, etc.
+
+"""
+
 import numpy as np
 
 
 class TimeSeries(np.ndarray):
     # noinspection PyUnresolvedReferences
     """Array-like object representing time-series data
```

### Comparing `sxs-2022.4.5/sxs/utilities/__init__.py` & `sxs-2022.5.1/sxs/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/bitwise.py` & `sxs-2022.5.1/sxs/utilities/bitwise.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/decimation/__init__.py` & `sxs-2022.5.1/sxs/utilities/decimation/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/decimation/greedy_spline.py` & `sxs-2022.5.1/sxs/utilities/decimation/greedy_spline.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/decimation/linear_bisection.py` & `sxs-2022.5.1/sxs/utilities/decimation/linear_bisection.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/decimation/peak_greed.py` & `sxs-2022.5.1/sxs/utilities/decimation/peak_greed.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/decimation/suppression.py` & `sxs-2022.5.1/sxs/utilities/decimation/suppression.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/dicts.py` & `sxs-2022.5.1/sxs/utilities/dicts.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/downloads.py` & `sxs-2022.5.1/sxs/utilities/downloads.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/files.py` & `sxs-2022.5.1/sxs/utilities/files.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/formats.py` & `sxs-2022.5.1/sxs/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/inspire.py` & `sxs-2022.5.1/sxs/utilities/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/__init__.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/comparisons.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/comparisons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/conversion.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/conversion.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/dataset.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/dataset.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/horizons.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/metadata.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/waveform_amp_phase.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/waveform_amp_phase.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/lvcnr/waveforms.py` & `sxs-2022.5.1/sxs/utilities/lvcnr/waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/monotonicity.py` & `sxs-2022.5.1/sxs/utilities/monotonicity.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/pretty_print.py` & `sxs-2022.5.1/sxs/utilities/pretty_print.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/references/ads.py` & `sxs-2022.5.1/sxs/utilities/references/ads.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/references/arxiv.py` & `sxs-2022.5.1/sxs/utilities/references/arxiv.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/references/fairchild_report.py` & `sxs-2022.5.1/sxs/utilities/references/fairchild_report.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/references/inspire.py` & `sxs-2022.5.1/sxs/utilities/references/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/references/journal_abbreviations.py` & `sxs-2022.5.1/sxs/utilities/references/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/select.py` & `sxs-2022.5.1/sxs/utilities/select.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/sxs_directories.py` & `sxs-2022.5.1/sxs/utilities/sxs_directories.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/sxs_identifiers.py` & `sxs-2022.5.1/sxs/utilities/sxs_identifiers.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/utilities/url.py` & `sxs-2022.5.1/sxs/utilities/url.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/__init__.py` & `sxs-2022.5.1/sxs/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/alignment.py` & `sxs-2022.5.1/sxs/waveforms/alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     )
     modes_B = CubicSpline(
         wb.t, wb[:, wb.index(2, -2) : wb.index(ell_max + 1, -(ell_max + 1))].data
     )(t_reference)
 
     normalization = trapezoid(
         CubicSpline(
-            wb.t, wb[:, wb.index(2, -2) : wb.index(ell_max + 1, -(ell_max + 1))].norm
+            wb.t, wb[:, wb.index(2, -2) : wb.index(ell_max + 1, -(ell_max + 1))].norm ** 2
         )(t_reference),
         t_reference,
     )
 
     m = np.array([M for L in range(2, ell_max + 1) for M in range(-L, L + 1)])
 
     optimums = []
```

### Comparing `sxs-2022.4.5/sxs/waveforms/memory.py` & `sxs-2022.5.1/sxs/waveforms/memory.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/mode_utilities.py` & `sxs-2022.5.1/sxs/waveforms/mode_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/nrar.py` & `sxs-2022.5.1/sxs/waveforms/nrar.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py` & `sxs-2022.5.1/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,16 +371,31 @@
     file_name_str = str(file_name)
     group = None
     if ".h5" in file_name_str and not file_name_str.endswith(".h5"):
         file_name_str, group = file_name_str.split(".h5")
     if group == "/":
         group = None
 
-    h5_path = pathlib.Path(file_name_str).expanduser().resolve().with_suffix(".h5")
-    json_path = h5_path.with_suffix(".json")
+    # At this point, file_name_str may or may not have an h5 suffix
+    # (because the user may have passed in a file without the suffix,
+    # or because there was an .h5 in the middle of the filename.)
+    # But that's ok, we will use with_suffix below.
+
+
+    # In a common use case, the h5 and json files will be named
+    # bla.h5 and bla.json as expected, but they will be git-annex symlinks.
+    # This means that the files pointed to will have strange names, like:
+    # bla.h5   -> /some/crazy/path/some_crazy_hash.h5
+    # bla.json -> /some/different/crazy/path/a_different_crazy_hash.json
+    # where the paths are determined by git-annex and the hashes are basically
+    # SHA256 hashes of the contents.
+    #
+    # This means we need to change the suffix *before* the resolve() call.
+    h5_path = pathlib.Path(file_name_str).with_suffix(".h5").expanduser().resolve()
+    json_path = pathlib.Path(file_name_str).with_suffix(".json").expanduser().resolve()
 
     # This will be used for validation
     h5_size = h5_path.stat().st_size
 
     data_type = kwargs.pop("data_type", "unknown")
     m_is_scaled_out = kwargs.pop("m_is_scaled_out", True)
     r_is_scaled_out = kwargs.pop("r_is_scaled_out", True)
@@ -538,15 +553,15 @@
     file_name_str = str(file_name)
     group = None
     if ".h5" in file_name_str and not file_name_str.endswith(".h5"):
         file_name_str, group = file_name_str.split(".h5")
     if group == "/":
         group = None
 
-    h5_path = pathlib.Path(file_name_str).expanduser().resolve().with_suffix(".h5")
+    h5_path = pathlib.Path(file_name_str).with_suffix(".h5").expanduser().resolve()
 
     with h5py.File(h5_path, "r") as f:
         if group is not None:
             g = f[group]
         else:
             g = f
```

### Comparing `sxs-2022.4.5/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py` & `sxs-2022.5.1/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/transformations.py` & `sxs-2022.5.1/sxs/waveforms/transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/waveform_mixin.py` & `sxs-2022.5.1/sxs/waveforms/waveform_mixin.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/waveforms/waveform_modes.py` & `sxs-2022.5.1/sxs/waveforms/waveform_modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,23 @@
     order of increasing `m` and `ell`, with `m` varying most rapidly — something
     like the following:
 
         [f(ell, m) for ell in range(ell_min, ell_max+1) for m in range(-ell,ell+1)]
 
     The total size is implicitly `ell_max * (ell_max + 2) - ell_min ** 2 + 1`.
 
-    For backwards compatibility, it is possible to retrieve individual modes in the
+    The recommended way of retrieving individual modes is
+
+        h_22 = waveform[:, waveform.index(2,2)]
+
+    or equivalently,
+
+        h_22 = waveform.data[:, waveform.index(2,2)]
+
+    For backwards compatibility, it is also possible to retrieve individual modes in the
     same way as the old NRAR-format HDF5 files would be read, as in
 
         h_22 = waveform["Y_l2_m2.dat"]
 
     Note that "History.txt" may not contain anything but an empty string, because
     history is not retained in more recent data formats.  Also note that — while
     not strictly a part of this class — the loaders that open waveform files will
```

### Comparing `sxs-2022.4.5/sxs/zenodo/__init__.py` & `sxs-2022.5.1/sxs/zenodo/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/api/deposit.py` & `sxs-2022.5.1/sxs/zenodo/api/deposit.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/api/login.py` & `sxs-2022.5.1/sxs/zenodo/api/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/api/records.py` & `sxs-2022.5.1/sxs/zenodo/api/records.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/catalog.py` & `sxs-2022.5.1/sxs/zenodo/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/creators.py` & `sxs-2022.5.1/sxs/zenodo/creators.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/simannex.py` & `sxs-2022.5.1/sxs/zenodo/simannex.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/sxs/zenodo/surrogatemodeling.py` & `sxs-2022.5.1/sxs/zenodo/surrogatemodeling.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/conftest.py` & `sxs-2022.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_catalog.py` & `sxs-2022.5.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_horizons.py` & `sxs-2022.5.1/tests/test_horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_loader.py` & `sxs-2022.5.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_metadata.py` & `sxs-2022.5.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_time_series.py` & `sxs-2022.5.1/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_transformations.py` & `sxs-2022.5.1/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_utilities.py` & `sxs-2022.5.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_waveform_rotations.py` & `sxs-2022.5.1/tests/test_waveform_rotations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.4.5/tests/test_waveforms.py` & `sxs-2022.5.1/tests/test_waveforms.py`

 * *Files identical despite different names*

