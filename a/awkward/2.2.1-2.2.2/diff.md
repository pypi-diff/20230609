# Comparing `tmp/awkward-2.2.1.tar.gz` & `tmp/awkward-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr 24 16:57:22 2023, max compression
+gzip compressed data, last modified: Mon Jun  5 18:34:57 2023, max compression
```

## Comparing `awkward-2.2.1.tar` & `awkward-2.2.2.tar`

### file list

```diff
@@ -1,853 +1,857 @@
--rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.1/CITATION.cff
--rw-r--r--   0        0        0    13855 2023-04-24 16:57:22.000000 awkward-2.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-04-24 16:57:22.000000 awkward-2.2.1/README.md
--rw-r--r--   0        0        0      241 2023-04-24 16:57:22.000000 awkward-2.2.1/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/conf.py
--rw-r--r--   0        0        0      346 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/index.md
--rw-r--r--   0        0        0    11642 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/redirects.json
--rw-r--r--   0        0        0      463 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/requirements.txt
--rw-r--r--   0        0        0      460 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    25534 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/ak.behavior.md
--rw-r--r--   0        0        0     1426 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/index.md
--rw-r--r--   0        0        0     7349 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-04-24 16:57:22.000000 awkward-2.2.1/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1325 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/__init__.py
--rw-r--r--   0        0        0     5026 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_behavior.py
--rw-r--r--   0        0        0    39029 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    13617 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_do.py
--rw-r--r--   0        0        0    12279 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_errors.py
--rw-r--r--   0        0        0     5672 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5860 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_lookup.py
--rw-r--r--   0        0        0     5454 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    24569 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_reducers.py
--rw-r--r--   0        0        0     2041 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23934 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_typing.py
--rw-r--r--   0        0        0     2498 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forth.py
--rw-r--r--   0        0        0   103232 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8005 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/index.py
--rw-r--r--   0        0        0     3988 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/jax.py
--rw-r--r--   0        0        0     6017 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/numba.py
--rw-r--r--   0        0        0     8272 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/record.py
--rw-r--r--   0        0        0     1002 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/typetracer.py
--rw-r--r--   0        0        0        0 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1259 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     3763 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1781 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      944 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1902 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53533 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      985 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4485 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    11395 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    37988 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      755 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
--rw-r--r--   0        0        0      806 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0     1123 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0      623 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
--rw-r--r--   0        0        0      789 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19822 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0     6627 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5982 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35824 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1182 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31510 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9624 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49124 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9377 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     1111 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    13294 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     4939 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1357 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2010 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2922 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    14150 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     2288 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    43889 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     8509 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    27803 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    40958 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    45020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13347 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    40382 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    63462 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    60161 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    85023 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    49439 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    45029 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    54872 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    57740 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    18878 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     5955 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5242 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3244 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    15639 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5630 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5020 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5508 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4602 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     5902 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8095 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     4971 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     7647 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4116 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4828 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3500 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     8181 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     3503 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5109 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3819 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5924 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5881 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3158 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      952 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9855 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6595 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12213 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5319 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4730 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3537 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     4672 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4581 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50451 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5323 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3467 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2727 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14486 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     4109 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30065 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11931 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3324 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     3000 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2513 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8934 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4753 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     6466 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     8103 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3603 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12413 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     6418 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4410 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3909 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5396 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4216 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9604 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3063 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     2839 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2670 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     7160 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10754 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2370 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6378 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1107 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13370 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11648 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4507 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2123 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    16968 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2785 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3382 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23979 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4422 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9461 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2484 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1138 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     8388 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5862 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6130 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2600 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3756 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8819 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     2168 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     2972 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6174 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4866 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     9079 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3874 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1341 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0    10063 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/type.py
--rw-r--r--   0        0        0     4602 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     2492 2023-04-24 16:57:22.000000 awkward-2.2.1/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6321 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6615 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77410 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35162 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3212 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2338 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0912_packed.py
--rw-r--r--   0        0        0   113054 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28376 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26467 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33145 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1085 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     4372 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4607 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2845 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     1018 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2085_empty_if_typetracer.py
--rw-r--r--   0        0        0     2765 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     6059 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4104 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      560 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0      720 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2296_duplicate_field.py
--rw-r--r--   0        0        0     2262 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      648 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2929 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      721 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15615 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      647 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0      934 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2364_empty_list_of_string.py
--rw-r--r--   0        0        0    37200 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2921 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5250 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5848 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1037 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      956 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      212 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0     1070 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      800 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      704 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      351 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1563 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1211 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      545 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      495 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-04-24 16:57:22.000000 awkward-2.2.1/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9911 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1782 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-04-24 16:57:22.000000 awkward-2.2.1/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-04-24 16:57:22.000000 awkward-2.2.1/.gitignore
--rw-r--r--   0        0        0     1520 2023-04-24 16:57:22.000000 awkward-2.2.1/LICENSE
--rw-r--r--   0        0        0     8479 2023-04-24 16:57:22.000000 awkward-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-24 16:57:22.000000 awkward-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-06-05 18:34:57.000000 awkward-2.2.2/CITATION.cff
+-rw-r--r--   0        0        0    13855 2023-06-05 18:34:57.000000 awkward-2.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-06-05 18:34:57.000000 awkward-2.2.2/README.md
+-rw-r--r--   0        0        0      241 2023-06-05 18:34:57.000000 awkward-2.2.2/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/redirects.json
+-rw-r--r--   0        0        0      463 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/requirements.txt
+-rw-r--r--   0        0        0      460 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24165 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/reference/index.md
+-rw-r--r--   0        0        0     7349 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-06-05 18:34:57.000000 awkward-2.2.2/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1325 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/__init__.py
+-rw-r--r--   0        0        0     4626 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    38487 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0    13672 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_do.py
+-rw-r--r--   0        0        0    12279 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5784 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5860 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     5454 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    26534 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     2041 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2498 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forth.py
+-rw-r--r--   0        0        0   103232 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8044 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/jax.py
+-rw-r--r--   0        0        0     6017 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/numba.py
+-rw-r--r--   0        0        0     8272 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/record.py
+-rw-r--r--   0        0        0     1679 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     2121 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3763 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1453 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1425 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53533 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4485 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    11515 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    37988 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      806 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0      789 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0    10375 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35829 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31510 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9624 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49133 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1111 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    16149 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     5365 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2276 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     3065 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    14154 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     3579 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/placeholder.py
+-rw-r--r--   0        0        0     2379 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    48307 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     7884 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    28289 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    41835 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    44581 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13853 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    41044 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    64499 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    62401 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    84788 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    50243 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    46017 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    56591 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    58157 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    19483 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      962 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     5955 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5242 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3381 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    18686 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5630 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5020 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5508 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4753 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     5902 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8095 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     4971 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     7647 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4116 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4828 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3500 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8181 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     3503 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5109 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3819 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5924 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5881 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3158 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      952 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9855 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6595 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15615 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1420 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8118 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12753 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2715 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5319 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4730 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3537 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     4672 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4581 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50451 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1106 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5323 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3467 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7802 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3154 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      813 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2727 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14486 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1839 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1651 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     4109 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1716 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    30065 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2282 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11931 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3324 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     3000 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8859 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      873 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2513 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      705 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      930 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2568 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8934 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3258 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4753 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     6466 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     8103 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3603 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12413 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3217 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     6418 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4410 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2081 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5103 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3909 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1951 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4362 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1786 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5396 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4216 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2275 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9604 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3063 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     2839 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2670 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     7160 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3058 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10754 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4931 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6725 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2370 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6378 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6050 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1107 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13370 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1106 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11648 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4507 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2612 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2123 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3354 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    16968 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2785 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3382 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23979 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4422 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9461 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2484 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1138 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2659 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     8388 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5862 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6130 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2600 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1848 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3756 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1509 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2134 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8819 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2168 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     3007 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6171 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4886 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8774 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3928 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1341 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10063 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4593 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     2489 2023-06-05 18:34:57.000000 awkward-2.2.2/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6321 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2335 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   113054 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28376 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26468 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33145 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18809 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4372 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      727 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4607 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2845 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1716 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2765 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     6059 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4104 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      877 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      720 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2262 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      648 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2929 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15615 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      934 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37200 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2921 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5250 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5848 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      956 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      212 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0     1070 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      800 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      704 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      351 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1563 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1211 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      545 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      495 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      857 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2471_flatten_string.py
+-rw-r--r--   0        0        0     1032 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2484_reduce_starts_empty.py
+-rw-r--r--   0        0        0      659 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2487_broadcast_list_offsets.py
+-rw-r--r--   0        0        0     1319 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2490_reduce_regulararray_positional.py
+-rw-r--r--   0        0        0     1816 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2495_concatenate_typetracer.py
+-rw-r--r--   0        0        0     3800 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/test_2501_positional_record_reducer.py
+-rw-r--r--   0        0        0      128 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-06-05 18:34:57.000000 awkward-2.2.2/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9757 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1629 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-06-05 18:34:57.000000 awkward-2.2.2/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-06-05 18:34:57.000000 awkward-2.2.2/.gitignore
+-rw-r--r--   0        0        0     1520 2023-06-05 18:34:57.000000 awkward-2.2.2/LICENSE
+-rw-r--r--   0        0        0     8479 2023-06-05 18:34:57.000000 awkward-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-06-05 18:34:57.000000 awkward-2.2.2/PKG-INFO
```

### Comparing `awkward-2.2.1/CITATION.cff` & `awkward-2.2.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/CONTRIBUTING.md` & `awkward-2.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/README.md` & `awkward-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/_toc.yml` & `awkward-2.2.2/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/conf.py` & `awkward-2.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/index.md` & `awkward-2.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/prepare_docstrings.py` & `awkward-2.2.2/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/redirects-user-guide.json` & `awkward-2.2.2/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/redirects.json` & `awkward-2.2.2/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/_static/css/awkward.css` & `awkward-2.2.2/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/getting-started/community-tutorials.md` & `awkward-2.2.2/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/getting-started/index.md` & `awkward-2.2.2/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/getting-started/papers-and-talks.md` & `awkward-2.2.2/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.2.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/image/example-hierarchy.svg` & `awkward-2.2.2/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/reference/ak.behavior.md` & `awkward-2.2.2/docs/reference/ak.behavior.md`

 * *Files 7% similar despite different names*

```diff
@@ -566,58 +566,14 @@
 so that
 
 ```python
 >>> ak.type(ak.Array(["one", "two", "three"]))
 3 * string
 ```
 
-## Custom broadcasting
-
-In situations where we want to think about lists as objects, such as strings,
-we may even need to override the broadcasting rules. For instance, given
-
-```python
-ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]])
-```
-
-we might expect `"HAL"` to broadcast to each `1`, like
-
-```python
-[[[73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77], [73, 66, 77]]]
-```
-
-but (without custom broadcasting) instead it raises a broadcasting for any
-length of `1` list other than 3:
-
-```python
->>> # without custom broadcasting
->>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1, 1, 1]]))
-ValueError: in ListOffsetArray64, cannot broadcast nested list
->>> print(ak.Array(["HAL"]) + ak.Array([[1, 1, 1]]))
-[[73, 66, 77]]
-```
-
-It's matching each character of `"HAL"` with a number from the list, but we
-want the string to be taken as an object. That is fixed (in
-`ak.behaviors.string`) with a custom broadcasting rule:
-
-```python
-def _string_broadcast(layout, offsets):
-    # layout:  an ak.layout.Content object
-    # offsets: an ak.layout.Index of offsets to match
-    #
-    # should return: an ak.layout.Content object of the broadcasted result
-    ...
-
-awkward.behavior["__broadcast__", "string"] = _string_broadcast
-```
-
-Very few applications would need to do this, but the {data}`ak.behavior` object
-provides a lot of room for customization hooks like this.
-
 ## Overriding behavior in Numba
 
 Awkward Arrays can be arguments and return values of functions compiled with
 [Numba](http://numba.pydata.org). Since these functions run on low-level
 objects, most functionality must be reimplemented, including behavioral
 overrides.
```

### Comparing `awkward-2.2.1/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.2.2/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/reference/awkwardforth.rst` & `awkward-2.2.2/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/reference/toctree.txt` & `awkward-2.2.2/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.2.2/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.2.2/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.2.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-json.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-python.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.2.2/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.2.2/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-constructors.md` & `awkward-2.2.2/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-lists.md` & `awkward-2.2.2/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-missing.md` & `awkward-2.2.2/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-records.md` & `awkward-2.2.2/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-strings.md` & `awkward-2.2.2/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.2.2/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.2.2/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.2.2/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.2.2/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.2.2/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-examine-type.md` & `awkward-2.2.2/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.2.2/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-filter-masked.md` & `awkward-2.2.2/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-filter-num.md` & `awkward-2.2.2/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.2.2/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.2.2/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.2.2/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-gpu.md` & `awkward-2.2.2/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-numpy.md` & `awkward-2.2.2/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-reducing.md` & `awkward-2.2.2/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-math-statistics.md` & `awkward-2.2.2/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.2.2/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.2.2/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.2.2/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.2.2/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.2.2/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.2.2/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.2.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.2.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.2.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.2.2/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-data-analysts.png` & `awkward-2.2.2/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-data-analysts.svg` & `awkward-2.2.2/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-developers.png` & `awkward-2.2.2/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-developers.svg` & `awkward-2.2.2/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-doxygen.png` & `awkward-2.2.2/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-sphinx.png` & `awkward-2.2.2/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-tutorials-alternate.png` & `awkward-2.2.2/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/panel-tutorials.png` & `awkward-2.2.2/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.2.2/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.2.2/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-timeline.png` & `awkward-2.2.2/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.2.2/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.2.2/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.2.2/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.2.2/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.2.2/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.2.2/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.2.2/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.2.2/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.2.2/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.2.2/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-array.svg` & `awkward-2.2.2/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-hierarchy.png` & `awkward-2.2.2/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.2.2/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.2.2/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.2.2/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-reduction.png` & `awkward-2.2.2/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/example-reduction.svg` & `awkward-2.2.2/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/git-strategy.pdf` & `awkward-2.2.2/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/git-strategy.png` & `awkward-2.2.2/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/git-strategy.svg` & `awkward-2.2.2/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.2.2/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.2.2/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/how-it-works.svg` & `awkward-2.2.2/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/sorting-axis.svg` & `awkward-2.2.2/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/all.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/any.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/count.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/max.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/min.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/product.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/diagrams/reducers/sum.svg` & `awkward-2.2.2/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/logo/favicon.ico` & `awkward-2.2.2/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/logo/logo-300px-white.png` & `awkward-2.2.2/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/logo/logo-300px.png` & `awkward-2.2.2/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/logo/logo-600px.png` & `awkward-2.2.2/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/logo/logo.svg` & `awkward-2.2.2/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/photos/desire-path.jpg` & `awkward-2.2.2/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.2.2/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/plots/awkward-0-popularity.png` & `awkward-2.2.2/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.2.2/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.2.2/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.2.2/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/__init__.py` & `awkward-2.2.2/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_behavior.py` & `awkward-2.2.2/src/awkward/_behavior.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,27 +63,14 @@
     for cls in type(obj).__mro__:
         fcn = behavior.get(("__cast__", cls))
         if fcn is not None:
             return fcn
     return None
 
 
-def find_custom_broadcast(layout, behavior):
-    behavior = overlay_behavior(behavior)
-    custom = layout.parameter("__array__")
-    if custom is None:
-        custom = layout.parameter("__record__")
-    if custom is None:
-        custom = layout.purelist_parameter("__record__")
-    if isinstance(custom, str):
-        return behavior.get(("__broadcast__", custom))
-    else:
-        return None
-
-
 def find_ufunc_generic(ufunc, layout, behavior):
     behavior = overlay_behavior(behavior)
     custom = layout.parameter("__array__")
     if custom is None:
         custom = layout.parameter("__record__")
     if isinstance(custom, str):
         fcn = behavior.get((ufunc, custom))
```

### Comparing `awkward-2.2.1/src/awkward/_broadcasting.py` & `awkward-2.2.2/src/awkward/_broadcasting.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import functools
 import itertools
 from collections.abc import Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import backend_of
-from awkward._behavior import find_custom_broadcast
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_are_empty,
     parameters_are_equal,
     parameters_intersect,
@@ -103,27 +102,35 @@
             return x[0]
 
 
 def in_function(options):
     if options["function_name"] is None:
         return ""
     else:
-        return "in " + options["function_name"]
+        return " in " + options["function_name"]
 
 
 def checklength(inputs, options):
-    length = inputs[0].length
-    for x in inputs[1:]:
-        if x.length != length:
+    it = iter(inputs)
+    length: int
+    for content in it:
+        if content.length is not unknown_length:
+            length = content.length
+            break
+
+    for other_content in it:
+        if other_content.length is unknown_length:
+            continue
+        if other_content.length != length:
             raise ValueError(
                 "cannot broadcast {} of length {} with {} of length {}{}".format(
-                    type(inputs[0]).__name__,
+                    type(content).__name__,
                     length,
-                    type(x).__name__,
-                    x.length,
+                    type(other_content).__name__,
+                    other_content.length,
                     in_function(options),
                 )
             )
 
 
 def all_same_offsets(backend: Backend, inputs: list) -> bool:
     index_nplike = backend.index_nplike
@@ -400,19 +407,15 @@
                     depth_context,
                     lateral_context,
                     behavior,
                     options,
                 )
 
     # Now all lengths must agree.
-    if backend.nplike.known_data:
-        checklength(contents, options)
-    else:
-        for x in contents:
-            x._touch_shape(recursive=False)
+    checklength(contents, options)
 
     # Load the parameter broadcasting rule implementation
     rule = options["broadcast_parameters_rule"]
     try:
         parameters_factory_impl = BROADCAST_RULE_TO_FACTORY_IMPL[rule]
     except KeyError:
         raise ValueError(
@@ -504,16 +507,18 @@
                 # Any unknown length sets max_size to unknown
                 if x.size is unknown_length:
                     dim_size = unknown_length
                 # Any zero-length column triggers zero broadcasting
                 elif x.size == 0:
                     dim_size = 0
                     break
+                # Take first size as dim_size
                 elif dim_size is None:
                     dim_size = x.size
+                # If the dim_size is unknown, we can't compare
                 elif dim_size is unknown_length:
                     continue
                 else:
                     dim_size = max(dim_size, x.size)
 
             dimsize_greater_than_one_if_known = (
                 dim_size is unknown_length or dim_size > 1
@@ -591,77 +596,36 @@
             assert isinstance(outcontent, tuple)
             parameters = parameters_factory(len(outcontent))
             return tuple(
                 RegularArray(x, dim_size, length, parameters=p)
                 for x, p in zip(outcontent, parameters)
             )
 
-        elif not backend.nplike.known_data:
-            offsets = None
-            nextinputs = []
-            for x in inputs:
-                if isinstance(x, ListOffsetArray):
-                    x._touch_data(recursive=False)
-                    offsets = Index64(
-                        backend.index_nplike.empty(
-                            x.offsets.data.shape[0], dtype=np.int64
-                        ),
-                        nplike=backend.index_nplike,
-                    )
-                    nextinputs.append(x.content)
-                elif isinstance(x, ListArray):
-                    x._touch_data(recursive=False)
-                    offsets = Index64(
-                        backend.index_nplike.empty(
-                            x.starts.data.shape[0] + 1, dtype=np.int64
-                        ),
-                        nplike=backend.index_nplike,
-                    )
-                    nextinputs.append(x.content)
-                elif isinstance(x, RegularArray):
-                    nextinputs.append(x.content)
-                else:
-                    nextinputs.append(x)
-            assert offsets is not None
-
-            outcontent = apply_step(
-                backend,
-                nextinputs,
-                action,
-                depth + 1,
-                copy.copy(depth_context),
-                lateral_context,
-                behavior,
-                options,
-            )
-            assert isinstance(outcontent, tuple)
-            parameters = parameters_factory(len(outcontent))
-            return tuple(
-                ListOffsetArray(offsets, x, parameters=p)
-                for x, p in zip(outcontent, parameters)
-            )
-
         # Not all regular, but all same offsets?
         # Optimization: https://github.com/scikit-hep/awkward-1.0/issues/442
-        elif all_same_offsets(backend, inputs):
+        elif index_nplike.known_data and all_same_offsets(backend, inputs):
             lencontent, offsets, starts, stops = None, None, None, None
             nextinputs = []
 
             for x in inputs:
                 if isinstance(x, ListOffsetArray):
                     offsets = x.offsets
-                    lencontent = offsets[-1]
+                    lencontent = index_nplike.index_as_shape_item(offsets[-1])
                     nextinputs.append(x.content[:lencontent])
 
                 elif isinstance(x, ListArray):
                     starts, stops = x.starts, x.stops
-                    if starts.length == 0 or stops.length == 0:
+                    if (starts.length is not unknown_length and starts.length == 0) or (
+                        stops.length is not unknown_length and stops.length == 0
+                    ):
                         nextinputs.append(x.content[:0])
                     else:
-                        lencontent = backend.index_nplike.max(stops)
+                        lencontent = index_nplike.index_as_shape_item(
+                            index_nplike.max(stops)
+                        )
                         nextinputs.append(x.content[:lencontent])
                 elif isinstance(x, RegularArray):
                     nextinputs.append(x.content[: x.size * x.length])
                 else:
                     nextinputs.append(x)
 
             outcontent = apply_step(
@@ -696,53 +660,73 @@
                     "unexpected offsets, starts: {}, {}".format(
                         type(offsets), type(starts)
                     )
                 )
 
         # General list-handling case: the offsets of each list may be different.
         else:
-            fcns = [
-                find_custom_broadcast(x, behavior) if isinstance(x, Content) else None
-                for x in inputs
-            ]
+            # We have three possible cases here:
+            # 1. all-string (nothing to do)
+            # 2. mixed string-list (strings gain a dimension and broadcast to the non-string offsets)
+            # 3. no strings (all lists broadcast to a single offsets)
+            offsets_content = None
+            all_content_strings = True
+            input_is_string = []
+            for x in inputs:
+                if isinstance(x, Content):
+                    content_is_string = x.parameter("__array__") in {
+                        "string",
+                        "bytestring",
+                    }
+                    # Don't try and take offsets from strings
+                    if not content_is_string:
+                        all_content_strings = False
+                        # Take the offsets from the first irregular list
+                        if x.is_list and not x.is_regular and offsets_content is None:
+                            offsets_content = x
+                    input_is_string.append(content_is_string)
+                else:
+                    input_is_string.append(False)
 
-            # Find first list without custom broadcasting which will define the broadcast offsets
-            # Don't consider RegularArray (handle case of 1-sized regular broadcasting)
-            # Do this to prioritise non-custom broadcasting
-            first = None
-
-            for x, fcn in zip(inputs, fcns):
-                if (
-                    isinstance(x, listtypes)
-                    and not isinstance(x, RegularArray)
-                    and fcn is None
-                ):
-                    first = x
-                    break
+            # case (1): user getfunctions should exit before this gets called
+            if all_content_strings:
+                raise ValueError(
+                    "cannot broadcast all strings: {}{}".format(
+                        ", ".join(repr(type(x)) for x in inputs), in_function(options)
+                    )
+                )
 
-            # Did we fail to find a list without custom broadcasting?
-            secondround = False
-            # If we failed to find an irregular, non-custom broadcasting list,
-            # continue search for *any* list.
-            if first is None:
-                secondround = True
-                for x in inputs:
-                    if isinstance(x, listtypes) and not isinstance(x, RegularArray):
-                        first = x
+            # Didn't find a ragged list, try any list!
+            if offsets_content is None:
+                for content in contents:
+                    if content.is_list:
+                        offsets_content = content
                         break
+                else:
+                    raise AssertionError("no list found in list branch!")
 
-            offsets = first._compact_offsets64(True)
+            offsets = offsets_content._compact_offsets64(True)
 
             nextinputs = []
-            for x, fcn in zip(inputs, fcns):
-                if callable(fcn) and not secondround:
-                    nextinputs.append(fcn(x, offsets))
+            for x, x_is_string in zip(inputs, input_is_string):
+                if x_is_string:
+                    offsets_data = backend.index_nplike.asarray(offsets)
+                    counts = offsets_data[1:] - offsets_data[:-1]
+                    if ak._util.win or ak._util.bits32:
+                        counts = index_nplike.astype(counts, dtype=np.int32)
+                    parents = index_nplike.repeat(
+                        index_nplike.arange(counts.size, dtype=counts.dtype), counts
+                    )
+                    nextinputs.append(
+                        ak.contents.IndexedArray(
+                            ak.index.Index64(parents, nplike=index_nplike), x
+                        ).project()
+                    )
                 elif isinstance(x, listtypes):
                     nextinputs.append(x._broadcast_tooffsets64(offsets).content)
-
                 # Handle implicit left-broadcasting (non-NumPy-like broadcasting).
                 elif options["left_broadcast"] and isinstance(x, Content):
                     nextinputs.append(
                         RegularArray(x, 1, x.length)
                         ._broadcast_tooffsets64(offsets)
                         .content
                     )
@@ -764,60 +748,48 @@
 
             return tuple(
                 ListOffsetArray(offsets, x, parameters=p)
                 for x, p in zip(outcontent, parameters)
             )
 
     def broadcast_any_option():
-        if backend.nplike.known_data:
-            mask = None
-            for x in contents:
-                if x.is_option:
-                    m = x.mask_as_bool(valid_when=False)
-                    if mask is None:
-                        mask = m
-                    else:
-                        mask = backend.index_nplike.logical_or(mask, m, maybe_out=mask)
+        mask = None
+        for x in contents:
+            if x.is_option:
+                m = x.mask_as_bool(valid_when=False)
+                if mask is None:
+                    mask = m
+                else:
+                    mask = backend.index_nplike.logical_or(mask, m, maybe_out=mask)
 
-            nextmask = Index8(mask.view(np.int8))
-            index = backend.index_nplike.full(mask.shape[0], -1, dtype=np.int64)
-            index[~mask] = backend.index_nplike.arange(
-                mask.shape[0] - backend.index_nplike.count_nonzero(mask),
+        nextmask = Index8(mask.view(np.int8))
+        index = backend.index_nplike.full(mask.shape[0], -1, dtype=np.int64)
+        index[~mask] = backend.index_nplike.arange(
+            backend.index_nplike.shape_item_as_index(mask.shape[0])
+            - backend.index_nplike.count_nonzero(mask),
+            dtype=np.int64,
+        )
+        index = Index64(index)
+        if any(not x.is_option for x in contents):
+            nextindex = backend.index_nplike.arange(
+                backend.index_nplike.shape_item_as_index(mask.shape[0]),
                 dtype=np.int64,
             )
-            index = Index64(index)
-            if any(not x.is_option for x in contents):
-                nextindex = backend.index_nplike.arange(mask.shape[0], dtype=np.int64)
-                nextindex[mask] = -1
-                nextindex = Index64(nextindex)
+            nextindex[mask] = -1
+            nextindex = Index64(nextindex)
 
-            nextinputs = []
-            for x in inputs:
-                if isinstance(x, optiontypes):
-                    nextinputs.append(x.project(nextmask))
-                elif isinstance(x, Content):
-                    nextinputs.append(
-                        IndexedOptionArray(nextindex, x).project(nextmask)
-                    )
-                else:
-                    nextinputs.append(x)
+        nextinputs = []
+        for x in inputs:
+            if isinstance(x, optiontypes):
+                nextinputs.append(x.project(nextmask))
+            elif isinstance(x, Content):
+                nextinputs.append(IndexedOptionArray(nextindex, x).project(nextmask))
+            else:
+                nextinputs.append(x)
 
-        else:
-            index = None
-            nextinputs = []
-            for x in inputs:
-                if isinstance(x, optiontypes):
-                    x._touch_data(recursive=False)
-                    index = Index64(
-                        backend.index_nplike.empty(x.length, dtype=np.int64)
-                    )
-                    nextinputs.append(x.content)
-                else:
-                    nextinputs.append(x)
-            assert index is not None
         outcontent = apply_step(
             backend,
             nextinputs,
             action,
             depth,
             copy.copy(depth_context),
             lateral_context,
```

### Comparing `awkward-2.2.1/src/awkward/_do.py` & `awkward-2.2.2/src/awkward/_do.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,16 @@
     layout: Content,
     reducer: ak._reducers.Reducer,
     axis: AxisMaybeNone = -1,
     mask: bool = True,
     keepdims: bool = False,
     behavior: dict | None = None,
 ):
+    reducer = layout.backend.prepare_reducer(reducer)
+
     if axis is None:
         parts = remove_structure(
             layout,
             flatten_records=False,
             drop_nones=False,
             keepdims=keepdims,
             allow_records=True,
```

### Comparing `awkward-2.2.1/src/awkward/_errors.py` & `awkward-2.2.2/src/awkward/_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_kernels.py` & `awkward-2.2.2/src/awkward/_kernels.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Callable
 
 import awkward as ak
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._nplikes.typetracer import try_touch_data
 from awkward._typing import Protocol, TypeAlias
 
 KernelKeyType: TypeAlias = tuple  # Tuple[str, Unpack[Tuple[metadata.dtype, ...]]]
 
 
 numpy = Numpy.instance()
 metadata = NumpyMetadata.instance()
@@ -179,14 +180,16 @@
 
 
 class TypeTracerKernel:
     def __init__(self, index):
         self._name_and_types = index
 
     def __call__(self, *args) -> TypeTracerKernelError:
+        for arg in args:
+            try_touch_data(arg)
         return TypeTracerKernelError()
 
     def __repr__(self):
         return "<{} {}{}>".format(
             type(self).__name__,
             self._name_and_types[0],
             "".join(", " + str(metadata.dtype(x)) for x in self._name_and_types[1:]),
```

### Comparing `awkward-2.2.1/src/awkward/_layout.py` & `awkward-2.2.2/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_lookup.py` & `awkward-2.2.2/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_parameters.py` & `awkward-2.2.2/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_prettyprint.py` & `awkward-2.2.2/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_reducers.py` & `awkward-2.2.2/src/awkward/_reducers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from typing import Any as AnyType
+from abc import abstractmethod
 
 import awkward as ak
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward._typing import Final
+from awkward._nplikes.shape import ShapeItem
+from awkward._typing import Any as AnyType
+from awkward._typing import Final, Protocol
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 DTypeLike = AnyType
 
 
-class Reducer(ABC):
+class Reducer(Protocol):
     name: str
 
     # Does the output correspond to array positions?
     @property
     @abstractmethod
     def needs_position(self) -> bool:
         ...
@@ -29,249 +30,256 @@
     def preferred_dtype(self) -> DTypeLike:
         ...
 
     @classmethod
     def highlevel_function(cls):
         return getattr(ak.operations, cls.name)
 
-    @classmethod
-    def return_dtype(cls, given_dtype: DTypeLike) -> DTypeLike:
-        if given_dtype in (np.bool_, np.int8, np.int16, np.int32):
-            return np.int32 if ak._util.win or ak._util.bits32 else np.int64
-
-        if given_dtype in (np.uint8, np.uint16, np.uint32):
-            return np.uint32 if ak._util.win or ak._util.bits32 else np.uint64
+    @abstractmethod
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
+        ...
 
-        return given_dtype
 
+class KernelReducer(Reducer):
     @classmethod
-    def maybe_double_length(cls, type: DTypeLike, length: int) -> int:
+    def _length_for_kernel(cls, type: DTypeLike, length: ShapeItem) -> ShapeItem:
+        # Complex types are implemented as double-wide arrays
         return 2 * length if type in (np.complex128, np.complex64) else length
 
     @classmethod
-    def maybe_other_type(cls, dtype: DTypeLike) -> DTypeLike:
+    def _dtype_for_kernel(cls, dtype: DTypeLike) -> DTypeLike:
         dtype = np.dtype(dtype)
-        type = np.int64 if dtype.kind.upper() == "M" else dtype.type
-        if dtype == np.complex128:
-            type = np.float64
-        if dtype == np.complex64:
-            type = np.float32
-        return type
+        if dtype.kind.upper() == "M":
+            return np.dtype(np.int64)
+        elif dtype == np.complex128:
+            return np.dtype(np.float64)
+        elif dtype == np.complex64:
+            return np.dtype(np.float32)
+        else:
+            return dtype
 
-    @abstractmethod
-    def identity_for(self, dtype: DTypeLike | None):
-        raise NotImplementedError
+    @classmethod
+    def _promote_integer_rank(cls, given_dtype: DTypeLike) -> DTypeLike:
+        if given_dtype in (np.bool_, np.int8, np.int16, np.int32):
+            return np.int32 if ak._util.win or ak._util.bits32 else np.int64
 
-    @abstractmethod
-    def apply(self, array, parents, outlength: int):
-        raise NotImplementedError
+        elif given_dtype in (np.uint8, np.uint16, np.uint32):
+            return np.uint32 if ak._util.win or ak._util.bits32 else np.uint64
+
+        else:
+            return given_dtype
 
 
-class ArgMin(Reducer):
+class ArgMin(KernelReducer):
     name: Final = "argmin"
-    needs_position: Final = True
     preferred_dtype: Final = np.int64
+    needs_position: Final = True
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.int64
-
-    def identity_for(self, dtype: np.dtype | None):
-        return np.int64(-1)
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
+        # View array data in kernel-supported dtype
+        kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
         result = array.backend.nplike.empty(outlength, dtype=np.int64)
         if array.dtype.type in (np.complex128, np.complex64):
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_argmin_complex",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
         else:
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_argmin",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        return ak.contents.NumpyArray(result)
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
 
-class ArgMax(Reducer):
+class ArgMax(KernelReducer):
     name: Final = "argmax"
-    needs_position: Final = True
     preferred_dtype: Final = np.int64
+    needs_position: Final = True
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.int64
-
-    def identity_for(self, dtype: np.dtype | None):
-        return np.int64(-1)
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
+        # View array data in kernel-supported dtype
+        kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
         result = array.backend.nplike.empty(outlength, dtype=np.int64)
         if array.dtype.type in (np.complex128, np.complex64):
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_argmax_complex",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
         else:
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_argmax",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        return ak.contents.NumpyArray(result)
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
 
-class Count(Reducer):
+class Count(KernelReducer):
     name: Final = "count"
     preferred_dtype: Final = np.int64
     needs_position: Final = False
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.int64
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
         result = array.backend.nplike.empty(outlength, dtype=np.int64)
         assert parents.nplike is array.backend.index_nplike
-        array._handle_error(
+        array.backend.maybe_kernel_error(
             array.backend[
                 "awkward_reduce_count_64", result.dtype.type, parents.dtype.type
             ](
                 result,
                 parents.data,
                 parents.length,
                 outlength,
             )
         )
-        return ak.contents.NumpyArray(result)
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
-    def identity_for(self, dtype: np.dtype | None):
-        return np.int64(0)
 
-
-class CountNonzero(Reducer):
+class CountNonzero(KernelReducer):
     name: Final = "count_nonzero"
     preferred_dtype: Final = np.float64
     needs_position: Final = False
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.int64
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = np.dtype(np.int64) if array.dtype.kind.upper() == "M" else array.dtype
+        # View array data in kernel-supported dtype
+        kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
+
         result = array.backend.nplike.empty(outlength, dtype=np.int64)
-        if array.dtype.type in (np.complex128, np.complex64):
+        if np.issubdtype(array.dtype, np.complexfloating):
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_countnonzero_complex",
                     result.dtype.type,
-                    np.float64 if array.dtype.type == np.complex128 else np.float32,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
         else:
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_countnonzero",
                     result.dtype.type,
-                    dtype.type,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        return ak.contents.NumpyArray(result)
-
-    def identity_for(self, dtype: np.dtype | None):
-        return np.int64(0)
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
 
-class Sum(Reducer):
+class Sum(KernelReducer):
     name: Final = "sum"
     preferred_dtype: Final = np.float64
     needs_position: Final = False
 
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
         if array.dtype.kind == "M":
             raise ValueError(f"cannot compute the sum (ak.sum) of {array.dtype!r}")
-        else:
-            dtype = self.maybe_other_type(array.dtype)
-        result = array.backend.nplike.empty(
-            self.maybe_double_length(array.dtype.type, outlength),
-            dtype=self.return_dtype(dtype),
-        )
 
+        # Boolean kernels are special; the result is _not_ a boolean
         if array.dtype == np.bool_:
+            result = array.backend.nplike.empty(
+                self._length_for_kernel(array.dtype.type, outlength),
+                dtype=self._promote_integer_rank(np.bool_),
+            )
             if result.dtype in (np.int64, np.uint64):
                 assert parents.nplike is array.backend.index_nplike
-                array._handle_error(
+                array.backend.maybe_kernel_error(
                     array.backend[
                         "awkward_reduce_sum_int64_bool_64",
                         np.int64,
                         array.dtype.type,
                         parents.dtype.type,
                     ](
                         result,
@@ -279,15 +287,15 @@
                         parents.data,
                         parents.length,
                         outlength,
                     )
                 )
             elif result.dtype in (np.int32, np.uint32):
                 assert parents.nplike is array.backend.index_nplike
-                array._handle_error(
+                array.backend.maybe_kernel_error(
                     array.backend[
                         "awkward_reduce_sum_int32_bool_64",
                         np.int32,
                         array.dtype.type,
                         parents.dtype.type,
                     ](
                         result,
@@ -295,268 +303,265 @@
                         parents.data,
                         parents.length,
                         outlength,
                     )
                 )
             else:
                 raise NotImplementedError
-        elif array.dtype.type in (np.complex128, np.complex64):
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_sum_complex",
-                    np.float64 if array.dtype.type == np.complex128 else np.float32,
-                    np.float64 if array.dtype.type == np.complex128 else np.float32,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                )
-            )
+            return ak.contents.NumpyArray(result, backend=array.backend)
         else:
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_sum",
-                    result.dtype.type,
-                    np.int64 if array.dtype.kind == "m" else array.dtype.type,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                )
+            # View array data in kernel-supported dtype
+            kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
+            result = array.backend.nplike.empty(
+                self._length_for_kernel(array.dtype.type, outlength),
+                dtype=self._promote_integer_rank(kernel_array_data.dtype),
             )
+            if array.dtype.type in (np.complex128, np.complex64):
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_sum_complex",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                    )
+                )
+            else:
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_sum",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                    )
+                )
 
-        if array.dtype.kind == "m":
             return ak.contents.NumpyArray(
-                array.backend.nplike.asarray(result, dtype=array.dtype)
+                result.view(self._promote_integer_rank(array.dtype)),
+                backend=array.backend,
             )
-        elif array.dtype.type in (np.complex128, np.complex64):
-            return ak.contents.NumpyArray(result.view(array.dtype))
-        else:
-            return ak.contents.NumpyArray(result)
-
-    def identity_for(self, dtype: np.dtype | None):
-        if dtype is None:
-            dtype = self.preferred_dtype
-
-        if dtype in {np.timedelta64, np.datetime64}:
-            return np.timedelta64(0)
-        else:
-            return numpy.asarray(0, dtype=dtype)[()]
 
 
-class Prod(Reducer):
+class Prod(KernelReducer):
     name: Final = "prod"
     preferred_dtype: Final = np.int64
     needs_position: Final = False
 
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
         if array.dtype.kind.upper() == "M":
             raise ValueError(f"cannot compute the product (ak.prod) of {array.dtype!r}")
+
+        # Boolean kernels are special; the result is _not_ a boolean
         if array.dtype == np.bool_:
             result = array.backend.nplike.empty(
-                self.maybe_double_length(array.dtype.type, outlength),
-                dtype=np.dtype(np.bool_),
+                outlength,
+                # This kernel, unlike sum, returns bools!
+                dtype=np.bool_,
             )
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_prod_bool",
                     result.dtype.type,
                     array.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
                     array.data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-            result = array.backend.nplike.astype(
-                result, dtype=self.return_dtype(array.dtype)
-            )
-        elif array.dtype.type in (np.complex128, np.complex64):
-            result = array.backend.nplike.empty(
-                self.maybe_double_length(array.dtype.type, outlength),
-                dtype=self.return_dtype(array.dtype),
-            )
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_prod_complex",
-                    np.float64 if array.dtype.type == np.complex128 else np.float32,
-                    np.float64 if array.dtype.type == np.complex128 else np.float32,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                )
+            return ak.contents.NumpyArray(
+                array.backend.nplike.astype(
+                    result, dtype=self._promote_integer_rank(array.dtype)
+                ),
+                backend=array.backend,
             )
         else:
+            # View array data in kernel-supported dtype
+            kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
             result = array.backend.nplike.empty(
-                self.maybe_double_length(array.dtype.type, outlength),
-                dtype=self.return_dtype(array.dtype),
+                self._length_for_kernel(array.dtype.type, outlength),
+                dtype=self._promote_integer_rank(kernel_array_data.dtype),
             )
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_prod",
-                    result.dtype.type,
-                    array.dtype.type,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
+            if array.dtype.type in (np.complex128, np.complex64):
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_prod_complex",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                    )
+                )
+            else:
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_prod",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                    )
                 )
-            )
-        if array.dtype.type in (np.complex128, np.complex64):
-            return ak.contents.NumpyArray(result.view(array.dtype))
-        else:
-            return ak.contents.NumpyArray(result)
-
-    def identity_for(self, dtype: np.dtype | None):
-        if dtype is None:
-            dtype = self.preferred_dtype
 
-        if dtype in {np.timedelta64, np.datetime64}:
-            return np.timedelta64(0)
-        else:
-            return numpy.asarray(1, dtype=dtype)[()]
+            return ak.contents.NumpyArray(
+                result.view(self._promote_integer_rank(array.dtype)),
+                backend=array.backend,
+            )
 
 
-class Any(Reducer):
+class Any(KernelReducer):
     name: Final = "any"
     preferred_dtype: Final = np.bool_
     needs_position: Final = False
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.bool_
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
+        # View array data in kernel-supported dtype
+        kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
         result = array.backend.nplike.empty(outlength, dtype=np.bool_)
+
         if array.dtype.type in (np.complex128, np.complex64):
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_sum_bool_complex",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
         else:
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_sum_bool",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        return ak.contents.NumpyArray(result)
-
-    def identity_for(self, dtype: DTypeLike | None) -> float:
-        return False
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
 
-class All(Reducer):
+class All(KernelReducer):
     name: Final = "all"
     preferred_dtype: Final = np.bool_
     needs_position: Final = False
 
-    @classmethod
-    def return_dtype(cls, given_dtype):
-        return np.bool_
-
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
+        # View array data in kernel-supported dtype
+        kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
         result = array.backend.nplike.empty(outlength, dtype=np.bool_)
+
         if array.dtype.type in (np.complex128, np.complex64):
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_prod_bool_complex",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
         else:
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_prod_bool",
                     result.dtype.type,
-                    dtype,
+                    kernel_array_data.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
-                    array.data,
+                    kernel_array_data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        return ak.contents.NumpyArray(result)
-
-    def identity_for(self, dtype: DTypeLike | None) -> float:
-        return True
+        return ak.contents.NumpyArray(result, backend=array.backend)
 
 
-class Min(Reducer):
+class Min(KernelReducer):
     name: Final = "min"
     preferred_dtype: Final = np.float64
     needs_position: Final = False
 
     def __init__(self, initial: float | None):
         self._initial = initial
 
     @property
     def initial(self) -> float | None:
         return self._initial
 
-    def identity_for(self, dtype: DTypeLike | None) -> float:
+    def _identity_for(self, dtype: DTypeLike | None) -> float:
         dtype = np.dtype(dtype)
 
         assert (
             dtype.kind.upper() != "M"
         ), "datetime64/timedelta64 should be converted to int64 before reduction"
         if self._initial is None:
             if dtype in (
@@ -571,95 +576,98 @@
             ):
                 return np.iinfo(dtype).max
             else:
                 return np.inf
 
         return self._initial
 
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
-        result = array.backend.nplike.empty(
-            self.maybe_double_length(array.dtype.type, outlength), dtype=dtype
-        )
         if array.dtype == np.bool_:
+            result = array.backend.nplike.empty(outlength, dtype=np.bool_)
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_prod_bool",
                     result.dtype.type,
                     array.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
                     array.data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        elif array.dtype.type in (np.complex128, np.complex64):
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_min_complex",
-                    result.dtype.type,
-                    dtype,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                    self.identity_for(dtype),
-                )
-            )
+            return ak.contents.NumpyArray(result, backend=array.backend)
         else:
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_min",
-                    result.dtype.type,
-                    dtype,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                    self.identity_for(dtype),
-                )
+            # View array data in kernel-supported dtype
+            kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
+            result = array.backend.nplike.empty(
+                self._length_for_kernel(array.dtype.type, outlength),
+                dtype=kernel_array_data.dtype,
             )
-        if array.dtype.type in (np.complex128, np.complex64):
-            return ak.contents.NumpyArray(
-                array.backend.nplike.asarray(
-                    result.view(array.dtype), dtype=array.dtype
+            if array.dtype.type in (np.complex128, np.complex64):
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_min_complex",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                        self._identity_for(result.dtype),
+                    )
+                )
+            else:
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_min",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                        self._identity_for(result.dtype),
+                    )
                 )
-            )
-        else:
             return ak.contents.NumpyArray(
-                array.backend.nplike.asarray(result, dtype=array.dtype)
+                result.view(array.dtype), backend=array.backend
             )
 
 
-class Max(Reducer):
+class Max(KernelReducer):
     name: Final = "max"
     preferred_dtype: Final = np.float64
     needs_position: Final = False
 
     def __init__(self, initial):
         self._initial = initial
 
     @property
     def initial(self):
         return self._initial
 
-    def identity_for(self, dtype: DTypeLike | None):
+    def _identity_for(self, dtype: DTypeLike | None):
         dtype = np.dtype(dtype)
 
         assert (
             dtype.kind.upper() != "M"
         ), "datetime64/timedelta64 should be converted to int64 before reduction"
         if self._initial is None:
             if dtype in (
@@ -674,73 +682,76 @@
             ):
                 return np.iinfo(dtype).min
             else:
                 return -np.inf
 
         return self._initial
 
-    def apply(self, array, parents, outlength):
+    def apply(
+        self,
+        array: ak.contents.NumpyArray,
+        parents: ak.index.Index,
+        outlength: ShapeItem,
+    ) -> ak.contents.NumpyArray:
         assert isinstance(array, ak.contents.NumpyArray)
-        dtype = self.maybe_other_type(array.dtype)
-        result = array.backend.nplike.empty(
-            self.maybe_double_length(array.dtype.type, outlength), dtype=dtype
-        )
         if array.dtype == np.bool_:
+            result = array.backend.nplike.empty(outlength, dtype=np.bool_)
             assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
+            array.backend.maybe_kernel_error(
                 array.backend[
                     "awkward_reduce_sum_bool",
                     result.dtype.type,
                     array.dtype.type,
                     parents.dtype.type,
                 ](
                     result,
                     array.data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-        elif array.dtype.type in (np.complex128, np.complex64):
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_max_complex",
-                    result.dtype.type,
-                    dtype,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                    self.identity_for(dtype),
-                )
-            )
+            return ak.contents.NumpyArray(result, backend=array.backend)
         else:
-            assert parents.nplike is array.backend.index_nplike
-            array._handle_error(
-                array.backend[
-                    "awkward_reduce_max",
-                    result.dtype.type,
-                    dtype,
-                    parents.dtype.type,
-                ](
-                    result,
-                    array.data,
-                    parents.data,
-                    parents.length,
-                    outlength,
-                    self.identity_for(dtype),
-                )
+            # View array data in kernel-supported dtype
+            kernel_array_data = array.data.view(self._dtype_for_kernel(array.dtype))
+            result = array.backend.nplike.empty(
+                self._length_for_kernel(array.dtype.type, outlength),
+                dtype=kernel_array_data.dtype,
             )
-        if array.dtype.type in (np.complex128, np.complex64):
-            return ak.contents.NumpyArray(
-                array.backend.nplike.asarray(
-                    result.view(array.dtype), dtype=array.dtype
+            if array.dtype.type in (np.complex128, np.complex64):
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_max_complex",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                        self._identity_for(result.dtype),
+                    )
+                )
+            else:
+                assert parents.nplike is array.backend.index_nplike
+                array.backend.maybe_kernel_error(
+                    array.backend[
+                        "awkward_reduce_max",
+                        result.dtype.type,
+                        kernel_array_data.dtype.type,
+                        parents.dtype.type,
+                    ](
+                        result,
+                        kernel_array_data,
+                        parents.data,
+                        parents.length,
+                        outlength,
+                        self._identity_for(result.dtype),
+                    )
                 )
-            )
-        else:
             return ak.contents.NumpyArray(
-                array.backend.nplike.asarray(result, dtype=array.dtype)
+                result.view(array.dtype), backend=array.backend
             )
```

### Comparing `awkward-2.2.1/src/awkward/_regularize.py` & `awkward-2.2.2/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_slicing.py` & `awkward-2.2.2/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_typetracer.py` & `awkward-2.2.2/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_typing.py` & `awkward-2.2.2/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_util.py` & `awkward-2.2.2/src/awkward/_util.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_v2.py` & `awkward-2.2.2/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/cppyy.py` & `awkward-2.2.2/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/highlevel.py` & `awkward-2.2.2/src/awkward/highlevel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/index.py` & `awkward-2.2.2/src/awkward/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,42 +6,37 @@
 from awkward._nplikes import to_nplike
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
-from awkward._typing import Self
+from awkward._typing import Final, Self
 
-np = NumpyMetadata.instance()
-numpy = Numpy.instance()
+np: Final = NumpyMetadata.instance()
+numpy: Final = Numpy.instance()
 
 
-_dtype_to_form = {
+_dtype_to_form: Final = {
     np.dtype(np.int8): "i8",
     np.dtype(np.uint8): "u8",
     np.dtype(np.int32): "i32",
     np.dtype(np.uint32): "u32",
     np.dtype(np.int64): "i64",
 }
 
+_form_to_dtype: Final = {v: k for k, v in _dtype_to_form.items()}
 
-def _form_to_zero_length(form):
-    if form == "i8":
-        return Index8(numpy.zeros(0, dtype=np.int8))
-    elif form == "u8":
-        return IndexU8(numpy.zeros(0, dtype=np.uint8))
-    elif form == "i32":
-        return Index32(numpy.zeros(0, dtype=np.int32))
-    elif form == "u32":
-        return IndexU32(numpy.zeros(0, dtype=np.uint32))
-    elif form == "i64":
-        return Index64(numpy.zeros(0, dtype=np.int64))
-    else:
-        raise AssertionError(f"unrecognized Index form: {form!r}")
+
+def _form_to_zero_length(form: str) -> Index:
+    try:
+        dtype = _form_to_dtype[form]
+    except KeyError:
+        raise AssertionError(f"unrecognized Index form: {form!r}") from None
+    return Index(numpy.zeros(0, dtype=dtype))
 
 
 class Index:
     _expected_dtype = None
 
     def __init__(self, data, *, metadata=None, nplike=None):
         assert not isinstance(data, Index)
@@ -227,14 +222,22 @@
             return (
                 self.nplike.array_equal(self.data, other.data)
                 and self._data.dtype == other.data.dtype
             )
         else:
             return self.nplike.array_equal(self.data, other.data)
 
+    def _touch_data(self):
+        if not self.nplike.known_data:
+            self._data.touch_data()
+
+    def _touch_shape(self):
+        if not self.nplike.known_data:
+            self._data.touch_shape()
+
 
 class Index8(Index):
     _expected_dtype = np.dtype(np.int8)
 
 
 class IndexU8(Index):
     _expected_dtype = np.dtype(np.uint8)
```

### Comparing `awkward-2.2.1/src/awkward/jax.py` & `awkward-2.2.2/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/numba.py` & `awkward-2.2.2/src/awkward/numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/record.py` & `awkward-2.2.2/src/awkward/record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/typetracer.py` & `awkward-2.2.2/src/awkward/typetracer.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,36 +2,59 @@
 
 __all__ = [
     "is_unknown_array",
     "is_unknown_scalar",
     "empty_if_typetracer",
     "TypeTracerReport",
     "typetracer_with_report",
+    "PlaceholderArray",
+    "unknown_length",
 ]
 
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._behavior import behavior_of
+from awkward._errors import deprecate
 from awkward._layout import wrap_layout
+from awkward._nplikes.placeholder import PlaceholderArray
+from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import (
     TypeTracerReport,
     is_unknown_array,
     is_unknown_scalar,
     typetracer_with_report,
 )
 from awkward._typing import TypeVar
+from awkward.forms import Form
 from awkward.highlevel import Array, Record
 from awkward.operations.ak_to_layout import to_layout
 
 T = TypeVar("T", Array, Record)
 
 
-def empty_if_typetracer(array: T) -> T:
+def _length_0_1_if_typetracer(array: T, function):
     typetracer_backend = TypeTracerBackend.instance()
 
     layout = to_layout(array, allow_other=False)
     behavior = behavior_of(array)
 
     if layout.backend is typetracer_backend:
         layout._touch_data(True)
-        layout = layout.form.length_zero_array(highlevel=False)
+        layout = function(layout.form, highlevel=False)
 
     return wrap_layout(layout, behavior=behavior)
+
+
+def empty_if_typetracer(array: T) -> T:
+    deprecate(
+        "'empty_if_typetracer' is being replaced by 'length_zero_if_typetracer' (change name)",
+        "2.4.0",
+    )
+
+    return length_zero_if_typetracer(array)
+
+
+def length_zero_if_typetracer(array: T) -> T:
+    return _length_0_1_if_typetracer(array, Form.length_zero_array)
+
+
+def length_one_if_typetracer(array: T) -> T:
+    return _length_0_1_if_typetracer(array, Form.length_one_array)
```

### Comparing `awkward-2.2.1/src/awkward/_backends/cupy.py` & `awkward-2.2.2/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_backends/dispatch.py` & `awkward-2.2.2/src/awkward/_backends/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_backends/jax.py` & `awkward-2.2.2/src/awkward/_backends/jax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward_cpp
 
 import awkward as ak
-from awkward._backends.backend import Backend, KernelKeyType
+from awkward._backends.backend import Backend, KernelKeyType, UfuncLike
 from awkward._backends.dispatch import register_backend
 from awkward._kernels import JaxKernel
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Final
 
@@ -35,27 +35,16 @@
         self._jax = Jax.instance()
         self._numpy = Numpy.instance()
 
     def __getitem__(self, index: KernelKeyType) -> JaxKernel:
         # JAX uses Awkward's C++ kernels for index-only operations
         return JaxKernel(awkward_cpp.cpu_kernels.kernel[index], index)
 
-    def apply_reducer(
-        self,
-        reducer: ak._reducers.Reducer,
-        layout: ak.contents.NumpyArray,
-        parents: ak.index.Index,
-        outlength: int,
-    ) -> ak.contents.NumpyArray:
+    def prepare_reducer(self, reducer: ak._reducers.Reducer) -> ak._reducers.Reducer:
         from awkward._connect.jax import get_jax_reducer
 
-        jax_reducer = get_jax_reducer(reducer)
-        return jax_reducer.apply(layout, parents, outlength)
+        return get_jax_reducer(reducer)
 
-    def apply_ufunc(self, ufunc, method, args, kwargs):
+    def prepare_ufunc(self, ufunc: UfuncLike) -> UfuncLike:
         from awkward._connect.jax import get_jax_ufunc
 
-        if method != "__call__":
-            raise ValueError(f"unsupported ufunc method {method} called")
-
-        jax_ufunc = get_jax_ufunc(ufunc)
-        return jax_ufunc(*args, **kwargs)
+        return get_jax_ufunc(ufunc)
```

### Comparing `awkward-2.2.1/src/awkward/_backends/numpy.py` & `awkward-2.2.2/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/avro.py` & `awkward-2.2.2/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cling.py` & `awkward-2.2.2/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/hist.py` & `awkward-2.2.2/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numexpr.py` & `awkward-2.2.2/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numpy.py` & `awkward-2.2.2/src/awkward/_connect/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,19 @@
             args = []
             for x in inputs:
                 if isinstance(x, NumpyArray):
                     args.append(x._raw(nplike))
                 else:
                     args.append(x)
 
-            result = backend.apply_ufunc(ufunc, method, args, kwargs)
+            # Give backend a chance to change the ufunc implementation
+            impl = backend.prepare_ufunc(ufunc)
+
+            # Invoke ufunc
+            result = impl(*args, **kwargs)
 
             return (NumpyArray(result, backend=backend, parameters=parameters),)
 
         # Do we have a custom generic ufunc override (a function that accepts _all_ ufuncs)?
         for x in inputs:
             if isinstance(x, ak.contents.Content):
                 apply_ufunc = find_ufunc_generic(ufunc, x, behavior)
```

### Comparing `awkward-2.2.1/src/awkward/_connect/pyarrow.py` & `awkward-2.2.2/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/__init__.py` & `awkward-2.2.2/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T, typename C>
+template <typename T>
 __global__ void
-awkward_ListOffsetArray_compact_offsets(T* tooffsets,
-                                        const C* fromoffsets,
-                                        int64_t length,
-                                        uint64_t invocation_index,
-                                        uint64_t* err_code) {
+awkward_NumpyArray_contiguous_init(T* toptr,
+                                   int64_t skip,
+                                   int64_t stride,
+                                   uint64_t invocation_index,
+                                   uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
     int64_t thread_id = blockIdx.x * blockDim.x + threadIdx.x;
-    if (thread_id < length) {
-      int64_t diff = (int64_t)fromoffsets[0];
-      if (thread_id == 0) {
-        tooffsets[0] = 0;
-      }
-      tooffsets[thread_id + 1] = fromoffsets[thread_id + 1] - diff;
+    if (thread_id < skip) {
+      toptr[thread_id] = (thread_id * stride);
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T>
+template <typename T, typename C>
 __global__ void
-awkward_NumpyArray_contiguous_init(T* toptr,
-                                   int64_t skip,
-                                   int64_t stride,
+awkward_RegularArray_getitem_carry(T* tocarry,
+                                   const C* fromcarry,
+                                   int64_t lencarry,
+                                   int64_t size,
                                    uint64_t invocation_index,
                                    uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
-    int64_t thread_id = blockIdx.x * blockDim.x + threadIdx.x;
-    if (thread_id < skip) {
-      toptr[thread_id] = (thread_id * stride);
+    int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / size;
+    int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % size;
+
+    if (thread_id < lencarry) {
+      tocarry[(thread_id * size) + thready_id] =
+          (fromcarry[thread_id] * size) + thready_id;
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 template <typename T>
 __global__ void
-awkward_RegularArray_compact_offsets(T* tooffsets,
-                                     int64_t length,
-                                     int64_t size,
-                                     uint64_t invocation_index,
-                                     uint64_t* err_code) {
+awkward_RegularArray_localindex(T* toindex,
+                                int64_t size,
+                                int64_t length,
+                                uint64_t invocation_index,
+                                uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
-    int64_t thread_id = blockIdx.x * blockDim.x + threadIdx.x;
-    tooffsets[0] = 0;
+    int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / size;
+    int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % size;
+
     if (thread_id < length) {
-      tooffsets[thread_id + 1] = (thread_id + 1) * size;
+      toindex[((thread_id * size) + thready_id)] = thready_id;
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T, typename C>
+template <typename T>
 __global__ void
-awkward_RegularArray_getitem_carry(T* tocarry,
-                                   const C* fromcarry,
-                                   int64_t lencarry,
-                                   int64_t size,
-                                   uint64_t invocation_index,
-                                   uint64_t* err_code) {
+awkward_RegularArray_getitem_next_range(T* tocarry,
+                                        int64_t regular_start,
+                                        int64_t step,
+                                        int64_t length,
+                                        int64_t size,
+                                        int64_t nextsize,
+                                        uint64_t invocation_index,
+                                        uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
-    int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / size;
-    int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % size;
+    int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / nextsize;
+    int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % nextsize;
 
-    if (thread_id < lencarry) {
-      tocarry[(thread_id * size) + thready_id] =
-          (fromcarry[thread_id] * size) + thready_id;
+    if (thread_id < length) {
+      tocarry[(thread_id * nextsize) + thready_id] =
+          ((thread_id * size) + regular_start) + (thready_id * step);
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T>
+template <typename T, typename C>
 __global__ void
-awkward_RegularArray_getitem_next_range(T* tocarry,
-                                        int64_t regular_start,
-                                        int64_t step,
-                                        int64_t length,
-                                        int64_t size,
-                                        int64_t nextsize,
-                                        uint64_t invocation_index,
-                                        uint64_t* err_code) {
+awkward_RegularArray_getitem_next_range_spreadadvanced(T* toadvanced,
+                                                       const C* fromadvanced,
+                                                       int64_t length,
+                                                       int64_t nextsize,
+                                                       uint64_t invocation_index,
+                                                       uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
     int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / nextsize;
     int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % nextsize;
 
     if (thread_id < length) {
-      tocarry[(thread_id * nextsize) + thready_id] =
-          ((thread_id * size) + regular_start) + (thready_id * step);
+      toadvanced[(thread_id * nextsize) + thready_id] = fromadvanced[thread_id];
     }
+    toadvanced[(thread_id * nextsize) + thready_id] = fromadvanced[thread_id];
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T>
+template <typename T, typename C>
 __global__ void
-awkward_RegularArray_localindex(T* toindex,
-                                int64_t size,
-                                int64_t length,
-                                uint64_t invocation_index,
-                                uint64_t* err_code) {
+awkward_UnionArray_fillna(T* toindex,
+                          const C* fromindex,
+                          int64_t length,
+                          uint64_t invocation_index,
+                          uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
-    int64_t thread_id = (blockIdx.x * blockDim.x + threadIdx.x) / size;
-    int64_t thready_id = (blockIdx.x * blockDim.x + threadIdx.x) % size;
-
+    int64_t thread_id = blockIdx.x * blockDim.x + threadIdx.x;
     if (thread_id < length) {
-      toindex[((thread_id * size) + thready_id)] = thready_id;
+      toindex[thread_id] = fromindex[thread_id] >= 0 ? fromindex[thread_id] : 0;
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 // BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-template <typename T, typename C>
+template <typename T, typename C, typename U>
 __global__ void
-awkward_UnionArray_fillna(T* toindex,
-                          const C* fromindex,
-                          int64_t length,
-                          uint64_t invocation_index,
-                          uint64_t* err_code) {
+awkward_index_carry_nocheck(T* toindex,
+                            const C* fromindex,
+                            const U* carry,
+                            int64_t length,
+                            uint64_t invocation_index,
+                            uint64_t* err_code) {
   if (err_code[0] == NO_ERROR) {
     int64_t thread_id = blockIdx.x * blockDim.x + threadIdx.x;
     if (thread_id < length) {
-      toindex[thread_id] = fromindex[thread_id] >= 0 ? fromindex[thread_id] : 0;
+      toindex[thread_id] = fromindex[(int64_t)carry[thread_id]];
     }
   }
 }
```

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.2.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.2.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.2.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.2.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.2.2/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/jax/trees.py` & `awkward-2.2.2/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numba/arrayview.py` & `awkward-2.2.2/src/awkward/_connect/numba/arrayview.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,23 +100,23 @@
         print("################### " + function_name)  # noqa: T201
         print(code)  # noqa: T201
     namespace = {} if externals is None else dict(externals)
     exec(code, namespace)
     return namespace[function_name]
 
 
-def tonumbatype(form):
+def to_numbatype(form):
     if isinstance(form, ak.forms.EmptyForm):
-        return tonumbatype(form.to_NumpyForm(np.dtype(np.float64)))
+        return to_numbatype(form.to_NumpyForm(np.dtype(np.float64)))
 
     elif isinstance(form, ak.forms.NumpyForm):
         if len(form.inner_shape) == 0:
             return ak._connect.numba.layout.NumpyArrayType.from_form(form)
         else:
-            return tonumbatype(form.to_RegularForm())
+            return to_numbatype(form.to_RegularForm())
 
     elif isinstance(form, ak.forms.RegularForm):
         return ak._connect.numba.layout.RegularArrayType.from_form(form)
 
     elif isinstance(form, (ak.forms.ListForm, ak.forms.ListOffsetForm)):
         return ak._connect.numba.layout.ListArrayType.from_form(form)
 
@@ -192,15 +192,15 @@
         layout = ak.operations.to_layout(
             array,
             allow_record=False,
             allow_other=False,
         )
 
         return ArrayView(
-            tonumbatype(layout.form),
+            to_numbatype(layout.form),
             behavior,
             ak._lookup.Lookup(layout),
             0,
             0,
             len(layout),
             (),
         )
@@ -581,15 +581,15 @@
     def fromrecord(cls, record):
         behavior = behavior_of(record)
         layout = ak.operations.to_layout(record, allow_record=True, allow_other=False)
         assert isinstance(layout, ak.record.Record)
         arraylayout = layout.array
         return RecordView(
             ArrayView(
-                tonumbatype(arraylayout.form),
+                to_numbatype(arraylayout.form),
                 behavior,
                 ak._lookup.Lookup(arraylayout),
                 0,
                 0,
                 len(arraylayout),
                 (),
             ),
```

### Comparing `awkward-2.2.1/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.2.2/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numba/builder.py` & `awkward-2.2.2/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.2.2/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/numba/layout.py` & `awkward-2.2.2/src/awkward/_connect/numba/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
         return False
 
 
 class RegularArrayType(ContentType, ak._lookup.RegularLookup):
     @classmethod
     def from_form(cls, form):
         return RegularArrayType(
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.size,
             form.parameters,
         )
 
     def __init__(self, contenttype, size, parameters):
         super().__init__(
             name=f"ak.RegularArrayType({contenttype.name}, {size}, {json.dumps(parameters)})"
@@ -445,15 +445,15 @@
         if isinstance(form, ak.forms.ListForm):
             index_string = form.starts
         else:
             index_string = form.offsets
 
         return ListArrayType(
             cls.from_form_index(index_string),
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.parameters,
         )
 
     def __init__(self, indextype, contenttype, parameters):
         super().__init__(
             name=f"ak.ListArrayType({indextype.name}, {contenttype.name}, {json.dumps(parameters)})"
         )
@@ -531,15 +531,15 @@
 
 
 class IndexedArrayType(ContentType, ak._lookup.IndexedLookup):
     @classmethod
     def from_form(cls, form):
         return IndexedArrayType(
             cls.from_form_index(form.index),
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.parameters,
         )
 
     def __init__(self, indextype, contenttype, parameters):
         super().__init__(
             name=f"ak.IndexedArrayType({indextype.name}, {contenttype.name}, {json.dumps(parameters)})"
         )
@@ -625,15 +625,15 @@
 
 
 class IndexedOptionArrayType(ContentType, ak._lookup.IndexedOptionLookup):
     @classmethod
     def from_form(cls, form):
         return IndexedOptionArrayType(
             cls.from_form_index(form.index),
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.parameters,
         )
 
     def __init__(self, indextype, contenttype, parameters):
         super().__init__(
             name=f"ak.IndexedOptionArrayType({indextype.name}, {contenttype.name}, {json.dumps(parameters)})"
         )
@@ -736,15 +736,15 @@
 
 
 class ByteMaskedArrayType(ContentType, ak._lookup.ByteMaskedLookup):
     @classmethod
     def from_form(cls, form):
         return ByteMaskedArrayType(
             cls.from_form_index(form.mask),
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.valid_when,
             form.parameters,
         )
 
     def __init__(self, masktype, contenttype, valid_when, parameters):
         super().__init__(
             name=f"ak.ByteMaskedArrayType({masktype.name}, {contenttype.name}, {valid_when}, {json.dumps(parameters)})"
@@ -848,15 +848,15 @@
 
 
 class BitMaskedArrayType(ContentType, ak._lookup.BitMaskedLookup):
     @classmethod
     def from_form(cls, form):
         return BitMaskedArrayType(
             cls.from_form_index(form.mask),
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.valid_when,
             form.lsb_order,
             form.parameters,
         )
 
     def __init__(self, masktype, contenttype, valid_when, lsb_order, parameters):
         super().__init__(
@@ -980,15 +980,15 @@
         return self.contenttype.is_recordtype
 
 
 class UnmaskedArrayType(ContentType, ak._lookup.UnmaskedLookup):
     @classmethod
     def from_form(cls, form):
         return UnmaskedArrayType(
-            ak._connect.numba.arrayview.tonumbatype(form.content),
+            ak._connect.numba.arrayview.to_numbatype(form.content),
             form.parameters,
         )
 
     def __init__(self, contenttype, parameters):
         super().__init__(
             name=f"ak.UnmaskedArrayType({contenttype.name}, {json.dumps(parameters)})"
         )
@@ -1069,15 +1069,15 @@
         return self.contenttype.is_recordtype
 
 
 class RecordArrayType(ContentType, ak._lookup.RecordLookup):
     @classmethod
     def from_form(cls, form):
         return RecordArrayType(
-            [ak._connect.numba.arrayview.tonumbatype(x) for x in form.contents],
+            [ak._connect.numba.arrayview.to_numbatype(x) for x in form.contents],
             None if form.is_tuple else form.fields,
             form.parameters,
         )
 
     def __init__(self, contenttypes, fields, parameters):
         tmp1 = ", ".join(x.name for x in contenttypes)
         tmp2 = "," if len(contenttypes) == 1 else ""
@@ -1360,15 +1360,15 @@
 
 class UnionArrayType(ContentType, ak._lookup.UnionLookup):
     @classmethod
     def from_form(cls, form):
         return UnionArrayType(
             cls.from_form_index(form.tags),
             cls.from_form_index(form.index),
-            [ak._connect.numba.arrayview.tonumbatype(x) for x in form.contents],
+            [ak._connect.numba.arrayview.to_numbatype(x) for x in form.contents],
             form.parameters,
         )
 
     def __init__(self, tagstype, indextype, contenttypes, parameters):
         tmp1 = ", ".join(x.name for x in contenttypes)
         tmp2 = "," if len(contenttypes) == 1 else ""
         super().__init__(
```

### Comparing `awkward-2.2.1/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.2.2/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.2.2/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.2.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_nplikes/__init__.py` & `awkward-2.2.2/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_nplikes/array_module.py` & `awkward-2.2.2/src/awkward/_nplikes/array_module.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from awkward._nplikes.numpylike import (
     ArrayLike,
     IndexType,
     NumpyLike,
     NumpyMetadata,
     UniqueAllResult,
 )
+from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
 class ArrayModuleNumpyLike(NumpyLike):
@@ -26,35 +27,40 @@
     def asarray(
         self,
         obj,
         *,
         dtype: numpy.dtype | None = None,
         copy: bool | None = None,
     ) -> ArrayLike:
-        if copy:
+        if isinstance(obj, PlaceholderArray):
+            assert obj.dtype == dtype or dtype is None
+            return obj
+        elif copy:
             return self._module.array(obj, dtype=dtype, copy=True)
         elif copy is None:
             return self._module.asarray(obj, dtype=dtype)
         else:
             if getattr(obj, "dtype", dtype) != dtype:
                 raise ValueError(
                     "asarray was called with copy=False for an array of a different dtype"
                 )
             else:
                 return self._module.asarray(obj, dtype=dtype)
 
     def ascontiguousarray(self, x: ArrayLike) -> ArrayLike:
-        # Allow buffers to _pretend_ to be contiguous already
-        if x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous"):
+        if isinstance(x, PlaceholderArray):
             return x
-        return self._module.ascontiguousarray(x)
+        else:
+            return self._module.ascontiguousarray(x)
 
     def frombuffer(
         self, buffer, *, dtype: np.dtype | None = None, count: int = -1
     ) -> ArrayLike:
+        assert not isinstance(buffer, PlaceholderArray)
+        assert not isinstance(count, PlaceholderArray)
         return self._module.frombuffer(buffer, dtype=dtype, count=count)
 
     def zeros(
         self, shape: int | tuple[int, ...], *, dtype: np.dtype | None = None
     ) -> ArrayLike:
         return self._module.zeros(shape, dtype=dtype)
 
@@ -70,66 +76,79 @@
 
     def full(
         self, shape: int | tuple[int, ...], fill_value, *, dtype: np.dtype | None = None
     ) -> ArrayLike:
         return self._module.full(shape, fill_value, dtype=dtype)
 
     def zeros_like(self, x: ArrayLike, *, dtype: np.dtype | None = None) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.zeros_like(x, dtype=dtype)
 
     def ones_like(self, x: ArrayLike, *, dtype: np.dtype | None = None) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.ones_like(x, dtype=dtype)
 
     def full_like(
         self, x: ArrayLike, fill_value, *, dtype: np.dtype | None = None
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.full_like(x, fill_value, dtype=dtype)
 
     def arange(
         self,
         start: float | int,
         stop: float | int | None = None,
         step: float | int = 1,
         *,
         dtype: np.dtype | None = None,
     ) -> ArrayLike:
+        assert not isinstance(start, PlaceholderArray)
+        assert not isinstance(stop, PlaceholderArray)
+        assert not isinstance(step, PlaceholderArray)
         return self._module.arange(start, stop, step, dtype=dtype)
 
     def meshgrid(
         self, *arrays: ArrayLike, indexing: Literal["xy", "ij"] = "xy"
     ) -> list[ArrayLike]:
         return self._module.meshgrid(*arrays, indexing=indexing)
 
     ############################ testing
 
     def array_equal(
         self, x1: ArrayLike, x2: ArrayLike, *, equal_nan: bool = False
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.asarray(
             self._module.array_equal(x1, x2, equal_nan=equal_nan)
         )
 
     def searchsorted(
         self,
         x: ArrayLike,
         values: ArrayLike,
         *,
         side: Literal["left", "right"] = "left",
         sorter: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
+        assert not isinstance(values, PlaceholderArray)
+        assert not isinstance(sorter, PlaceholderArray)
         return self._module.searchsorted(x, values, side=side, sorter=sorter)
 
     ############################ manipulation
 
     def broadcast_arrays(self, *arrays: ArrayLike) -> list[ArrayLike]:
+        assert not any(isinstance(x, PlaceholderArray) for x in arrays)
         return self._module.broadcast_arrays(*arrays)
 
     def reshape(
         self, x: ArrayLike, shape: tuple[ShapeItem, ...], *, copy: bool | None = None
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         if copy is None:
             return self._module.reshape(x, shape)
         elif copy:
             return self._module.reshape(self._module.copy(x, order="C"), shape)
         else:
             result = self._module.asarray(x)
             try:
@@ -180,29 +199,35 @@
 
         if 0 <= index < length:
             return index
         else:
             raise IndexError(f"index value out of bounds (0, {length}): {index}")
 
     def nonzero(self, x: ArrayLike) -> tuple[ArrayLike, ...]:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.nonzero(x)
 
     def where(self, condition: ArrayLike, x1: ArrayLike, x2: ArrayLike) -> ArrayLike:
+        assert not isinstance(condition, PlaceholderArray)
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.where(condition, x1, x2)
 
     def unique_values(self, x: ArrayLike) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.unique(
             x,
             return_counts=False,
             return_index=False,
             return_inverse=False,
             equal_nan=False,
         )
 
     def unique_all(self, x: ArrayLike) -> UniqueAllResult:
+        assert not isinstance(x, PlaceholderArray)
         values, indices, inverse_indices, counts = self._module.unique(
             x, return_counts=True, return_index=True, return_inverse=True
         )
         # np.unique() flattens inverse indices, but they need to share x's shape
         # See https://github.com/numpy/numpy/issues/20638
         inverse_indices = inverse_indices.reshape(x.shape)
         return UniqueAllResult(values, indices, inverse_indices, counts)
@@ -211,207 +236,238 @@
         self,
         x: ArrayLike,
         *,
         axis: int = -1,
         descending: bool = False,
         stable: bool = True,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         # Note: this keyword argument is different, and the default is different.
         kind = "stable" if stable else "quicksort"
         res = self._module.sort(x, axis=axis, kind=kind)
         if descending:
             return self._module.flip(res, axis=axis)
         else:
             return res
 
     def concat(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int | None = 0,
     ) -> ArrayLike:
+        assert not any(isinstance(x, PlaceholderArray) for x in arrays)
         return self._module.concatenate(arrays, axis=axis, casting="same_kind")
 
     def repeat(
         self,
         x: ArrayLike,
         repeats: ArrayLike | int,
         *,
         axis: int | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
+        assert not isinstance(repeats, PlaceholderArray)
         return self._module.repeat(x, repeats=repeats, axis=axis)
 
-    def tile(self, x: ArrayLike, reps: int) -> ArrayLike:
-        return self._module.tile(x, reps)
-
     def stack(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int = 0,
     ) -> ArrayLike:
+        assert not any(isinstance(x, PlaceholderArray) for x in arrays)
         arrays = list(arrays)
         return self._module.stack(arrays, axis=axis)
 
     def packbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.packbits(x, axis=axis, bitorder=bitorder)
 
     def unpackbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.unpackbits(x, axis=axis, count=count, bitorder=bitorder)
 
     def broadcast_to(self, x: ArrayLike, shape: tuple[ShapeItem, ...]) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.broadcast_to(x, shape)
 
+    def strides(self, x: ArrayLike) -> tuple[ShapeItem, ...]:
+        return x.strides
+
     ############################ ufuncs
 
     def add(
         self, x1: ArrayLike, x2: ArrayLike, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.add(x1, x2, out=maybe_out)
 
     def logical_or(
         self, x1: ArrayLike, x2: ArrayLike, *, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.logical_or(x1, x2, out=maybe_out)
 
     def logical_and(
         self, x1: ArrayLike, x2: ArrayLike, *, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.logical_and(x1, x2, out=maybe_out)
 
     def logical_not(
         self, x: ArrayLike, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.logical_not(x, out=maybe_out)
 
     def sqrt(self, x: ArrayLike, maybe_out: ArrayLike | None = None) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.sqrt(x, out=maybe_out)
 
     def exp(self, x: ArrayLike, maybe_out: ArrayLike | None = None) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.exp(x, out=maybe_out)
 
     def divide(
         self, x1: ArrayLike, x2: ArrayLike, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.divide(x1, x2, out=maybe_out)
 
     ############################ almost-ufuncs
 
     def nan_to_num(
         self,
         x: ArrayLike,
         *,
         copy: bool = True,
         nan: int | float | None = 0.0,
         posinf: int | float | None = None,
         neginf: int | float | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.nan_to_num(
             x, copy=copy, nan=nan, posinf=posinf, neginf=neginf
         )
 
     def isclose(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         *,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
     ) -> ArrayLike:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._module.isclose(x1, x2, rtol=rtol, atol=atol, equal_nan=equal_nan)
 
     def isnan(self, x: ArrayLike) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.isnan(x)
 
     def all(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.all(x, axis=axis, keepdims=keepdims, out=maybe_out)
 
     def any(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.any(x, axis=axis, keepdims=keepdims, out=maybe_out)
 
     def min(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.min(x, axis=axis, keepdims=keepdims, out=maybe_out)
 
     def max(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.max(x, axis=axis, keepdims=keepdims, out=maybe_out)
 
     def count_nonzero(
         self, x: ArrayLike, *, axis: int | None = None, keepdims: bool = False
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.count_nonzero(x, axis=axis, keepdims=keepdims)
 
     def cumsum(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return self._module.cumsum(x, axis=axis, out=maybe_out)
 
     def array_str(
         self,
         x: ArrayLike,
         *,
         max_line_width: int | None = None,
         precision: int | None = None,
         suppress_small: bool | None = None,
     ):
+        assert not isinstance(x, PlaceholderArray)
         return self._module.array_str(
             x,
             max_line_width=max_line_width,
             precision=precision,
             suppress_small=suppress_small,
         )
 
     def astype(
         self, x: ArrayLike, dtype: numpy.dtype, *, copy: bool | None = True
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         return x.astype(dtype, copy=copy)
 
     def can_cast(self, from_: np.dtype | ArrayLike, to: np.dtype | ArrayLike) -> bool:
         return self._module.can_cast(from_, to, casting="same_kind")
 
     @classmethod
     def is_own_array(cls, obj) -> bool:
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/cupy.py` & `awkward-2.2.2/src/awkward/_nplikes/cupy.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike
+from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._typing import Final
 
 
 @register_nplike
 class Cupy(ArrayModuleNumpyLike):
     is_eager: Final = False
 
@@ -36,26 +37,32 @@
     @property
     def ndarray(self):
         return self._module.ndarray
 
     def frombuffer(
         self, buffer, *, dtype: numpy.dtype | None = None, count: int = -1
     ) -> ArrayLike:
+        assert not isinstance(buffer, PlaceholderArray)
+        assert not isinstance(count, PlaceholderArray)
         np_array = numpy.frombuffer(buffer, dtype=dtype, count=count)
         return self._module.asarray(np_array)
 
     def array_equal(self, x1: ArrayLike, x2: ArrayLike, *, equal_nan: bool = False):
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         if x1.shape != x2.shape:
             return False
         else:
             return self._module.all(x1 - x2 == 0)
 
     def repeat(
         self, x: ArrayLike, repeats: ArrayLike | int, *, axis: int | None = None
     ):
+        assert not isinstance(x, PlaceholderArray)
+        assert not isinstance(repeats, PlaceholderArray)
         if axis is not None:
             raise NotImplementedError(f"repeat for CuPy with axis={axis!r}")
         # https://github.com/cupy/cupy/issues/3849
         if isinstance(repeats, self._module.ndarray):
             all_stops = self._module.cumsum(repeats)
             parents = self._module.zeros(all_stops[-1].item(), dtype=int)
             stops, stop_counts = self._module.unique(all_stops[:-1], return_counts=True)
@@ -71,89 +78,90 @@
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         out = self._module.all(x, axis=axis, out=maybe_out)
         if axis is None and isinstance(out, self._module.ndarray):
             return out.item()
         else:
             return out
 
     def any(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         out = self._module.any(x, axis=axis, out=maybe_out)
         if axis is None and isinstance(out, self._module.ndarray):
             return out.item()
         else:
             return out
 
     def count_nonzero(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         out = self._module.count_nonzero(x, axis=axis)
         if axis is None and isinstance(out, self._module.ndarray):
             return out.item()
         else:
             return out
 
     def min(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         out = self._module.min(x, axis=axis, out=maybe_out)
         if axis is None and isinstance(out, self._module.ndarray):
             return out.item()
         else:
             return out
 
     def max(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         out = self._module.max(x, axis=axis, out=maybe_out)
         if axis is None and isinstance(out, self._module.ndarray):
             return out.item()
         else:
             return out
 
-    def array_str(
-        self, array, max_line_width=None, precision=None, suppress_small=None
-    ):
-        return self._module.array_str(array, max_line_width, precision, suppress_small)
-
     @classmethod
     def is_own_array_type(cls, type_: type) -> bool:
         """
         Args:
             type_: object to test
 
         Return `True` if the given object is a cupy buffer, otherwise `False`.
 
         """
         module, _, suffix = type_.__module__.partition(".")
         return module == "cupy"
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
-        return x.flags["C_CONTIGUOUS"] or (
-            x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous")
-        )
+        if isinstance(x, PlaceholderArray):
+            return True
+        else:
+            return x.flags["C_CONTIGUOUS"]
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/dispatch.py` & `awkward-2.2.2/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/_nplikes/jax.py` & `awkward-2.2.2/src/awkward/_nplikes/jax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike
+from awkward._nplikes.shape import ShapeItem
 from awkward._typing import Final
 
 
 @register_nplike
 class Jax(ArrayModuleNumpyLike):
     is_eager: Final = True
 
@@ -70,7 +71,14 @@
         return module == "jax"
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
         return True
 
     def ascontiguousarray(self, x: ArrayLike) -> ArrayLike:
         return x
+
+    def strides(self, x: ArrayLike) -> tuple[ShapeItem, ...]:
+        x.touch_shape()
+        out = (x._dtype.itemsize,)
+        for item in reversed(x._shape):
+            out = (item * out[0], *out)
+        return out
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/numpy.py` & `awkward-2.2.2/src/awkward/_nplikes/numpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
+from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
 @register_nplike
 class Numpy(ArrayModuleNumpyLike):
@@ -39,25 +40,27 @@
 
         Return `True` if the given object is a numpy buffer, otherwise `False`.
 
         """
         return issubclass(type_, numpy.ndarray)
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
-        return x.flags["C_CONTIGUOUS"] or (
-            x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous")
-        )
+        if isinstance(x, PlaceholderArray):
+            return True
+        else:
+            return x.flags["C_CONTIGUOUS"]
 
     def packbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ):
+        assert not isinstance(x, PlaceholderArray)
         if ak._util.numpy_at_least("1.17.0"):
             return numpy.packbits(x, axis=axis, bitorder=bitorder)
         else:
             assert axis is None, "unsupported argument value for axis given"
             if bitorder == "little":
                 if len(x) % 8 == 0:
                     ready_to_pack = x
@@ -77,14 +80,15 @@
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ):
+        assert not isinstance(x, PlaceholderArray)
         if ak._util.numpy_at_least("1.17.0"):
             return numpy.unpackbits(x, axis=axis, count=count, bitorder=bitorder)
         else:
             assert axis is None, "unsupported argument value for axis given"
             assert count is None, "unsupported argument value for count given"
             ready_to_bitswap = numpy.unpackbits(x)
             if bitorder == "little":
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/numpylike.py` & `awkward-2.2.2/src/awkward/_nplikes/numpylike.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,18 +441,14 @@
         repeats: ArrayLike | int,
         *,
         axis: int | None = None,
     ) -> ArrayLike:
         ...
 
     @abstractmethod
-    def tile(self, x: ArrayLike, reps: int) -> ArrayLike:
-        ...
-
-    @abstractmethod
     def stack(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int = 0,
     ) -> ArrayLike:
         ...
@@ -474,14 +470,18 @@
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> ArrayLike:
         ...
 
+    @abstractmethod
+    def strides(self, x: ArrayLike) -> tuple[ShapeItem, ...]:
+        ...
+
     ############################ ufuncs
 
     @abstractmethod
     def add(
         self, x1: ArrayLike, x2: ArrayLike, maybe_out: ArrayLike | None = None
     ) -> ArrayLike:
         ...
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/shape.py` & `awkward-2.2.2/src/awkward/_nplikes/shape.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from awkward._typing import Self, TypeAlias
 
-ShapeItem: TypeAlias = "int | _UnknownLength"
+ShapeItem: TypeAlias = "int | type[unknown_length]"
 
 
 class _UnknownLength:
     _name: str
 
     @classmethod
     def _new(cls, name: str) -> Self:
         self = super().__new__(cls)
         self._name = name
         return self
 
     def __new__(cls, *args, **kwargs):
         raise TypeError(
-            "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
+            "internal_error: the _UnknownLength class should never be directly instantiated"
         )
 
     def __add__(self, other) -> Self | NotImplemented:
         if isinstance(other, int) or other is self:
             return self
         else:
             return NotImplemented
@@ -52,14 +52,19 @@
             return self
         else:
             return NotImplemented
 
     __rfloordiv__ = __floordiv__
     __ifloordiv__ = __floordiv__
 
+    def __divmod__(self, other) -> tuple[Self, Self]:
+        return self, self
+
+    __rdivmod__ = __divmod__
+
     def __str__(self) -> str:
         return "##"
 
     def __repr__(self):
         return f"{__name__}.{self._name}"
 
     def __eq__(self, other) -> bool:
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/typetracer.py` & `awkward-2.2.2/src/awkward/_nplikes/typetracer.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from awkward._nplikes.numpylike import (
     ArrayLike,
     IndexType,
     NumpyLike,
     NumpyMetadata,
     UniqueAllResult,
 )
+from awkward._nplikes.placeholder import PlaceholderArray
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._regularize import is_integer, is_non_string_like_sequence
 from awkward._typing import (
     Any,
     Final,
     Literal,
     Self,
@@ -194,15 +195,15 @@
     @property
     def T(self) -> Self:
         return TypeTracerArray._new(
             self.dtype, self._shape[::-1], self.form_key, self.report
         )
 
     @property
-    def dtype(self):
+    def dtype(self) -> np.dtype:
         return self._dtype
 
     @property
     def size(self) -> ShapeItem:
         size = 1
         for item in self._shape:
             size *= item
@@ -210,68 +211,59 @@
 
     @property
     def shape(self) -> tuple[ShapeItem, ...]:
         self.touch_shape()
         return self._shape
 
     @property
-    def form_key(self):
+    def form_key(self) -> str | None:
         return self._form_key
 
     @form_key.setter
-    def form_key(self, value):
+    def form_key(self, value: str | None):
         if value is not None and not isinstance(value, str):
             raise TypeError("form_key must be None or a string")
         self._form_key = value
 
     @property
-    def report(self):
+    def report(self) -> TypeTracerReport | None:
         return self._report
 
     @report.setter
-    def report(self, value):
+    def report(self, value: TypeTracerReport | None):
         if value is not None and not isinstance(value, TypeTracerReport):
             raise TypeError("report must be None or a TypeTracerReport")
         self._report = value
 
     def touch_shape(self):
         if self._report is not None:
             self._report.touch_shape(self._form_key)
 
     def touch_data(self):
         if self._report is not None:
             self._report.touch_data(self._form_key)
 
     @property
-    def strides(self):
-        self.touch_shape()
-        out = (self._dtype.itemsize,)
-        for x in self._shape[:0:-1]:
-            out = (x * out[0], *out)
-        return out
-
-    @property
     def nplike(self) -> TypeTracer:
         return TypeTracer.instance()
 
     @property
     def ndim(self) -> int:
         self.touch_shape()
         return len(self._shape)
 
     def view(self, dtype: np.dtype) -> Self:
         dtype = np.dtype(dtype)
-        if (
-            self.itemsize != dtype.itemsize
-            and self.ndim >= 1
-            and self._shape[-1] is not None
-        ):
-            last = int(
-                round(self._shape[-1] * self.itemsize / np.dtype(dtype).itemsize)
-            )
+        if len(self._shape) >= 1:
+            last, remainder = divmod(self._shape[-1] * self.itemsize, dtype.itemsize)
+            if remainder is not unknown_length and remainder != 0:
+                raise ValueError(
+                    "new size of array with larger dtype must be a "
+                    "divisor of the total size in bytes (of the last axis of the array)"
+                )
             shape = self._shape[:-1] + (last,)
         else:
             shape = self._shape
         return self._new(
             dtype, shape=shape, form_key=self._form_key, report=self._report
         )
 
@@ -290,15 +282,15 @@
 
     def __array__(self, dtype=None):
         raise AssertionError(
             "bug in Awkward Array: attempt to convert TypeTracerArray into a concrete array"
         )
 
     @property
-    def itemsize(self):
+    def itemsize(self) -> int:
         return self._dtype.itemsize
 
     class _CTypes:
         data = 0
 
     @property
     def ctypes(self):
@@ -312,15 +304,15 @@
     def __getitem__(
         self,
         key: SupportsIndex
         | slice
         | Ellipsis
         | tuple[SupportsIndex | slice | Ellipsis | ArrayLike, ...]
         | ArrayLike,
-    ) -> Self:
+    ) -> Self | int | float | bool | complex:
         if not isinstance(key, tuple):
             key = (key,)
 
         # 1. Validate slice items
         has_seen_ellipsis = 0
         n_basic_non_ellipsis = 0
         n_advanced = 0
@@ -386,14 +378,17 @@
                 dimension_length = next(iter_shape)
                 # Advanced index
                 if n_advanced and (
                     isinstance(item, int)
                     or is_unknown_integer(item)
                     or is_unknown_array(item)
                 ):
+                    try_touch_data(item)
+                    try_touch_data(self)
+
                     if is_unknown_scalar(item):
                         item = self.nplike.promote_scalar(item)
 
                     # If this is the first advanced index, insert the location
                     if not advanced_shapes:
                         result_shape_parts.append(adjacent_advanced_shape)
                     # If a previous item was basic and we have an advanced shape
@@ -411,14 +406,17 @@
                         step,
                         slice_length,
                     ) = self.nplike.derive_slice_for_length(item, dimension_length)
                     result_shape_parts.append((slice_length,))
                     previous_item_is_basic = True
                 # Integer
                 elif isinstance(item, int) or is_unknown_integer(item):
+                    try_touch_data(item)
+                    try_touch_data(self)
+
                     item = self.nplike.promote_scalar(item)
 
                     if is_unknown_length(dimension_length) or is_unknown_integer(item):
                         continue
 
                     if not 0 <= item < dimension_length:
                         raise NotImplementedError("integer index out of bounds")
@@ -501,16 +499,19 @@
 @register_nplike
 class TypeTracer(NumpyLike):
     known_data: Final = False
     is_eager: Final = True
 
     def _apply_ufunc(self, ufunc, *inputs):
         for x in inputs:
+            assert not isinstance(x, PlaceholderArray)
             try_touch_data(x)
 
+        inputs = [x.content if isinstance(x, MaybeNone) else x for x in inputs]
+
         broadcasted = self.broadcast_arrays(*inputs)
         placeholders = [numpy.empty(0, x.dtype) for x in broadcasted]
 
         result = ufunc(*placeholders)
         if isinstance(result, numpy.ndarray):
             return TypeTracerArray._new(result.dtype, shape=broadcasted[0].shape)
         elif isinstance(result, tuple):
@@ -543,14 +544,16 @@
     def asarray(
         self,
         obj,
         *,
         dtype: numpy.dtype | None = None,
         copy: bool | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(obj, PlaceholderArray)
+
         if isinstance(obj, ak.index.Index):
             obj = obj.data
 
         if isinstance(obj, TypeTracerArray):
             form_key = obj._form_key
             report = obj._report
 
@@ -632,22 +635,24 @@
                 if dtype is None:
                     dtype = numpy.result_type(*flat_items)
                 return TypeTracerArray._new(dtype, shape=tuple(shape))
             else:
                 raise TypeError
 
     def ascontiguousarray(self, x: ArrayLike) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         return TypeTracerArray._new(
             x.dtype, shape=x.shape, form_key=x.form_key, report=x.report
         )
 
     def frombuffer(
         self, buffer, *, dtype: np.dtype | None = None, count: int = -1
     ) -> TypeTracerArray:
         for x in (buffer, count):
+            assert not isinstance(x, PlaceholderArray)
             try_touch_data(x)
         raise NotImplementedError
 
     def zeros(
         self, shape: ShapeItem | tuple[ShapeItem, ...], *, dtype: np.dtype | None = None
     ) -> TypeTracerArray:
         if not isinstance(shape, tuple):
@@ -671,48 +676,55 @@
     def full(
         self,
         shape: ShapeItem | tuple[ShapeItem, ...],
         fill_value,
         *,
         dtype: np.dtype | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(fill_value, PlaceholderArray)
         if not isinstance(shape, tuple):
             shape = (shape,)
         dtype = _scalar_type_of(fill_value) if dtype is None else dtype
         return TypeTracerArray._new(dtype, shape)
 
     def zeros_like(
         self, x: ArrayLike, *, dtype: np.dtype | None = None
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_shape(x)
         if is_unknown_scalar(x):
             return TypeTracerArray._new(dtype or x.dtype, shape=())
         else:
             return TypeTracerArray._new(dtype or x.dtype, shape=x.shape)
 
     def ones_like(
         self, x: ArrayLike, *, dtype: np.dtype | None = None
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_shape(x)
         return self.zeros_like(x, dtype=dtype)
 
     def full_like(
         self, x: ArrayLike, fill_value, *, dtype: np.dtype | None = None
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_shape(x)
         return self.zeros_like(x, dtype=dtype)
 
     def arange(
         self,
         start: float | int,
         stop: float | int | None = None,
         step: float | int = 1,
         *,
         dtype: np.dtype | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(start, PlaceholderArray)
+        assert not isinstance(stop, PlaceholderArray)
+        assert not isinstance(step, PlaceholderArray)
         try_touch_data(start)
         try_touch_data(stop)
         try_touch_data(step)
         if stop is None:
             start, stop = 0, start
 
         if is_integer(start) and is_integer(stop) and is_integer(step):
@@ -723,14 +735,15 @@
         default_int_type = np.int64 if (ak._util.win or ak._util.bits32) else np.int32
         return TypeTracerArray._new(dtype or default_int_type, (length,))
 
     def meshgrid(
         self, *arrays: ArrayLike, indexing: Literal["xy", "ij"] = "xy"
     ) -> list[TypeTracerArray]:
         for x in arrays:
+            assert not isinstance(x, PlaceholderArray)
             try_touch_data(x)
 
             assert x.ndim == 1
 
         shape = tuple(x.size for x in arrays)
         if indexing == "xy":
             shape[:2] = shape[1], shape[0]
@@ -739,26 +752,31 @@
         return [TypeTracerArray._new(dtype, shape=shape) for _ in arrays]
 
     ############################ testing
 
     def array_equal(
         self, x1: ArrayLike, x2: ArrayLike, *, equal_nan: bool = False
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         try_touch_data(x1)
         try_touch_data(x2)
         return TypeTracerArray._new(np.bool_, shape=())
 
     def searchsorted(
         self,
         x: ArrayLike,
         values: ArrayLike,
         *,
         side: Literal["left", "right"] = "left",
         sorter: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
+        assert not isinstance(values, PlaceholderArray)
+        assert not isinstance(sorter, PlaceholderArray)
         try_touch_data(x)
         try_touch_data(values)
         try_touch_data(sorter)
         if (
             not (
                 is_unknown_length(x.size)
                 or sorter is None
@@ -769,14 +787,15 @@
             raise ValueError("x.size should equal sorter.size")
 
         return TypeTracerArray._new(x.dtype, (values.size,))
 
     ############################ manipulation
 
     def promote_scalar(self, obj) -> TypeTracerArray:
+        assert not isinstance(obj, PlaceholderArray)
         if is_unknown_scalar(obj):
             return obj
         elif isinstance(obj, (Number, bool)):
             # TODO: statically define these types for all nplikes
             as_array = numpy.asarray(obj)
             return TypeTracerArray._new(as_array.dtype, ())
         else:
@@ -928,14 +947,15 @@
                     raise ValueError(
                         "known component of shape does not match broadcast result"
                     )
         return tuple(result)
 
     def broadcast_arrays(self, *arrays: ArrayLike) -> list[TypeTracerArray]:
         for x in arrays:
+            assert not isinstance(x, PlaceholderArray)
             try_touch_data(x)
 
         if len(arrays) == 0:
             return []
 
         all_arrays = []
         for x in arrays:
@@ -947,19 +967,37 @@
         shape = self.broadcast_shapes(*shapes)
 
         return [TypeTracerArray._new(x.dtype, shape=shape) for x in all_arrays]
 
     def broadcast_to(
         self, x: ArrayLike, shape: tuple[ShapeItem, ...]
     ) -> TypeTracerArray:
-        raise NotImplementedError
+        assert not isinstance(x, PlaceholderArray)
+        try_touch_data(x)
+        new_shape = self.broadcast_shapes(x.shape, shape)
+        # broadcast_to is asymmetric, whilst broadcast_shapes is not
+        # rather than implement broadcasting logic here, let's just santitise the result
+        # the above broadcasting result can either be equal to `shape`, have greater number dimensions,
+        # and/or have differing dimensions we only want the case where the shape is equal
+        if len(new_shape) != len(shape):
+            raise ValueError
+
+        for result, intended in zip(new_shape, shape):
+            if intended is unknown_length:
+                continue
+            if result is unknown_length:
+                continue
+            if intended != result:
+                raise ValueError
+        return TypeTracerArray._new(x.dtype, shape=new_shape)
 
     def reshape(
         self, x: ArrayLike, shape: tuple[ShapeItem, ...], *, copy: bool | None = None
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         x.touch_shape()
 
         size = x.size
 
         # Validate new shape to ensure that it only contains at-most one placeholder
         n_placeholders = 0
         new_size = 1
@@ -994,38 +1032,45 @@
     def cumsum(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         if axis is None:
             return TypeTracerArray._new(x.dtype, (x.size,))
         else:
             assert self._axis_is_valid(axis, x.ndim)
             return TypeTracerArray._new(x.dtype, x.shape)
 
     def nonzero(self, x: ArrayLike) -> tuple[TypeTracerArray, ...]:
+        assert not isinstance(x, PlaceholderArray)
         # array
         try_touch_data(x)
         return (TypeTracerArray._new(np.int64, (unknown_length,)),) * len(x.shape)
 
     def where(
         self, condition: ArrayLike, x1: ArrayLike, x2: ArrayLike
     ) -> TypeTracerArray:
+        assert not isinstance(condition, PlaceholderArray)
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         condition, x1, x2 = self.broadcast_arrays(condition, x1, x2)
         result_dtype = numpy.result_type(x1, x2)
         return TypeTracerArray._new(result_dtype, shape=condition.shape)
 
     def unique_values(self, x: ArrayLike) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return TypeTracerArray._new(x.dtype, shape=(unknown_length,))
 
     def unique_all(self, x: ArrayLike) -> UniqueAllResult:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return UniqueAllResult(
             TypeTracerArray._new(x.dtype, shape=(unknown_length,)),
             TypeTracerArray._new(np.int64, shape=(unknown_length,)),
             TypeTracerArray._new(np.int64, shape=x.shape),
             TypeTracerArray._new(np.int64, shape=(unknown_length,)),
         )
@@ -1034,28 +1079,30 @@
         self,
         x: ArrayLike,
         *,
         axis: int = -1,
         descending: bool = False,
         stable: bool = True,
     ) -> ArrayLike:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return TypeTracerArray._new(x.dtype, shape=x.shape)
 
     def concat(self, arrays, *, axis: int | None = 0) -> TypeTracerArray:
         if axis is None:
             assert all(x.ndim == 1 for x in arrays)
         elif axis != 0:
             raise NotImplementedError("concat with axis != 0")
         for x in arrays:
             try_touch_data(x)
 
         inner_shape = None
         emptyarrays = []
         for x in arrays:
+            assert not isinstance(x, PlaceholderArray)
             if inner_shape is None:
                 inner_shape = x.shape[1:]
             elif inner_shape != x.shape[1:]:
                 raise ValueError(
                     "inner dimensions don't match in concatenate: {} vs {}".format(
                         inner_shape, x.shape[1:]
                     )
@@ -1072,216 +1119,251 @@
     def repeat(
         self,
         x: ArrayLike,
         repeats: ArrayLike | int,
         *,
         axis: int | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
+        assert not isinstance(repeats, PlaceholderArray)
         try_touch_data(x)
         try_touch_data(repeats)
 
         if axis is None:
             size = x.size
-            if isinstance(repeats, TypeTracerArray) and repeats.ndim > 0:
-                raise NotImplementedError
+            if is_unknown_array(repeats):
+                size = unknown_length
             else:
                 size = size * self.index_as_shape_item(repeats)
             return TypeTracerArray._new(x.dtype, (size,))
         else:
             shape = list(x.shape)
             if isinstance(repeats, TypeTracerArray) and repeats.ndim > 0:
                 raise NotImplementedError
             else:
                 shape[axis] = shape[axis] * self.index_as_shape_item(repeats)
             return TypeTracerArray._new(x.dtype, shape=tuple(shape))
 
-    def tile(self, x: ArrayLike, reps: int) -> TypeTracerArray:
-        try_touch_data(x)
-        raise NotImplementedError
-
     def stack(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int = 0,
     ) -> TypeTracerArray:
         for x in arrays:
+            assert not isinstance(x, PlaceholderArray)
             try_touch_data(x)
         raise NotImplementedError
 
     def packbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         raise NotImplementedError
 
     def unpackbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         raise NotImplementedError
 
+    def strides(self, x: ArrayLike) -> tuple[ShapeItem, ...]:
+        assert not isinstance(x, PlaceholderArray)
+        x.touch_shape()
+        out = (x._dtype.itemsize,)
+        for item in reversed(x._shape):
+            out = (item * out[0], *out)
+        return out
+
     ############################ ufuncs
 
     def add(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
         return self._apply_ufunc(numpy.add, x1, x2)
 
     def logical_and(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
         return self._apply_ufunc(numpy.logical_and, x1, x2)
 
     def logical_or(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._apply_ufunc(numpy.logical_or, x1, x2)
 
     def logical_not(
         self, x: ArrayLike, maybe_out: ArrayLike | None = None
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         return self._apply_ufunc(numpy.logical_not, x)
 
     def sqrt(self, x: ArrayLike, maybe_out: ArrayLike | None = None) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         return self._apply_ufunc(numpy.sqrt, x)
 
     def exp(self, x: ArrayLike, maybe_out: ArrayLike | None = None) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         return self._apply_ufunc(numpy.exp, x)
 
     def divide(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         return self._apply_ufunc(numpy.divide, x1, x2)
 
     ############################ almost-ufuncs
 
     def nan_to_num(
         self,
         x: ArrayLike,
         *,
         copy: bool = True,
         nan: int | float | None = 0.0,
         posinf: int | float | None = None,
         neginf: int | float | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return TypeTracerArray._new(x.dtype, shape=x.shape)
 
     def isclose(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
         *,
         rtol: float = 1e-5,
         atol: float = 1e-8,
         equal_nan: bool = False,
     ) -> TypeTracerArray:
+        assert not isinstance(x1, PlaceholderArray)
+        assert not isinstance(x2, PlaceholderArray)
         try_touch_data(x1)
         try_touch_data(x2)
         out, _ = self.broadcast_arrays(x1, x2)
         return TypeTracerArray._new(np.bool_, shape=out.shape)
 
     def isnan(self, x: ArrayLike) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return TypeTracerArray._new(np.bool_, shape=x.shape)
 
     ############################ reducers
 
     def all(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         if axis is None:
             return TypeTracerArray._new(np.bool_, shape=())
         else:
             raise NotImplementedError
 
     def any(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         if axis is None:
             return TypeTracerArray._new(np.bool_, shape=())
         else:
             raise NotImplementedError
 
     def count_nonzero(
         self, x: ArrayLike, *, axis: int | None = None, keepdims: bool = False
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
-        raise NotImplementedError
+        if axis is None:
+            return TypeTracerArray._new(np.intp, shape=())
+        else:
+            raise NotImplementedError
 
     def min(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         raise NotImplementedError
 
     def max(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
-        raise NotImplementedError
+        if axis is None:
+            return TypeTracerArray._new(x.dtype, shape=())
+        else:
+            raise NotImplementedError
 
     def array_str(
         self,
         x: ArrayLike,
         *,
         max_line_width: int | None = None,
         precision: int | None = None,
         suppress_small: bool | None = None,
     ):
+        assert not isinstance(x, PlaceholderArray)
         try_touch_data(x)
         return "[## ... ##]"
 
     def astype(
         self, x: ArrayLike, dtype: numpy.dtype, *, copy: bool | None = True
     ) -> TypeTracerArray:
+        assert not isinstance(x, PlaceholderArray)
         x.touch_data()
         return TypeTracerArray._new(np.dtype(dtype), x.shape)
 
     def can_cast(self, from_: np.dtype | ArrayLike, to: np.dtype | ArrayLike) -> bool:
         return numpy.can_cast(from_, to, casting="same_kind")
 
     @classmethod
@@ -1289,14 +1371,15 @@
         return issubclass(type_, TypeTracerArray)
 
     @classmethod
     def is_own_array(cls, obj) -> bool:
         return cls.is_own_array_type(type(obj))
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
+        assert not isinstance(x, PlaceholderArray)
         return True
 
 
 def _attach_report(
     layout: ak.contents.Content, form: ak.forms.Form, report: TypeTracerReport
 ):
     if isinstance(layout, (ak.contents.BitMaskedArray, ak.contents.ByteMaskedArray)):
```

### Comparing `awkward-2.2.1/src/awkward/_nplikes/ufuncs.py` & `awkward-2.2.2/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/behaviors/categorical.py` & `awkward-2.2.2/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/behaviors/mixins.py` & `awkward-2.2.2/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/behaviors/string.py` & `awkward-2.2.2/src/awkward/behaviors/string.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,28 +143,14 @@
     return wrap_layout(ak.contents.NumpyArray(out), behavior)
 
 
 def _string_notequal(one, two):
     return ~_string_equal(one, two)
 
 
-def _string_broadcast(layout, offsets):
-    index_nplike = layout.backend.index_nplike
-    offsets = index_nplike.asarray(offsets)
-    counts = offsets[1:] - offsets[:-1]
-    if ak._util.win or ak._util.bits32:
-        counts = index_nplike.astype(counts, dtype=np.int32)
-    parents = index_nplike.repeat(
-        index_nplike.arange(counts.size, dtype=counts.dtype), counts
-    )
-    return ak.contents.IndexedArray(
-        ak.index.Index64(parents, nplike=index_nplike), layout
-    ).project()
-
-
 def _string_numba_typer(viewtype):
     import numba
 
     if viewtype.type.parameters["__array__"] == "string":
         return numba.types.string
     else:
         return numba.cpython.charseq.bytes_type
@@ -263,17 +249,14 @@
     behavior["__typestr__", "string"] = "string"
 
     behavior[ufuncs.equal, "bytestring", "bytestring"] = _string_equal
     behavior[ufuncs.equal, "string", "string"] = _string_equal
     behavior[ufuncs.not_equal, "bytestring", "bytestring"] = _string_notequal
     behavior[ufuncs.not_equal, "string", "string"] = _string_notequal
 
-    behavior["__broadcast__", "bytestring"] = _string_broadcast
-    behavior["__broadcast__", "string"] = _string_broadcast
-
     behavior["__numba_typer__", "bytestring"] = _string_numba_typer
     behavior["__numba_lower__", "bytestring"] = _string_numba_lower
     behavior["__numba_typer__", "string"] = _string_numba_typer
     behavior["__numba_lower__", "string"] = _string_numba_lower
 
     behavior["__cast__", str] = _cast_bytes_or_str_to_string
     behavior["__cast__", bytes] = _cast_bytes_or_str_to_string
```

### Comparing `awkward-2.2.1/src/awkward/contents/__init__.py` & `awkward-2.2.2/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/contents/bitmaskedarray.py` & `awkward-2.2.2/src/awkward/contents/bitmaskedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import json
 import math
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     type_parameters_equal,
 )
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.forms.bitmaskedform import BitMaskedForm
+from awkward.forms.form import Form
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
+    from awkward.contents import IndexedOptionArray
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 @final
 class BitMaskedArray(Content):
@@ -186,15 +189,15 @@
         self._init(parameters, content.backend)
 
     @property
     def mask(self):
         return self._mask
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     @property
     def valid_when(self):
         return self._valid_when
 
     @property
@@ -242,15 +245,15 @@
         lsb_order,
         *,
         parameters=None,
     ):
         if content.is_union or content.is_indexed or content.is_option:
             backend = content.backend
             index = ak.index.Index64.empty(mask.length * 8, backend.index_nplike)
-            Content._selfless_handle_error(
+            backend.maybe_kernel_error(
                 backend[
                     "awkward_BitMaskedArray_to_IndexedOptionArray",
                     index.dtype.type,
                     mask.dtype.type,
                 ](
                     index.raw(backend.nplike),
                     mask.data,
@@ -271,26 +274,33 @@
                 content,
                 valid_when,
                 length,
                 lsb_order,
                 parameters=parameters,
             )
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> BitMaskedForm:
         form_key = getkey(self)
         return self.form_cls(
             self._mask.form,
             self._content._form_with_key(getkey),
             self._valid_when,
             self._lsb_order,
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "mask")
         container[key] = ak._util.native_to_byteorder(
             self._mask.raw(backend.index_nplike), byteorder
         )
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
@@ -301,28 +311,26 @@
             self._content._to_typetracer(False),
             self._valid_when,
             unknown_length if forget_length else self.length,
             self._lsb_order,
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._mask.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._mask._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._mask.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._mask._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<BitMaskedArray valid_when="]
@@ -336,23 +344,23 @@
         out.append("\n")
         out.append(self._mask._repr(indent + "    ", "<mask>", "</mask>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</BitMaskedArray>")
         out.append(post)
         return "".join(out)
 
-    def to_IndexedOptionArray64(self):
+    def to_IndexedOptionArray64(self) -> IndexedOptionArray:
         index = ak.index.Index64.empty(
             self._mask.length * 8, self._backend.index_nplike
         )
         assert (
             index.nplike is self._backend.nplike
             and self._mask.nplike is self._backend.nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_BitMaskedArray_to_IndexedOptionArray",
                 index.dtype.type,
                 self._mask.dtype.type,
             ](
                 index.raw(self._backend.nplike),
                 self._mask.data,
@@ -369,15 +377,15 @@
         bytemask = ak.index.Index8.empty(
             self._mask.length * 8, self._backend.index_nplike
         )
         assert (
             bytemask.nplike is self._backend.nplike
             and self._mask.nplike is self._backend.nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_BitMaskedArray_to_ByteMaskedArray",
                 bytemask.dtype.type,
                 self._mask.dtype.type,
             ](
                 bytemask.data,
                 self._mask.data,
@@ -435,15 +443,15 @@
         bytemask = ak.index.Index8.empty(
             self._mask.length * 8, self._backend.index_nplike
         )
         assert (
             bytemask.nplike is self._backend.nplike
             and self._mask.nplike is self._backend.nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_BitMaskedArray_to_ByteMaskedArray",
                 bytemask.dtype.type,
                 self._mask.dtype.type,
             ](
                 bytemask.data,
                 self._mask.data,
@@ -502,15 +510,17 @@
             parameters=None,
         )
 
     def _carry(self, carry: Index, allow_lazy: bool) -> Content:
         assert isinstance(carry, ak.index.Index)
         return self.to_ByteMaskedArray()._carry(carry, allow_lazy)
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return self.to_ByteMaskedArray()._getitem_next_jagged(
             slicestarts, slicestops, slicecontent, tail
         )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
@@ -542,33 +552,33 @@
 
         else:
             raise AssertionError(repr(head))
 
     def project(self, mask=None):
         return self.to_ByteMaskedArray().project(mask)
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         return self.to_ByteMaskedArray._offsets_and_flattened(axis, depth)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
             ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         out = self.to_IndexedOptionArray64()._mergemany(others)
 
         if all(
             isinstance(x, BitMaskedArray)
@@ -673,15 +683,15 @@
     def _remove_structure(self, backend, options):
         branch, depth = self.branch_depth
         if branch or options["drop_nones"] or depth > 1:
             return self.project()._remove_structure(backend, options)
         else:
             return [self]
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.to_ByteMaskedArray()._drop_none()
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if self._backend.nplike.known_data:
             content = self._content[0 : self._length]
```

### Comparing `awkward-2.2.1/src/awkward/contents/bytemaskedarray.py` & `awkward-2.2.2/src/awkward/contents/bytemaskedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import json
 import math
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.bytemaskedform import ByteMaskedForm
+from awkward.forms.form import Form
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
+    from awkward.contents import IndexedOptionArray
+
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 @final
 class ByteMaskedArray(Content):
     """
@@ -134,15 +138,15 @@
         self._init(parameters, content.backend)
 
     @property
     def mask(self):
         return self._mask
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     @property
     def valid_when(self):
         return self._valid_when
 
     form_cls: Final = ByteMaskedForm
@@ -173,15 +177,15 @@
         valid_when,
         *,
         parameters=None,
     ):
         if content.is_union or content.is_indexed or content.is_option:
             backend = content.backend
             index = ak.index.Index64.empty(mask.length, nplike=backend.index_nplike)
-            Content._selfless_handle_error(
+            backend.maybe_kernel_error(
                 backend[
                     "awkward_ByteMaskedArray_toIndexedOptionArray",
                     index.dtype.type,
                     mask.dtype.type,
                 ](
                     index.data,
                     mask.data,
@@ -194,25 +198,32 @@
             else:
                 return ak.contents.IndexedOptionArray.simplified(
                     index, content, parameters=parameters
                 )
         else:
             return cls(mask, content, valid_when, parameters=parameters)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> ByteMaskedForm:
         form_key = getkey(self)
         return self.form_cls(
             self._mask.form,
             self._content._form_with_key(getkey),
             self._valid_when,
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "mask")
         container[key] = ak._util.native_to_byteorder(
             self._mask.raw(backend.index_nplike), byteorder
         )
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
@@ -222,28 +233,26 @@
         return ByteMaskedArray(
             mask.forget_length() if forget_length else mask,
             self._content._to_typetracer(False),
             self._valid_when,
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._mask.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._mask._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._mask.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._mask._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._mask.length
 
     def _forget_length(self):
         return ByteMaskedArray(
             self._mask.forget_length(),
             self._content,
             self._valid_when,
@@ -263,23 +272,23 @@
         out.append("\n")
         out.append(self._mask._repr(indent + "    ", "<mask>", "</mask>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</ByteMaskedArray>")
         out.append(post)
         return "".join(out)
 
-    def to_IndexedOptionArray64(self):
+    def to_IndexedOptionArray64(self) -> IndexedOptionArray:
         index = ak.index.Index64.empty(
             self._mask.length, nplike=self._backend.index_nplike
         )
         assert (
             index.nplike is self._backend.index_nplike
             and self._mask.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ByteMaskedArray_toIndexedOptionArray",
                 index.dtype.type,
                 self._mask.dtype.type,
             ](
                 index.data,
                 self._mask.data,
@@ -419,15 +428,15 @@
     def _nextcarry_outindex(self) -> tuple[int, ak.index.Index64, ak.index.Index64]:
         _numnull = ak.index.Index64.empty(1, nplike=self._backend.index_nplike)
 
         assert (
             _numnull.nplike is self._backend.index_nplike
             and self._mask.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ByteMaskedArray_numnull",
                 _numnull.dtype.type,
                 self._mask.dtype.type,
             ](
                 _numnull.data,
                 self._mask.data,
@@ -444,15 +453,15 @@
             self.length, nplike=self._backend.index_nplike
         )
         assert (
             nextcarry.nplike is self._backend.index_nplike
             and outindex.nplike is self._backend.index_nplike
             and self._mask.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ByteMaskedArray_getitem_nextcarry_outindex",
                 nextcarry.dtype.type,
                 outindex.dtype.type,
                 self._mask.dtype.type,
             ](
                 nextcarry.data,
@@ -494,15 +503,15 @@
         assert (
             outindex.nplike is self._backend.index_nplike
             and slicestarts.nplike is self._backend.index_nplike
             and slicestops.nplike is self._backend.index_nplike
             and reducedstarts.nplike is self._backend.nplike
             and reducedstops.nplike is self._backend.nplike
         )
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_MaskedArray_getitem_next_jagged_project",
                 outindex.dtype.type,
                 slicestarts.dtype.type,
                 slicestops.dtype.type,
                 reducedstarts.dtype.type,
                 reducedstops.dtype.type,
@@ -520,15 +529,17 @@
         next = self._content._carry(nextcarry, True)
         out = next._getitem_next_jagged(reducedstarts, reducedstops, slicecontent, tail)
 
         return ak.contents.IndexedOptionArray.simplified(
             outindex, out, parameters=self._parameters
         )
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return self._getitem_next_jagged_generic(
             slicestarts, slicestops, slicecontent, tail
         )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
@@ -582,15 +593,15 @@
                 mask_length, nplike=self._backend.index_nplike
             )
             assert (
                 nextmask.nplike is self._backend.index_nplike
                 and mask.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ByteMaskedArray_overlay_mask",
                     nextmask.dtype.type,
                     mask.dtype.type,
                     self._mask.dtype.type,
                 ](
                     nextmask.data,
@@ -607,15 +618,15 @@
             return next.project()
 
         else:
             assert (
                 _numnull.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ByteMaskedArray_numnull",
                     _numnull.dtype.type,
                     self._mask.dtype.type,
                 ](
                     _numnull.data,
                     self._mask.data,
@@ -627,30 +638,30 @@
             nextcarry = ak.index.Index64.empty(
                 mask_length - numnull, nplike=self._backend.index_nplike
             )
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ByteMaskedArray_getitem_nextcarry",
                     nextcarry.dtype.type,
                     self._mask.dtype.type,
                 ](
                     nextcarry.data,
                     self._mask.data,
                     mask_length,
                     self._valid_when,
                 )
             )
 
             return self._content._carry(nextcarry, False)
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
 
             next = self._content._carry(nextcarry, False)
@@ -673,15 +684,15 @@
                 )
 
                 assert (
                     outoffsets.nplike is self._backend.index_nplike
                     and outindex.nplike is self._backend.index_nplike
                     and offsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_flatten_none2empty",
                         outoffsets.dtype.type,
                         outindex.dtype.type,
                         offsets.dtype.type,
                     ](
                         outoffsets.data,
@@ -689,30 +700,30 @@
                         outindex.length,
                         offsets.data,
                         offsets.length,
                     )
                 )
                 return (outoffsets, flattened)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
             ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         if all(
             isinstance(x, ByteMaskedArray) and x._valid_when == self._valid_when
             for x in others
         ):
@@ -822,15 +833,15 @@
         mask_length = self._mask.length
 
         _numnull = ak.index.Index64.empty(1, nplike=self._backend.index_nplike)
         assert (
             _numnull.nplike is self._backend.index_nplike
             and self._mask.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ByteMaskedArray_numnull",
                 _numnull.dtype.type,
                 self._mask.dtype.type,
             ](
                 _numnull.data,
                 self._mask.data,
@@ -853,15 +864,15 @@
         assert (
             nextcarry.nplike is self._backend.index_nplike
             and nextparents.nplike is self._backend.index_nplike
             and outindex.nplike is self._backend.index_nplike
             and self._mask.nplike is self._backend.index_nplike
             and parents.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ByteMaskedArray_reduce_next_64",
                 nextcarry.dtype.type,
                 nextparents.dtype.type,
                 outindex.dtype.type,
                 self._mask.dtype.type,
                 parents.dtype.type,
@@ -883,15 +894,15 @@
                 next_length, nplike=self._backend.index_nplike
             )
             if shifts is None:
                 assert (
                     nextshifts.nplike is self._backend.index_nplike
                     and self._mask.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64",
                         nextshifts.dtype.type,
                         self._mask.dtype.type,
                     ](
                         nextshifts.data,
                         self._mask.data,
@@ -900,15 +911,15 @@
                     )
                 )
             else:
                 assert (
                     nextshifts.nplike is self._backend.index_nplike
                     and self._mask.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64",
                         nextshifts.dtype.type,
                         self._mask.dtype.type,
                         shifts.dtype.type,
                     ](
                         nextshifts.data,
@@ -934,30 +945,32 @@
             keepdims,
             behavior,
         )
 
         if not branch and negaxis == depth:
             return out
         else:
-            if out.is_list:
-                out_content = out.content[out.starts[0] :]
-            elif out.is_regular:
+            if isinstance(out, ak.contents.RegularArray):
                 out_content = out.content
+            elif isinstance(out, ak.contents.ListOffsetArray):
+                # The `outindex` that will index into `out_content` is 0-based, so we should ensure that we normalise
+                # the list content to start at the first offset.
+                out_content = out.content[out.offsets[0] :]
             else:
                 raise ValueError(
                     "reduce_next with unbranching depth > negaxis is only "
                     "expected to return RegularArray or ListOffsetArray64; "
                     "instead, it returned " + out
                 )
 
             outoffsets = ak.index.Index64.empty(
                 starts.length + 1, nplike=self._backend.index_nplike
             )
             assert outoffsets.nplike is self._backend.nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_reduce_next_fix_offsets_64",
                     outoffsets.dtype.type,
                     starts.dtype.type,
                 ](
                     outoffsets.data,
                     starts.data,
@@ -989,15 +1002,15 @@
             index = ak.index.Index64.empty(
                 mask.length, nplike=self._backend.index_nplike
             )
             assert (
                 index.nplike is self._backend.index_nplike
                 and self._mask.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedOptionArray_rpad_and_clip_mask_axis1",
                     index.dtype.type,
                     self._mask.dtype.type,
                 ](
                     index.data,
                     self._mask.data,
@@ -1033,15 +1046,15 @@
     def _remove_structure(self, backend, options):
         branch, depth = self.branch_depth
         if branch or options["drop_nones"] or depth > 1:
             return self.project()._remove_structure(backend, options)
         else:
             return [self]
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.project()
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if self._backend.nplike.known_data:
             content = self._content[0 : self._mask.length]
```

### Comparing `awkward-2.2.1/src/awkward/contents/content.py` & `awkward-2.2.2/src/awkward/contents/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import math
-from collections.abc import Callable, Iterable, Mapping, MutableMapping, Sized
+from collections.abc import Callable, Iterable, Mapping, MutableMapping, Sequence, Sized
 from numbers import Complex, Real
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import (
     backend_of,
     register_backend_lookup_factory,
     regularize_backend,
 )
 from awkward._behavior import get_array_class, get_record_class
+from awkward._kernels import KernelError
 from awkward._layout import wrap_layout
 from awkward._nplikes import to_nplike
 from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import TypeTracer
@@ -40,14 +41,17 @@
 from awkward._util import UNSET
 from awkward.forms.form import Form
 from awkward.index import Index, Index64
 
 if TYPE_CHECKING:
     from awkward._nplikes.numpy import NumpyLike
     from awkward._slicing import SliceItem
+    from awkward.contents.indexedoptionarray import IndexedOptionArray
+    from awkward.contents.numpyarray import NumpyArray
+    from awkward.contents.regulararray import RegularArray
 
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 ActionType: TypeAlias = """Callable[
     [
@@ -58,14 +62,17 @@
         Callable[[], None],
         dict | None,
         NumpyLike | None,
         dict[str, Any],
     ],
     Content | None,
 ]"""
+JSONValueType: TypeAlias = """
+float | int | str | list[JSONValueType] | dict[str, JSONValueType]
+"""
 
 
 class RecursivelyApplyOptionsType(TypedDict):
     allow_records: bool
     keep_parameters: bool
     numpy_to_regular: bool
     regular_to_jagged: bool
@@ -132,30 +139,30 @@
                 )
             )
 
         self._parameters = parameters
         self._backend = backend
 
     @property
-    def parameters(self) -> dict[str, Any]:
+    def parameters(self) -> dict[str, JSONValueType]:
         """
         Free-form parameters associated with every array node as a dict from parameter
         name to its JSON-like value. Some parameters are special and are used to assign
         behaviors to the data.
 
         Note that the dict returned by this property is a *view* of the array node's
         parameters. *Changing the dict will change the array!*
 
         See #ak.behavior.
         """
         if self._parameters is None:
             self._parameters = {}
         return self._parameters
 
-    def parameter(self, key: str):
+    def parameter(self, key: str) -> JSONValueType | None:
         """
         Returns a parameter's value or None.
 
         (No distinction is ever made between unset parameters and parameters set to None.)
         """
         if self._parameters is None:
             return None
@@ -166,15 +173,17 @@
     def backend(self) -> Backend:
         return self._backend
 
     @property
     def form(self) -> Form:
         return self.form_with_key(None)
 
-    def form_with_key(self, form_key="node{id}", id_start=0):
+    def form_with_key(
+        self, form_key: str | None | Callable = "node{id}", id_start: int = 0
+    ) -> Form:
         hold_id = [id_start]
 
         if form_key is None:
 
             def getkey(layout):
                 return None
 
@@ -199,32 +208,32 @@
                 )
             )
 
         return self._form_with_key(getkey)
 
     def _form_with_key(
         self,
-        getkey: Callable[[Content], Form],
+        getkey: Callable[[Content], str | None],
     ) -> Form:
         raise NotImplementedError
 
     @property
     def form_cls(self) -> type[Form]:
         raise NotImplementedError
 
     def to_typetracer(self, forget_length: bool = False) -> Self:
         return self._to_typetracer(forget_length)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         raise NotImplementedError
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         raise NotImplementedError
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         raise NotImplementedError
 
     @property
     def length(self) -> ShapeItem:
         raise NotImplementedError
 
     def _to_buffers(
@@ -250,61 +259,20 @@
                     )
                 )
         return out
 
     def maybe_to_NumpyArray(self):
         return None
 
-    def _handle_error(self, error, slicer=None):
-        if error is not None and error.str is not None:
-            if error.filename is None:
-                filename = ""
-            else:
-                filename = " (in compiled code: " + error.filename.decode(
-                    errors="surrogateescape"
-                ).lstrip("\n").lstrip("(")
-
-            message = error.str.decode(errors="surrogateescape")
-
-            if error.pass_through:
-                raise ValueError(message + filename)
-
-            else:
-                if error.attempt != ak._util.kSliceNone:
-                    message += f" while attempting to get index {error.attempt}"
-
-                message += filename
-
-                if slicer is None:
-                    raise ValueError(message)
-                else:
-                    raise ak._errors.index_error(self, slicer, message)
-
-    @staticmethod
-    def _selfless_handle_error(error):
-        if error.str is not None:
-            if error.filename is None:
-                filename = ""
-            else:
-                filename = " (in compiled code: " + error.filename.decode(
-                    errors="surrogateescape"
-                ).lstrip("\n").lstrip("(")
-
-            message = error.str.decode(errors="surrogateescape")
-
-            if error.pass_through:
-                raise ValueError(message + filename)
-
-            else:
-                if error.attempt != ak._util.kSliceNone:
-                    message += f" while attempting to get index {error.attempt}"
-
-                message += filename
-
-                raise ValueError(message)
+    def _maybe_index_error(self, error: KernelError | None, slicer):
+        if error is None or error.str is None:
+            return
+        else:
+            message = self._backend.format_kernel_error(error)
+            raise ak._errors.index_error(self, slicer, message)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         raise TypeError(
             "do not apply NumPy functions to low-level layouts (Content subclasses); put them in ak.highlevel.Array"
         )
 
     def __array_function__(self, func, types, args, kwargs):
@@ -329,33 +297,39 @@
         head: SliceItem | tuple,
         tail: tuple[SliceItem, ...],
         advanced: Index | None,
     ):
         nexthead, nexttail = ak._slicing.head_tail(tail)
         return self._getitem_field(head)._getitem_next(nexthead, nexttail, advanced)
 
-    def _getitem_next_fields(self, head, tail, advanced: Index | None) -> Content:
+    def _getitem_next_fields(
+        self, head: SliceItem, tail: tuple[SliceItem, ...], advanced: Index | None
+    ) -> Content:
         only_fields, not_fields = [], []
         for x in tail:
             if isinstance(x, (str, list)):
                 only_fields.append(x)
             else:
                 not_fields.append(x)
         nexthead, nexttail = ak._slicing.head_tail(tuple(not_fields))
         return self._getitem_fields(head, tuple(only_fields))._getitem_next(
             nexthead, nexttail, advanced
         )
 
-    def _getitem_next_newaxis(self, tail, advanced: Index | None):
+    def _getitem_next_newaxis(
+        self, tail: tuple[SliceItem, ...], advanced: Index | None
+    ) -> RegularArray:
         nexthead, nexttail = ak._slicing.head_tail(tail)
         return ak.contents.RegularArray(
             self._getitem_next(nexthead, nexttail, advanced), 1, 0, parameters=None
         )
 
-    def _getitem_next_ellipsis(self, tail, advanced: Index | None):
+    def _getitem_next_ellipsis(
+        self, tail: tuple[SliceItem, ...], advanced: Index | None
+    ) -> Content:
         mindepth, maxdepth = self.minmax_depth
 
         dimlength = sum(
             1 if is_integer_like(x) or isinstance(x, (slice, Index64)) else 0
             for x in tail
         )
 
@@ -371,35 +345,35 @@
             )
 
         else:
             return self._getitem_next(slice(None), (Ellipsis, *tail), advanced)
 
     def _getitem_next_regular_missing(
         self,
-        head: ak.contents.IndexedOptionArray,
-        tail,
+        head: IndexedOptionArray,
+        tail: tuple[SliceItem, ...],
         advanced: Index | None,
         raw: Content,
         length: int,
-    ):
+    ) -> RegularArray:
         # if this is in a tuple-slice and really should be 0, it will be trimmed later
         length = 1 if length is not unknown_length and length == 0 else length
         index = head.index
         indexlength = index.length
         index = index.to_nplike(self._backend.index_nplike)
         outindex = Index64.empty(
             index.length * length,
             self._backend.index_nplike,
         )
 
         assert (
             outindex.nplike is self._backend.index_nplike
             and index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_missing_repeat", outindex.dtype.type, index.dtype.type
             ](
                 outindex.data,
                 index.data,
                 index.length,
                 length,
@@ -413,15 +387,15 @@
         )
         return ak.contents.RegularArray(
             out, indexlength, 1, parameters=self._parameters
         )
 
     def _getitem_next_missing_jagged(
         self, head: Content, tail, advanced: Index | None, that: Content
-    ):
+    ) -> RegularArray:
         head = head.to_backend(self._backend)
         jagged = head.content.to_ListOffsetArray64()
         index = head._index
         content = that._getitem_at(0)
         if self._backend.nplike.known_data and content.length < index.length:
             raise ak._errors.index_error(
                 self,
@@ -438,15 +412,15 @@
         assert (
             index.nplike is self._backend.index_nplike
             and jagged._offsets.nplike is self._backend.index_nplike
             and outputmask.nplike is self._backend.index_nplike
             and starts.nplike is self._backend.index_nplike
             and stops.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_Content_getitem_next_missing_jagged_getmaskstartstop",
                 index.dtype.type,
                 jagged._offsets.dtype.type,
                 outputmask.dtype.type,
                 starts.dtype.type,
                 stops.dtype.type,
@@ -467,18 +441,18 @@
         )
         return ak.contents.RegularArray(
             out, index.length, 1, parameters=self._parameters
         )
 
     def _getitem_next_missing(
         self,
-        head: ak.contents.IndexedOptionArray,
-        tail,
+        head: IndexedOptionArray,
+        tail: tuple[SliceItem, ...],
         advanced: Index | None,
-    ):
+    ) -> Content:
         assert isinstance(head, ak.contents.IndexedOptionArray)
 
         if advanced is not None:
             raise ak._errors.index_error(
                 self,
                 head,
                 "cannot mix missing values in slice with NumPy-style advanced indexing",
@@ -726,36 +700,42 @@
         self,
         head: SliceItem | tuple,
         tail: tuple[SliceItem, ...],
         advanced: Index | None,
     ) -> Content:
         raise NotImplementedError
 
+    def _getitem_next_jagged(
+        self,
+        slicestarts: Index,
+        slicestops: Index,
+        slicecontent: Content,
+        tail: tuple[SliceItem, ...],
+    ) -> Content:
+        raise NotImplementedError
+
     def _carry(self, carry: Index, allow_lazy: bool) -> Content:
         raise NotImplementedError
 
-    def _local_index_axis0(self) -> ak.contents.NumpyArray:
+    def _local_index_axis0(self) -> NumpyArray:
         localindex = Index64.empty(self.length, self._backend.index_nplike)
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend["awkward_localindex", np.int64](
                 localindex.data,
                 localindex.length,
             )
         )
         return ak.contents.NumpyArray(
             localindex.data, parameters=None, backend=self._backend
         )
 
     def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         raise NotImplementedError
 
-    def _mergemany(
-        self,
-        others: list[Content],
-    ) -> Content:
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         raise NotImplementedError
 
     def _merging_strategy(
         self, others: list[Content]
     ) -> tuple[list[Content], list[Content]]:
         if len(others) == 0:
             raise ValueError(
@@ -881,15 +861,15 @@
         toindex = Index64.empty(n, self._backend.index_nplike, dtype=np.int64)
         fromindex = Index64.empty(n, self._backend.index_nplike, dtype=np.int64)
 
         assert (
             toindex.nplike is self._backend.index_nplike
             and fromindex.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_RegularArray_combinations_64",
                 np.int64,
                 toindex.data.dtype.type,
                 fromindex.data.dtype.type,
             ](
                 tocarryraw,
@@ -1019,15 +999,15 @@
                 nplike=self._backend.index_nplike,
             )
 
         else:
             index = Index64.empty(target, self._backend.index_nplike)
 
             assert index.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_index_rpad_and_clip_axis0",
                     index.dtype.type,
                 ](index.data, target, self.length)
             )
 
         return ak.contents.IndexedOptionArray.simplified(
```

### Comparing `awkward-2.2.1/src/awkward/contents/emptyarray.py` & `awkward-2.2.2/src/awkward/contents/emptyarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._errors import AxisError, deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.forms.emptyform import EmptyForm
+from awkward.forms.form import Form
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
@@ -99,34 +102,41 @@
 
     @classmethod
     def simplified(cls, *, parameters=None, backend=None):
         if not (parameters is None or len(parameters) == 0):
             deprecate(f"{cls.__name__} cannot contain parameters", version="2.2.0")
         return cls(parameters=parameters, backend=backend)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> EmptyForm:
         return self.form_cls(parameters=self._parameters, form_key=getkey(self))
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         return EmptyArray(
             parameters=self._parameters,
             backend=TypeTracerBackend.instance(),
         )
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         pass
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         pass
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return 0
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         extra = self._repr_extra(indent + "    ")
@@ -178,15 +188,17 @@
         assert isinstance(carry, ak.index.Index)
 
         if not carry.nplike.known_data or carry.length == 0:
             return self
         else:
             raise ak._errors.index_error(self, carry.data, "array is empty")
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         raise ak._errors.index_error(
             self,
             ak.contents.ListArray(
                 slicestarts, slicestops, slicecontent, parameters=None
             ),
             "too many jagged slice dimensions for array",
         )
@@ -229,29 +241,29 @@
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             raise ak._errors.index_error(self, head, "array is empty")
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError(self, "axis=0 not allowed for flatten")
         else:
             offsets = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
             return (
                 offsets,
                 EmptyArray(parameters=self._parameters, backend=self._backend),
             )
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         return True
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
         elif len(others) == 1:
             return others[0]
         else:
             return others[0]._mergemany(others[1:])
```

### Comparing `awkward-2.2.1/src/awkward/contents/indexedarray.py` & `awkward-2.2.2/src/awkward/contents/indexedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.indexedform import IndexedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
+    from awkward.contents.indexedoptionarray import IndexedOptionArray
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 @final
 class IndexedArray(Content):
@@ -119,15 +123,15 @@
         self._init(parameters, content.backend)
 
     @property
     def index(self):
         return self._index
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     form_cls: Final = IndexedForm
 
     def copy(self, index=UNSET, content=UNSET, *, parameters=UNSET):
         return IndexedArray(
             self._index if index is UNSET else index,
@@ -158,15 +162,15 @@
             backend = content.backend
             if content.is_indexed:
                 inner = content.index
             else:
                 inner = content.to_IndexedOptionArray64().index
             result = ak.index.Index64.empty(index.length, nplike=backend.index_nplike)
 
-            Content._selfless_handle_error(
+            backend.maybe_kernel_error(
                 backend[
                     "awkward_IndexedArray_simplify",
                     result.dtype.type,
                     index.dtype.type,
                     inner.dtype.type,
                 ](
                     result.data,
@@ -188,24 +192,31 @@
                     content.content,
                     parameters=parameters_union(content._parameters, parameters),
                 )
 
         else:
             return cls(index, content, parameters=parameters)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> IndexedForm:
         form_key = getkey(self)
         return self.form_cls(
             self._index.form,
             self._content._form_with_key(getkey),
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "index")
         container[key] = ak._util.native_to_byteorder(
             self._index.raw(backend.index_nplike), byteorder
         )
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
@@ -213,28 +224,26 @@
         index = self._index.to_nplike(TypeTracer.instance())
         return IndexedArray(
             index.forget_length() if forget_length else index,
             self._content._to_typetracer(False),
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._index.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._index._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._index.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._index._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._index.length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<IndexedArray len="]
@@ -244,15 +253,15 @@
         out.append("\n")
         out.append(self._index._repr(indent + "    ", "<index>", "</index>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</IndexedArray>")
         out.append(post)
         return "".join(out)
 
-    def to_IndexedOptionArray64(self):
+    def to_IndexedOptionArray64(self) -> IndexedOptionArray:
         return ak.contents.IndexedOptionArray(
             self._index, self._content, parameters=self._parameters
         )
 
     def mask_as_bool(self, valid_when=True):
         if valid_when:
             return self._index.data >= 0
@@ -323,15 +332,15 @@
             )
 
         nextcarry = ak.index.Index64.empty(self.length, self._backend.index_nplike)
         assert (
             nextcarry.nplike is self._backend.index_nplike
             and self._index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_IndexedArray_getitem_nextcarry",
                 nextcarry.dtype.type,
                 self._index.dtype.type,
             ](
                 nextcarry.data,
                 self._index.data,
@@ -340,15 +349,17 @@
             ),
             slicer=ak.contents.ListArray(slicestarts, slicestops, slicecontent),
         )
         # an eager carry (allow_lazy = false) to avoid infinite loop (unproven)
         next = self._content._carry(nextcarry, False)
         return next._getitem_next_jagged(slicestarts, slicestops, slicecontent, tail)
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return self._getitem_next_jagged_generic(
             slicestarts, slicestops, slicecontent, tail
         )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
@@ -366,15 +377,15 @@
             nextcarry = ak.index.Index64.empty(
                 self._index.length, self._backend.index_nplike
             )
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_IndexedArray_getitem_nextcarry",
                     nextcarry.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextcarry.data,
                     self._index.data,
@@ -417,15 +428,15 @@
                 self._index.length, self._backend.index_nplike
             )
             assert (
                 nextindex.nplike is self._backend.index_nplike
                 and mask.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_overlay_mask",
                     nextindex.dtype.type,
                     mask.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextindex.data,
@@ -441,15 +452,15 @@
 
         else:
             nextcarry = ak.index.Index64.empty(self.length, self._backend.index_nplike)
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_getitem_nextcarry",
                     nextcarry.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextcarry.data,
                     self._index.data,
@@ -462,23 +473,23 @@
                 parameters=parameters_union(
                     next._parameters,
                     self._parameters,
                     exclude=(("__array__", "categorical"),),
                 )
             )
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
 
         else:
             return self.project()._offsets_and_flattened(axis, depth)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option/indexed types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
@@ -527,26 +538,26 @@
             (theirlength + mylength), self._backend.index_nplike
         )
 
         content = other._mergemany([self._content])
 
         # Fill `index` with a range starting at zero, up to `theirlength`
         assert index.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend["awkward_IndexedArray_fill_count", index.dtype.type](
                 index.data,
                 0,
                 theirlength,
                 0,
             )
         )
 
         # Fill remaining indices
         assert index.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_fill",
                 index.dtype.type,
                 self.index.dtype.type,
             ](
                 index.data,
                 theirlength,
@@ -562,15 +573,15 @@
         else:
             parameters = self._parameters
 
         return ak.contents.IndexedArray.simplified(
             index, content, parameters=parameters
         )
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         head, tail = self._merging_strategy(others)
 
         total_length = 0
         for array in head:
@@ -605,15 +616,15 @@
 
                 contents.append(array.content)
                 array_index = array.index
                 assert (
                     nextindex.nplike is self._backend.index_nplike
                     and array_index.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_fill",
                         nextindex.dtype.type,
                         array_index.dtype.type,
                     ](
                         nextindex.data,
                         length_so_far,
@@ -623,15 +634,15 @@
                     )
                 )
                 contentlength_so_far += array.content.length
                 length_so_far += array.length
             else:
                 contents.append(array)
                 assert nextindex.nplike is self._backend.index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_fill_count",
                         nextindex.dtype.type,
                     ](
                         nextindex.data,
                         length_so_far,
                         array.length,
@@ -688,15 +699,15 @@
             offsets = ak.index.Index64.empty(2, self._backend.index_nplike)
             offsets[0] = 0
             offsets[1] = next.length
             assert (
                 next.nplike is self._backend.index_nplike
                 and offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sort",
                     next.dtype.type,
                     next.dtype.type,
                     offsets.dtype.type,
                 ](
                     next.data,
@@ -710,29 +721,29 @@
                 )
             )
 
             assert (
                 next.nplike is self._backend.index_nplike
                 and length.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend["awkward_unique", next.dtype.type, length.dtype.type](
                     next.data,
                     self._index.length,
                     length.data,
                 )
             )
 
         else:
             assert (
                 self._index.nplike is self._backend.index_nplike
                 and next.nplike is self._backend.index_nplike
                 and length.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_unique_copy",
                     self._index.dtype.type,
                     next.dtype.type,
                     length.dtype.type,
                 ](
                     self._index.data,
@@ -779,15 +790,15 @@
         assert (
             nextcarry.nplike is self._backend.index_nplike
             and nextparents.nplike is self._backend.index_nplike
             and outindex.nplike is self._backend.index_nplike
             and self._index.nplike is self._backend.index_nplike
             and parents.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_reduce_next_64",
                 nextcarry.dtype.type,
                 nextparents.dtype.type,
                 outindex.dtype.type,
                 self._index.dtype.type,
                 parents.dtype.type,
@@ -814,15 +825,15 @@
             )
             assert (
                 nextoutindex.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
                 and nextparents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_local_preparenext",
                     nextoutindex.dtype.type,
                     starts.dtype.type,
                     parents.dtype.type,
                     nextparents.dtype.type,
                 ](
@@ -857,15 +868,15 @@
                 outoffsets = ak.index.Index64.empty(
                     starts.length + 1, self._backend.index_nplike
                 )
                 assert (
                     outoffsets.nplike is self._backend.index_nplike
                     and starts.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_reduce_next_fix_offsets_64",
                         outoffsets.dtype.type,
                         starts.dtype.type,
                     ](
                         outoffsets.data,
                         starts.data,
```

### Comparing `awkward-2.2.1/src/awkward/contents/indexedoptionarray.py` & `awkward-2.2.2/src/awkward/contents/indexedoptionarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.indexedoptionform import IndexedOptionForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
@@ -117,15 +119,15 @@
         self._init(parameters, content.backend)
 
     @property
     def index(self):
         return self._index
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     form_cls: Final = IndexedOptionForm
 
     def copy(self, index=UNSET, content=UNSET, *, parameters=UNSET):
         return IndexedOptionArray(
             self._index if index is UNSET else index,
@@ -154,15 +156,15 @@
             backend = content.backend
             if content.is_indexed:
                 inner = content.index
             else:
                 inner = content.to_IndexedOptionArray64().index
             result = ak.index.Index64.empty(index.length, nplike=backend.index_nplike)
 
-            Content._selfless_handle_error(
+            backend.maybe_kernel_error(
                 backend[
                     "awkward_IndexedArray_simplify",
                     result.dtype.type,
                     index.dtype.type,
                     inner.dtype.type,
                 ](
                     result.data,
@@ -177,24 +179,33 @@
                 content.content,
                 parameters=parameters_union(content._parameters, parameters),
             )
 
         else:
             return cls(index, content, parameters=parameters)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(
+        self, getkey: Callable[[Content], str | None]
+    ) -> IndexedOptionForm:
         form_key = getkey(self)
         return self.form_cls(
             self._index.form,
             self._content._form_with_key(getkey),
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "index")
         container[key] = ak._util.native_to_byteorder(
             self._index.raw(backend.index_nplike), byteorder
         )
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
@@ -202,28 +213,26 @@
         index = self._index.to_nplike(TypeTracer.instance())
         return IndexedOptionArray(
             index.forget_length() if forget_length else index,
             self._content._to_typetracer(False),
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._index.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._index._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._index.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._index._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._index.length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<IndexedOptionArray len="]
@@ -233,15 +242,15 @@
         out.append("\n")
         out.append(self._index._repr(indent + "    ", "<index>", "</index>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</IndexedOptionArray>")
         out.append(post)
         return "".join(out)
 
-    def to_IndexedOptionArray64(self):
+    def to_IndexedOptionArray64(self) -> IndexedOptionArray:
         if self._index.dtype == np.dtype(np.int64):
             return self
         else:
             return IndexedOptionArray(
                 self._backend.index_nplike.astype(self._index, dtype=np.int64),
                 self._content,
                 parameters=self._parameters,
@@ -337,15 +346,15 @@
 
     def _nextcarry_outindex(self):
         backend = self._backend
         index_nplike = backend.index_nplike
 
         _numnull = ak.index.Index64.empty(1, nplike=backend.index_nplike)
         assert _numnull.nplike is index_nplike and self._index.nplike is index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             backend[
                 "awkward_IndexedArray_numnull",
                 _numnull.dtype.type,
                 self._index.dtype.type,
             ](
                 _numnull.data,
                 self._index.data,
@@ -364,15 +373,15 @@
         )
 
         assert (
             nextcarry.nplike is index_nplike
             and outindex.nplike is index_nplike
             and self._index.nplike is index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             backend[
                 "awkward_IndexedArray_getitem_nextcarry_outindex",
                 nextcarry.dtype.type,
                 outindex.dtype.type,
                 self._index.dtype.type,
             ](
                 nextcarry.data,
@@ -413,15 +422,15 @@
         assert (
             outindex.nplike is self._backend.index_nplike
             and slicestarts.nplike is self._backend.index_nplike
             and slicestops.nplike is self._backend.index_nplike
             and reducedstarts.nplike is self._backend.index_nplike
             and reducedstops.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_MaskedArray_getitem_next_jagged_project",
                 outindex.dtype.type,
                 slicestarts.dtype.type,
                 slicestops.dtype.type,
                 reducedstarts.dtype.type,
                 reducedstops.dtype.type,
@@ -438,15 +447,17 @@
         next = self._content._carry(nextcarry, True)
         out = next._getitem_next_jagged(reducedstarts, reducedstops, slicecontent, tail)
 
         return ak.contents.IndexedOptionArray.simplified(
             outindex, out, parameters=self._parameters
         )
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return self._getitem_next_jagged_generic(
             slicestarts, slicestops, slicecontent, tail
         )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
@@ -499,15 +510,15 @@
                 self._index.length, self._backend.index_nplike
             )
             assert (
                 nextindex.nplike is self._backend.index_nplike
                 and mask.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_overlay_mask",
                     nextindex.dtype.type,
                     mask.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextindex.data,
@@ -522,15 +533,15 @@
             return next.project()
         else:
             _numnull = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _numnull.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_numnull",
                     _numnull.dtype.type,
                     self._index.dtype.type,
                 ](
                     _numnull.data,
                     self._index.data,
@@ -543,30 +554,30 @@
                 self._backend.index_nplike,
             )
 
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_flatten_nextcarry",
                     nextcarry.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextcarry.data,
                     self._index.data,
                     self._index.length,
                     self._content.length,
                 )
             )
 
             return self._content._carry(nextcarry, False)
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
             next = self._content._carry(nextcarry, False)
 
@@ -588,15 +599,15 @@
                 )
 
                 assert (
                     outoffsets.nplike is self._backend.index_nplike
                     and outindex.nplike is self._backend.index_nplike
                     and offsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_flatten_none2empty",
                         outoffsets.dtype.type,
                         outindex.dtype.type,
                         offsets.dtype.type,
                     ](
                         outoffsets.data,
@@ -604,15 +615,15 @@
                         outindex.length,
                         offsets.data,
                         offsets.length,
                     )
                 )
                 return (outoffsets, flattened)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option/indexed types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
@@ -664,15 +675,15 @@
             theirlength + mylength,
             self._backend.index_nplike,
         )
 
         content = other._mergemany([self._content])
 
         assert index.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend["awkward_IndexedArray_fill_count", index.dtype.type](
                 index.data,
                 0,
                 theirlength,
                 0,
             )
         )
@@ -681,15 +692,15 @@
             nplike=self._backend.index_nplike,
         )
 
         assert (
             index.nplike is self._backend.index_nplike
             and reinterpreted_index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_fill",
                 index.dtype.type,
                 reinterpreted_index.dtype.type,
             ](
                 index.data,
                 theirlength,
@@ -705,15 +716,15 @@
         else:
             parameters = self._parameters
 
         return ak.contents.IndexedOptionArray.simplified(
             index, content, parameters=parameters
         )
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         head, tail = self._merging_strategy(others)
 
         total_length = 0
         for array in head:
@@ -746,15 +757,15 @@
                 parameters = parameters_intersect(parameters, array._parameters)
                 contents.append(array.content)
                 array_index = array.index
                 assert (
                     nextindex.nplike is self._backend.index_nplike
                     and array_index.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_fill",
                         nextindex.dtype.type,
                         array_index.dtype.type,
                     ](
                         nextindex.data,
                         length_so_far,
@@ -766,15 +777,15 @@
                 contentlength_so_far += array.content.length
 
                 length_so_far += array.length
 
             else:
                 contents.append(array)
                 assert nextindex.nplike is self._backend.index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_IndexedArray_fill_count",
                         nextindex.dtype.type,
                     ](
                         nextindex.data,
                         length_so_far,
                         array.length,
@@ -810,15 +821,15 @@
         tags = ak.index.Index8(self.mask_as_bool(valid_when=False))
         index = ak.index.Index64.empty(tags.length, self._backend.index_nplike)
 
         assert (
             index.nplike is self._backend.index_nplike
             and self._index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_UnionArray_fillna", index.dtype.type, self._index.dtype.type
             ](index.data, self._index.data, tags.length)
         )
         return ak.contents.UnionArray.simplified(
             tags,
             index,
@@ -851,15 +862,15 @@
             self._index.nplike is self._backend.index_nplike
             and starts.nplike is self._backend.index_nplike
             and stops.nplike is self._backend.index_nplike
             and nextstarts.nplike is self._backend.index_nplike
             and nextstops.nplike is self._backend.index_nplike
             and subranges_length.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_ranges_next_64",
                 self._index.dtype.type,
                 starts.dtype.type,
                 stops.dtype.type,
                 nextstarts.dtype.type,
                 nextstops.dtype.type,
@@ -880,15 +891,15 @@
         )
         assert (
             self._index.nplike is self._backend.index_nplike
             and starts.nplike is self._backend.index_nplike
             and stops.nplike is self._backend.index_nplike
             and nextcarry.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_ranges_carry_next_64",
                 self._index.dtype.type,
                 starts.dtype.type,
                 stops.dtype.type,
                 nextcarry.dtype.type,
             ](
@@ -946,15 +957,15 @@
             )
             assert (
                 nextoutindex.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
                 and nextparents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_local_preparenext",
                     nextoutindex.dtype.type,
                     starts.dtype.type,
                     parents.dtype.type,
                     nextparents.dtype.type,
                 ](
@@ -977,15 +988,15 @@
             )
             _len_newnulls = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 newnulls.nplike is self._backend.index_nplike
                 and _len_newnulls.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_numnull_parents",
                     newnulls.dtype.type,
                     _len_newnulls.dtype.type,
                     self._index.dtype.type,
                 ](
                     newnulls.data,
@@ -1008,15 +1019,15 @@
             )
             assert (
                 newindex.nplike is self._backend.index_nplike
                 and newoffsets.nplike is self._backend.index_nplike
                 and out._offsets.nplike is self._backend.index_nplike
                 and newnulls.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_unique_next_index_and_offsets_64",
                     newindex.dtype.type,
                     newoffsets.dtype.type,
                     out._offsets.dtype.type,
                     newnulls.dtype.type,
                 ](
@@ -1041,15 +1052,15 @@
             # values in the result. We do this by creating an IndexedOptionArray
             # and tacking the index -1 onto the end
             nextoutindex = ak.index.Index64.empty(
                 out.length + 1,
                 self._backend.index_nplike,
             )
             assert nextoutindex.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_numnull_unique_64",
                     nextoutindex.dtype.type,
                 ](
                     nextoutindex.data,
                     out.length,
                 )
@@ -1073,15 +1084,15 @@
         assert nextshifts.nplike is self._backend.index_nplike
 
         if shifts is None:
             assert (
                 nextshifts.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64",
                     nextshifts.dtype.type,
                     self._index.dtype.type,
                 ](
                     nextshifts.data,
                     self._index.data,
@@ -1090,15 +1101,15 @@
             )
         else:
             assert (
                 nextshifts.nplike is self._backend.index_nplike
                 and self._index.nplike is self._backend.index_nplike
                 and shifts.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64",
                     nextshifts.dtype.type,
                     self._index.dtype.type,
                     shifts.dtype.type,
                 ](
                     nextshifts.data,
@@ -1114,15 +1125,15 @@
             self._index.nplike is self._backend.index_nplike
             and parents.nplike is self._backend.index_nplike
         )
         index_length = self._index.length
         _numnull = ak.index.Index64.empty(1, self._backend.index_nplike)
         assert _numnull.nplike is self._backend.index_nplike
 
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_numnull",
                 _numnull.dtype.type,
                 self._index.dtype.type,
             ](
                 _numnull.data,
                 self._index.data,
@@ -1136,15 +1147,15 @@
         nextcarry = ak.index.Index64.empty(next_length, self._backend.index_nplike)
         outindex = ak.index.Index64.empty(index_length, self._backend.index_nplike)
         assert (
             nextcarry.nplike is self._backend.index_nplike
             and nextparents.nplike is self._backend.index_nplike
             and outindex.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_reduce_next_64",
                 nextcarry.dtype.type,
                 nextparents.dtype.type,
                 outindex.dtype.type,
                 self._index.dtype.type,
                 parents.dtype.type,
@@ -1185,15 +1196,15 @@
         # `next._argsort_next` is given the non-None values. We choose to
         # sort None values to the end of the list, meaning we need to grow `out`
         # to account for these None values. First, we locate these nones within
         # their sublists
         nulls_merged = False
         nulls_index = ak.index.Index64.empty(numnull, self._backend.index_nplike)
         assert nulls_index.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_index_of_nulls",
                 nulls_index.dtype.type,
                 self._index.dtype.type,
                 parents.dtype.type,
                 starts.dtype.type,
             ](
@@ -1221,15 +1232,15 @@
         )
         assert (
             nextoutindex.nplike is self._backend.index_nplike
             and starts.nplike is self._backend.index_nplike
             and parents.nplike is self._backend.index_nplike
             and nextparents.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_local_preparenext",
                 nextoutindex.dtype.type,
                 starts.dtype.type,
                 parents.dtype.type,
                 nextparents.dtype.type,
             ](
@@ -1245,15 +1256,15 @@
         if nulls_merged:
             # awkward_IndexedArray_local_preparenext uses -1 to
             # indicate `None` values. Given that this code-path runs
             # only when the `None` value indices are explicitly stored in out,
             # we need to mapping the -1 values to their corresponding indices
             # in `out`
             assert nextoutindex.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend["awkward_Index_nones_as_index", nextoutindex.dtype.type](
                     nextoutindex.data,
                     nextoutindex.length,
                 )
             )
 
         out = ak.contents.IndexedOptionArray.simplified(
@@ -1298,15 +1309,15 @@
         )
 
         nextoutindex = ak.index.Index64.empty(
             parents.length, self._backend.index_nplike
         )
         assert nextoutindex.nplike is self._backend.index_nplike
 
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_IndexedArray_local_preparenext",
                 nextoutindex.dtype.type,
                 starts.dtype.type,
                 parents.dtype.type,
                 nextparents.dtype.type,
             ](
@@ -1372,18 +1383,20 @@
         )
 
         # If we are reducing the contents of this layout,
         # then we do NOT want to return an optional layout
         if not branch and negaxis == depth:
             return out
         else:
-            if out.is_list:
-                out_content = out.content[out.starts[0] :]
-            elif out.is_regular:
+            if isinstance(out, ak.contents.RegularArray):
                 out_content = out.content
+            elif isinstance(out, ak.contents.ListOffsetArray):
+                # The `outindex` that will index into `out_content` is 0-based, so we should ensure that we normalise
+                # the list content to start at the first offset.
+                out_content = out.content[out.offsets[0] :]
             else:
                 raise AssertionError(
                     "reduce_next with unbranching depth > negaxis is only "
                     "expected to return RegularArray or ListOffsetArray or "
                     "IndexedOptionArray; "
                     "instead, it returned {}".format(type(out).__name__)
                 )
@@ -1410,15 +1423,15 @@
                     starts.length + 1,
                     self._backend.index_nplike,
                 )
             assert (
                 outoffsets.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedArray_reduce_next_fix_offsets_64",
                     outoffsets.dtype.type,
                     starts.dtype.type,
                 ](
                     outoffsets.data,
                     starts.data,
@@ -1479,15 +1492,15 @@
         elif posaxis is not None and posaxis + 1 == depth + 1:
             mask = ak.index.Index8(self.mask_as_bool(valid_when=False))
             index = ak.index.Index64.empty(mask.length, self._backend.index_nplike)
             assert (
                 index.nplike is self._backend.index_nplike
                 and mask.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_IndexedOptionArray_rpad_and_clip_mask_axis1",
                     index.dtype.type,
                     mask.dtype.type,
                 ](index.data, mask.data, mask.length)
             )
             next = self.project()._pad_none(target, axis, depth, clip)
@@ -1582,15 +1595,15 @@
     def _remove_structure(self, backend, options):
         branch, depth = self.branch_depth
         if branch or options["drop_nones"] or depth > 1:
             return self.project()._remove_structure(backend, options)
         else:
             return [self]
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.project()
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if (
             self._backend.nplike.known_data
```

### Comparing `awkward-2.2.1/src/awkward/contents/listarray.py` & `awkward-2.2.2/src/awkward/contents/listarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
 from awkward.contents.listoffsetarray import ListOffsetArray
+from awkward.forms.form import Form
 from awkward.forms.listform import ListForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
@@ -155,23 +157,23 @@
 
         self._starts = starts
         self._stops = stops
         self._content = content
         self._init(parameters, content.backend)
 
     @property
-    def starts(self):
+    def starts(self) -> Index:
         return self._starts
 
     @property
-    def stops(self):
+    def stops(self) -> Index:
         return self._stops
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     form_cls: Final = ListForm
 
     def copy(self, starts=UNSET, stops=UNSET, content=UNSET, *, parameters=UNSET):
         return ListArray(
             self._starts if starts is UNSET else starts,
@@ -191,25 +193,32 @@
             parameters=copy.deepcopy(self._parameters, memo),
         )
 
     @classmethod
     def simplified(cls, starts, stops, content, *, parameters=None):
         return cls(starts, stops, content, parameters=parameters)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> ListForm:
         form_key = getkey(self)
         return self.form_cls(
             self._starts.form,
             self._stops.form,
             self._content._form_with_key(getkey),
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key1 = getkey(self, form, "starts")
         key2 = getkey(self, form, "stops")
         container[key1] = ak._util.native_to_byteorder(
             self._starts.raw(backend.index_nplike), byteorder
         )
         container[key2] = ak._util.native_to_byteorder(
@@ -223,30 +232,28 @@
         return ListArray(
             starts.forget_length() if forget_length else starts,
             self._stops.to_nplike(tt),
             self._content._to_typetracer(False),
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._starts.data.touch_data()
-            self._stops.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._starts._touch_data()
+        self._stops._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._starts.data.touch_shape()
-            self._stops.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._starts._touch_shape()
+        self._stops._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._starts.length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<ListArray len="]
@@ -257,32 +264,26 @@
         out.append(self._starts._repr(indent + "    ", "<starts>", "</starts>\n"))
         out.append(self._stops._repr(indent + "    ", "<stops>", "</stops>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</ListArray>")
         out.append(post)
         return "".join(out)
 
-    def to_ListOffsetArray64(self, start_at_zero=False):
+    def to_ListOffsetArray64(self, start_at_zero: bool = False) -> ListOffsetArray:
+        index_nplike = self._backend.index_nplike
+
         starts = self._starts.data
         stops = self._stops.data
 
-        lenoffsets = None if (starts.shape[0] is None) else (starts.shape[0] + 1)
-        if not self._backend.nplike.known_data:
-            self._touch_data(recursive=False)
-            self._content._touch_data(recursive=False)
-            offsets = self._backend.index_nplike.empty(lenoffsets, dtype=starts.dtype)
-            return ListOffsetArray(
-                ak.index.Index(offsets, nplike=self._backend.index_nplike),
-                self._content,
-                parameters=self._parameters,
-            )
-
-        elif self._backend.index_nplike.array_equal(starts[1:], stops[:-1]):
-            offsets = self._backend.index_nplike.empty(lenoffsets, dtype=starts.dtype)
-            if offsets.shape[0] == 1:
+        lenoffsets = self._starts.length + 1
+        if (not index_nplike.known_data) or index_nplike.array_equal(
+            starts[1:], stops[:-1]
+        ):
+            offsets = index_nplike.empty(lenoffsets, dtype=starts.dtype)
+            if lenoffsets is not unknown_length and lenoffsets == 1:
                 offsets[0] = 0
             else:
                 offsets[:-1] = starts
                 offsets[-1] = stops[-1]
             return ListOffsetArray(
                 ak.index.Index(offsets, nplike=self._backend.index_nplike),
                 self._content,
@@ -364,33 +365,88 @@
             self._backend.index_nplike,
         )
         assert (
             out.nplike is self._backend.index_nplike
             and self._starts.nplike is self._backend.index_nplike
             and self._stops.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListArray_compact_offsets",
                 out.dtype.type,
                 self._starts.dtype.type,
                 self._stops.dtype.type,
             ](
                 out.data,
                 self._starts.data,
                 self._stops.data,
                 starts_len,
             )
         )
         return out
 
-    def _broadcast_tooffsets64(self, offsets):
-        return ListOffsetArray._broadcast_tooffsets64(self, offsets)
+    def _broadcast_tooffsets64(self, offsets: Index) -> ListOffsetArray:
+        self._touch_data(recursive=False)
+        offsets._touch_data()
+
+        index_nplike = self._backend.index_nplike
+        assert offsets.nplike is index_nplike
+        if offsets.length is not unknown_length and offsets.length == 0:
+            raise AssertionError(
+                "broadcast_tooffsets64 can only be used with non-empty offsets"
+            )
+        elif index_nplike.known_data and offsets[0] != 0:
+            raise AssertionError(
+                f"broadcast_tooffsets64 can only be used with offsets that start at 0, not {offsets[0]}"
+            )
+        elif (
+            offsets.length is not unknown_length
+            and self._starts.length is not unknown_length
+            and offsets.length - 1 != self._starts.length
+        ):
+            raise AssertionError(
+                "cannot broadcast RegularArray of length {} to length {}".format(
+                    self._starts.length, offsets.length - 1
+                )
+            )
+
+        nextcarry = ak.index.Index64.empty(
+            self._backend.index_nplike.index_as_shape_item(offsets[-1]),
+            self._backend.index_nplike,
+        )
+        assert (
+            nextcarry.nplike is self._backend.index_nplike
+            and offsets.nplike is self._backend.index_nplike
+            and self._starts.nplike is self._backend.index_nplike
+            and self._stops.nplike is self._backend.index_nplike
+        )
+        self._backend.maybe_kernel_error(
+            self._backend[
+                "awkward_ListArray_broadcast_tooffsets",
+                nextcarry.dtype.type,
+                offsets.dtype.type,
+                self._starts.dtype.type,
+                self._stops.dtype.type,
+            ](
+                nextcarry.data,
+                offsets.data,
+                offsets.length,
+                self._starts.data,
+                self._stops.data,
+                self._content.length,
+            )
+        )
+
+        nextcontent = self._content._carry(nextcarry, True)
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+        return ListOffsetArray(offsets, nextcontent, parameters=self._parameters)
+
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         slicestarts = slicestarts.to_nplike(self._backend.index_nplike)
         slicestops = slicestops.to_nplike(self._backend.index_nplike)
         if self._backend.nplike.known_data and slicestarts.length != self.length:
             raise ak._errors.index_error(
                 self,
                 ak.contents.ListArray(
                     slicestarts, slicestops, slicecontent, parameters=None
@@ -408,15 +464,15 @@
             assert (
                 outoffsets.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
                 and self._starts.nplike is self._backend.index_nplike
                 and self._stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_descend",
                     outoffsets.dtype.type,
                     slicestarts.dtype.type,
                     slicestops.dtype.type,
                     self._starts.dtype.type,
                     self._stops.dtype.type,
@@ -449,15 +505,15 @@
         elif isinstance(slicecontent, ak.contents.NumpyArray):
             _carrylen = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _carrylen.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_carrylen",
                     _carrylen.dtype.type,
                     slicestarts.dtype.type,
                     slicestops.dtype.type,
                 ](
                     _carrylen.data,
@@ -481,15 +537,15 @@
                 and nextcarry.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
                 and sliceindex.nplike is self._backend.index_nplike
                 and self._starts.nplike is self._backend.index_nplike
                 and self._stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_apply",
                     outoffsets.dtype.type,
                     nextcarry.dtype.type,
                     slicestarts.dtype.type,
                     slicestops.dtype.type,
                     sliceindex.dtype.type,
@@ -532,15 +588,15 @@
             _numvalid = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _numvalid.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
                 and missing.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_numvalid",
                     _numvalid.dtype.type,
                     slicestarts.dtype.type,
                     slicestops.dtype.type,
                     missing.dtype.type,
                 ](
@@ -570,15 +626,15 @@
                 nextcarry.nplike is self._backend.index_nplike
                 and smalloffsets.nplike is self._backend.index_nplike
                 and largeoffsets.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
                 and missing.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_shrink",
                     nextcarry.dtype.type,
                     smalloffsets.dtype.type,
                     largeoffsets.dtype.type,
                     slicestarts.dtype.type,
                     slicestops.dtype.type,
@@ -660,15 +716,15 @@
             lenstarts = self._starts.length
             nextcarry = ak.index.Index64.empty(lenstarts, self._backend.index_nplike)
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and self._starts.nplike is self._backend.index_nplike
                 and self._stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_next_at",
                     nextcarry.dtype.type,
                     self._starts.dtype.type,
                     self._stops.dtype.type,
                 ](
                     nextcarry.data,
@@ -696,15 +752,15 @@
             if self._backend.nplike.known_data:
                 carrylength = ak.index.Index64.empty(1, self._backend.index_nplike)
                 assert (
                     carrylength.nplike is self._backend.index_nplike
                     and self._starts.nplike is self._backend.index_nplike
                     and self._stops.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_range_carrylength",
                         carrylength.dtype.type,
                         self._starts.dtype.type,
                         self._stops.dtype.type,
                     ](
                         carrylength.data,
@@ -742,15 +798,15 @@
 
             assert (
                 nextoffsets.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
                 and self._starts.nplike is self._backend.index_nplike
                 and self._stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_next_range",
                     nextoffsets.dtype.type,
                     nextcarry.dtype.type,
                     self._starts.dtype.type,
                     self._stops.dtype.type,
                 ](
@@ -779,15 +835,15 @@
             else:
                 if self._backend.nplike.known_data:
                     total = ak.index.Index64.empty(1, self._backend.index_nplike)
                     assert (
                         total.nplike is self._backend.index_nplike
                         and nextoffsets.nplike is self._backend.index_nplike
                     )
-                    self._handle_error(
+                    self._maybe_index_error(
                         self._backend[
                             "awkward_ListArray_getitem_next_range_counts",
                             total.dtype.type,
                             nextoffsets.dtype.type,
                         ](
                             total.data,
                             nextoffsets.data,
@@ -805,15 +861,15 @@
                     )
                 advanced = advanced.to_nplike(self._backend.index_nplike)
                 assert (
                     nextadvanced.nplike is self._backend.index_nplike
                     and advanced.nplike is self._backend.index_nplike
                     and nextoffsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_range_spreadadvanced",
                         nextadvanced.dtype.type,
                         advanced.dtype.type,
                         nextoffsets.dtype.type,
                     ](
                         nextadvanced.data,
@@ -865,15 +921,15 @@
                 assert (
                     nextcarry.nplike is self._backend.index_nplike
                     and nextadvanced.nplike is self._backend.index_nplike
                     and self._starts.nplike is self._backend.index_nplike
                     and self._stops.nplike is self._backend.index_nplike
                     and regular_flathead.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_array",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         self._starts.dtype.type,
                         self._stops.dtype.type,
                         regular_flathead.dtype.type,
@@ -911,15 +967,15 @@
                     nextcarry.nplike is self._backend.index_nplike
                     and nextadvanced.nplike is self._backend.index_nplike
                     and self._starts.nplike is self._backend.index_nplike
                     and self._stops.nplike is self._backend.index_nplike
                     and regular_flathead.nplike is self._backend.index_nplike
                     and advanced.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_array_advanced",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         self._starts.dtype.type,
                         self._stops.dtype.type,
                         regular_flathead.dtype.type,
@@ -966,15 +1022,15 @@
                 multistarts.nplike is self._backend.index_nplike
                 and multistops.nplike is self._backend.index_nplike
                 and singleoffsets.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
                 and self._starts.nplike is self._backend.index_nplike
                 and self._stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_jagged_expand",
                     multistarts.dtype.type,
                     multistops.dtype.type,
                     singleoffsets.dtype.type,
                     nextcarry.dtype.type,
                     self._starts.dtype.type,
@@ -1002,18 +1058,18 @@
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         return self.to_ListOffsetArray64(True)._offsets_and_flattened(axis, depth)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
@@ -1029,15 +1085,15 @@
         ):
             return self._content._mergeable_next(other.content, mergebool)
         elif isinstance(other, ak.contents.NumpyArray) and len(other.shape) > 1:
             return self._mergeable_next(other._to_regular_primitive(), mergebool)
         else:
             return False
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         head, tail = self._merging_strategy(others)
 
         total_length = 0
         for array in head:
@@ -1092,15 +1148,15 @@
 
                 assert (
                     nextstarts.nplike is self._backend.index_nplike
                     and nextstops.nplike is self._backend.index_nplike
                     and array_starts.nplike is self._backend.index_nplike
                     and array_stops.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListArray_fill",
                         nextstarts.dtype.type,
                         nextstops.dtype.type,
                         array_starts.dtype.type,
                         array_stops.dtype.type,
                     ](
@@ -1126,15 +1182,15 @@
 
                 assert (
                     nextstarts.nplike is self._backend.index_nplike
                     and nextstops.nplike is self._backend.index_nplike
                     and array_starts.nplike is self._backend.index_nplike
                     and array_stops.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListArray_fill",
                         nextstarts.dtype.type,
                         nextstops.dtype.type,
                         array_starts.dtype.type,
                         array_stops.dtype.type,
                     ](
@@ -1186,15 +1242,15 @@
                 offsets[-1]
             )  # todo: removed touch_data?
             localindex = ak.index.Index64.empty(innerlength, self._backend.index_nplike)
             assert (
                 localindex.nplike is self._backend.index_nplike
                 and offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListArray_localindex",
                     localindex.dtype.type,
                     offsets.dtype.type,
                 ](
                     localindex.data,
                     offsets.data,
@@ -1322,15 +1378,15 @@
             elif posaxis is not None and posaxis + 1 == depth + 1:
                 _min = ak.index.Index64.empty(1, self._backend.index_nplike)
                 assert (
                     _min.nplike is self._backend.index_nplike
                     and self._starts.nplike is self._backend.index_nplike
                     and self._stops.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListArray_min_range",
                         _min.dtype.type,
                         self._starts.dtype.type,
                         self._stops.dtype.type,
                     ](
                         _min.data,
@@ -1347,15 +1403,15 @@
                 else:
                     _tolength = ak.index.Index64.empty(1, self._backend.index_nplike)
                     assert (
                         _tolength.nplike is self._backend.index_nplike
                         and self._starts.nplike is self._backend.index_nplike
                         and self._stops.nplike is self._backend.index_nplike
                     )
-                    self._handle_error(
+                    self._backend.maybe_kernel_error(
                         self._backend[
                             "awkward_ListArray_rpad_and_clip_length_axis1",
                             _tolength.dtype.type,
                             self._starts.dtype.type,
                             self._stops.dtype.type,
                         ](
                             _tolength.data,
@@ -1379,15 +1435,15 @@
                     assert (
                         index.nplike is self._backend.index_nplike
                         and self._starts.nplike is self._backend.index_nplike
                         and self._stops.nplike is self._backend.index_nplike
                         and starts_.nplike is self._backend.index_nplike
                         and stops_.nplike is self._backend.index_nplike
                     )
-                    self._handle_error(
+                    self._backend.maybe_kernel_error(
                         self._backend[
                             "awkward_ListArray_rpad_axis1",
                             index.dtype.type,
                             self._starts.dtype.type,
                             self._stops.dtype.type,
                             starts_.dtype.type,
                             stops_.dtype.type,
@@ -1435,15 +1491,15 @@
             return backend.nplike.asarray(self.to_list(), dtype=dtype)
         else:
             return self.to_RegularArray()._to_backend_array(allow_missing, backend)
 
     def _remove_structure(self, backend, options):
         return self.to_ListOffsetArray64(False)._remove_structure(backend, options)
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.to_ListOffsetArray64()._drop_none()
 
     def _rebuild_without_nones(self, none_indexes, new_content):
         return self.to_ListOffsetArray64()._rebuild_without_nones(
             none_indexes, new_content
         )
```

### Comparing `awkward-2.2.1/src/awkward/contents/listoffsetarray.py` & `awkward-2.2.2/src/awkward/contents/listoffsetarray.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import TypeTracer, is_unknown_scalar
 from awkward._parameters import (
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.listoffsetform import ListOffsetForm
-from awkward.index import Index
+from awkward.index import Index, Index64
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -137,19 +139,19 @@
         assert offsets.nplike is content.backend.index_nplike
 
         self._offsets = offsets
         self._content = content
         self._init(parameters, content.backend)
 
     @property
-    def offsets(self):
+    def offsets(self) -> Index:
         return self._offsets
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     form_cls: Final = ListOffsetForm
 
     def copy(self, offsets=UNSET, content=UNSET, *, parameters=UNSET):
         return ListOffsetArray(
             self._offsets if offsets is UNSET else offsets,
@@ -168,31 +170,38 @@
         )
 
     @classmethod
     def simplified(cls, offsets, content, *, parameters=None):
         return cls(offsets, content, parameters=parameters)
 
     @property
-    def starts(self):
+    def starts(self) -> Index:
         return self._offsets[:-1]
 
     @property
     def stops(self):
         return self._offsets[1:]
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> ListOffsetForm:
         form_key = getkey(self)
         return self.form_cls(
             self._offsets.form,
             self._content._form_with_key(getkey),
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "offsets")
         container[key] = ak._util.native_to_byteorder(
             self._offsets.raw(backend.index_nplike), byteorder
         )
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
@@ -200,28 +209,26 @@
         offsets = self._offsets.to_nplike(TypeTracer.instance())
         return ListOffsetArray(
             offsets.forget_length() if forget_length else offsets,
             self._content._to_typetracer(False),
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._offsets.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._offsets._touch_data()
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._offsets.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._offsets._touch_shape()
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._offsets.length - 1
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<ListOffsetArray len="]
@@ -231,53 +238,40 @@
         out.append("\n")
         out.append(self._offsets._repr(indent + "    ", "<offsets>", "</offsets>\n"))
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</ListOffsetArray>")
         out.append(post)
         return "".join(out)
 
-    def to_ListOffsetArray64(self, start_at_zero=False):
-        if not self._backend.nplike.known_data and (
-            start_at_zero or self._offsets.dtype != np.dtype(np.int64)
-        ):
-            self._touch_data(recursive=False)
-            self._content._touch_data(recursive=False)
-
-        if issubclass(self._offsets.dtype.type, np.int64):
-            if (
-                not self._backend.nplike.known_data
-                or self._offsets[0] == 0
-                or not start_at_zero
-            ):
-                return self
-
-            if start_at_zero:
-                offsets = ak.index.Index64(
-                    self._offsets.raw(self._backend.nplike) - self._offsets[0],
-                    nplike=self._backend.index_nplike,
-                )
-                content = self._content[self._offsets[0] :]
-            else:
-                offsets, content = self._offsets, self._content
-
-            return ListOffsetArray(offsets, content, parameters=self._parameters)
-
+    def to_ListOffsetArray64(self, start_at_zero: bool = False) -> ListOffsetArray:
+        known_starts_at_zero = (
+            self._backend.index_nplike.known_data and self._offsets[0] == 0
+        )
+        if start_at_zero and not known_starts_at_zero:
+            offsets = Index64(
+                self._offsets.data - self._offsets[0],
+                nplike=self._backend.index_nplike,
+            )
+            return ListOffsetArray(
+                offsets, self._content[self._offsets[0] :], parameters=self._parameters
+            )
         else:
-            offsets = self._compact_offsets64(start_at_zero)
-            return self._broadcast_tooffsets64(offsets)
+            return ListOffsetArray(
+                self._offsets.to64(), self._content, parameters=self._parameters
+            )
 
     def to_RegularArray(self):
         start, stop = self._offsets[0], self._offsets[self._offsets.length - 1]
         content = self._content._getitem_range(start, stop)
-        _size = ak.index.Index64.empty(1, self._backend.index_nplike)
+        _size = Index64.empty(1, self._backend.index_nplike)
         assert (
             _size.nplike is self._backend.index_nplike
             and self._offsets.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListOffsetArray_toRegularArray",
                 _size.dtype.type,
                 self._offsets.dtype.type,
             ](
                 _size.data,
                 self._offsets.data,
@@ -312,15 +306,15 @@
         if not self._backend.nplike.known_data:
             self._touch_shape(recursive=False)
             return self
 
         offsets = self._offsets[start : stop + 1]
         if offsets.length is not unknown_length and offsets.length == 0:
             offsets = Index(
-                self._backend.index_nplike.asarray([0], dtype=self._offsets.dtype),
+                self._backend.index_nplike.zeros(1, dtype=self._offsets.dtype),
                 nplike=self._backend.index_nplike,
             )
         return ListOffsetArray(offsets, self._content, parameters=self._parameters)
 
     def _getitem_field(
         self, where: str | SupportsIndex, only_fields: tuple[str, ...] = ()
     ) -> Content:
@@ -348,76 +342,71 @@
         except IndexError as err:
             raise ak._errors.index_error(self, carry.data, str(err)) from err
 
         return ak.contents.ListArray(
             nextstarts, nextstops, self._content, parameters=self._parameters
         )
 
-    def _compact_offsets64(self, start_at_zero):
-        offsets_len = self._offsets.length - 1
-        out = ak.index.Index64.empty(self._offsets.length, self._backend.index_nplike)
-        assert (
-            out.nplike is self._backend.index_nplike
-            and self._offsets.nplike is self._backend.index_nplike
-        )
-        self._handle_error(
-            self._backend[
-                "awkward_ListOffsetArray_compact_offsets",
-                out.dtype.type,
-                self._offsets.dtype.type,
-            ](out.data, self._offsets.data, offsets_len)
-        )
-        return out
+    def _compact_offsets64(self, start_at_zero: bool) -> Index64:
+        if not start_at_zero or (
+            self._backend.index_nplike.known_data and self._offsets[0] == 0
+        ):
+            return self._offsets
+        else:
+            return Index64(
+                self._offsets.data - self._offsets[0],
+                nplike=self._backend.index_nplike,
+            )
 
-    def _broadcast_tooffsets64(self, offsets):
-        if offsets.nplike.known_data and (offsets.length == 0 or offsets[0] != 0):
+    def _broadcast_tooffsets64(self, offsets: Index) -> ListOffsetArray:
+        self._touch_data(recursive=False)
+        offsets._touch_data()
+
+        index_nplike = self._backend.index_nplike
+        assert offsets.nplike is index_nplike
+        if offsets.length is not unknown_length and offsets.length == 0:
             raise AssertionError(
-                "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
-                    "(empty)" if offsets.length == 0 else str(offsets[0])
-                )
+                "broadcast_tooffsets64 can only be used with non-empty offsets"
             )
-
-        if offsets.nplike.known_data and offsets.length - 1 != self.length:
+        elif index_nplike.known_data and offsets[0] != 0:
+            raise AssertionError(
+                f"broadcast_tooffsets64 can only be used with offsets that start at 0, not {offsets[0]}"
+            )
+        elif (
+            offsets.length is not unknown_length
+            and self._offsets.length is not unknown_length
+            and offsets.length != self._offsets.length
+        ):
             raise AssertionError(
-                "cannot broadcast {} of length {} to length {}".format(
-                    type(self).__name__, self.length, offsets.length - 1
+                "cannot broadcast RegularArray of length {} to length {}".format(
+                    self.length, offsets.length - 1
                 )
             )
 
-        starts, stops = self.starts, self.stops
-
-        nextcarry = ak.index.Index64.empty(offsets[-1], self._backend.index_nplike)
-        assert (
-            nextcarry.nplike is self._backend.index_nplike
-            and offsets.nplike is self._backend.index_nplike
-            and starts.nplike is self._backend.index_nplike
-            and stops.nplike is self._backend.index_nplike
-        )
-        self._handle_error(
-            self._backend[
-                "awkward_ListArray_broadcast_tooffsets",
-                nextcarry.dtype.type,
-                offsets.dtype.type,
-                starts.dtype.type,
-                stops.dtype.type,
-            ](
-                nextcarry.data,
-                offsets.data,
-                offsets.length,
-                starts.data,
-                stops.data,
-                self._content.length,
-            )
-        )
+        # Check whether we need to slice the content, shift our offsets
+        this_start = self._offsets[0]
+        this_zero_offsets = self._offsets.data
+        if index_nplike.known_data and this_start == 0:
+            next_content = self._content
+        else:
+            this_zero_offsets = this_zero_offsets - this_start
+            next_content = self._content[this_start:]
 
-        nextcontent = self._content._carry(nextcarry, True)
+        if index_nplike.known_data and not index_nplike.array_equal(
+            this_zero_offsets, offsets
+        ):
+            raise ValueError("cannot broadcast nested list")
 
-        return ListOffsetArray(offsets, nextcontent, parameters=self._parameters)
+        return ListOffsetArray(
+            offsets, next_content[: offsets[-1]], parameters=self._parameters
+        )
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         out = ak.contents.ListArray(
             self.starts, self.stops, self._content, parameters=self._parameters
         )
         return out._getitem_next_jagged(slicestarts, slicestops, slicecontent, tail)
 
     def _getitem_next(
         self,
@@ -430,22 +419,22 @@
             return self
 
         elif is_integer_like(head):
             assert advanced is None
             lenstarts = self._offsets.length - 1
             starts, stops = self.starts, self.stops
             nexthead, nexttail = ak._slicing.head_tail(tail)
-            nextcarry = ak.index.Index64.empty(lenstarts, self._backend.index_nplike)
+            nextcarry = Index64.empty(lenstarts, self._backend.index_nplike)
 
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
                 and stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_next_at",
                     nextcarry.dtype.type,
                     starts.dtype.type,
                     stops.dtype.type,
                 ](
                     nextcarry.data,
@@ -464,21 +453,21 @@
             lenstarts = self._offsets.length - 1
             start, stop, step = head.start, head.stop, head.step
 
             step = 1 if step is None else step
             start = ak._util.kSliceNone if start is None else start
             stop = ak._util.kSliceNone if stop is None else stop
 
-            carrylength = ak.index.Index64.empty(1, self._backend.index_nplike)
+            carrylength = Index64.empty(1, self._backend.index_nplike)
             assert (
                 carrylength.nplike is self._backend.index_nplike
                 and self.starts.nplike is self._backend.index_nplike
                 and self.stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_next_range_carrylength",
                     carrylength.dtype.type,
                     self.starts.dtype.type,
                     self.stops.dtype.type,
                 ](
                     carrylength.data,
@@ -489,36 +478,34 @@
                     stop,
                     step,
                 ),
                 slicer=head,
             )
 
             if self._starts.dtype == "int64":
-                nextoffsets = ak.index.Index64.empty(
+                nextoffsets = Index64.empty(
                     lenstarts + 1, nplike=self._backend.index_nplike
                 )
             elif self._starts.dtype == "int32":
                 nextoffsets = ak.index.Index32.empty(
                     lenstarts + 1, nplike=self._backend.index_nplike
                 )
             elif self._starts.dtype == "uint32":
                 nextoffsets = ak.index.IndexU32.empty(
                     lenstarts + 1, nplike=self._backend.index_nplike
                 )
-            nextcarry = ak.index.Index64.empty(
-                carrylength[0], self._backend.index_nplike
-            )
+            nextcarry = Index64.empty(carrylength[0], self._backend.index_nplike)
 
             assert (
                 nextoffsets.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
                 and self.starts.nplike is self._backend.index_nplike
                 and self.stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_ListArray_getitem_next_range",
                     nextoffsets.dtype.type,
                     nextcarry.dtype.type,
                     self.starts.dtype.type,
                     self.stops.dtype.type,
                 ](
@@ -542,41 +529,39 @@
                 return ak.contents.ListOffsetArray(
                     nextoffsets,
                     nextcontent._getitem_next(nexthead, nexttail, advanced),
                     parameters=self._parameters,
                 )
 
             else:
-                total = ak.index.Index64.empty(1, self._backend.index_nplike)
+                total = Index64.empty(1, self._backend.index_nplike)
                 assert (
                     total.nplike is self._backend.index_nplike
                     and nextoffsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_range_counts",
                         total.dtype.type,
                         nextoffsets.dtype.type,
                     ](
                         total.data,
                         nextoffsets.data,
                         lenstarts,
                     ),
                     slicer=head,
                 )
 
-                nextadvanced = ak.index.Index64.empty(
-                    total[0], self._backend.index_nplike
-                )
+                nextadvanced = Index64.empty(total[0], self._backend.index_nplike)
                 assert (
                     nextadvanced.nplike is self._backend.index_nplike
                     and advanced.nplike is self._backend.index_nplike
                     and nextoffsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_range_spreadadvanced",
                         nextadvanced.dtype.type,
                         advanced.dtype.type,
                         nextoffsets.dtype.type,
                     ](
                         nextadvanced.data,
@@ -601,36 +586,36 @@
 
         elif head is np.newaxis:
             return self._getitem_next_newaxis(tail, advanced)
 
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
-        elif isinstance(head, ak.index.Index64):
+        elif isinstance(head, Index64):
             nexthead, nexttail = ak._slicing.head_tail(tail)
             flathead = self._backend.index_nplike.reshape(
                 self._backend.index_nplike.asarray(head.data), (-1,)
             )
             lenstarts = self.starts.length
-            regular_flathead = ak.index.Index64(flathead)
+            regular_flathead = Index64(flathead)
             if advanced is None or (
                 advanced.length is not unknown_length and advanced.length == 0
             ):
-                nextcarry = ak.index.Index64.empty(
+                nextcarry = Index64.empty(
                     lenstarts * flathead.length, self._backend.index_nplike
                 )
-                nextadvanced = ak.index.Index64.empty(
+                nextadvanced = Index64.empty(
                     lenstarts * flathead.length, self._backend.index_nplike
                 )
                 assert (
                     nextcarry.nplike is self._backend.index_nplike
                     and nextadvanced.nplike is self._backend.index_nplike
                     and regular_flathead.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_array",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         regular_flathead.dtype.type,
                     ](
                         nextcarry.data,
@@ -651,29 +636,25 @@
                     return ak._slicing.getitem_next_array_wrap(
                         out, head.metadata.get("shape", (head.length,), self.length)
                     )
                 else:
                     return out
 
             else:
-                nextcarry = ak.index.Index64.empty(
-                    self.length, self._backend.index_nplike
-                )
-                nextadvanced = ak.index.Index64.empty(
-                    self.length, self._backend.index_nplike
-                )
+                nextcarry = Index64.empty(self.length, self._backend.index_nplike)
+                nextadvanced = Index64.empty(self.length, self._backend.index_nplike)
                 assert (
                     nextcarry.nplike is self._backend.index_nplike
                     and nextadvanced.nplike is self._backend.index_nplike
                     and self.starts.nplike is self._backend.index_nplike
                     and self.stops.nplike is self._backend.index_nplike
                     and regular_flathead.nplike is self._backend.index_nplike
                     and advanced.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_ListArray_getitem_next_array_advanced",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         self.starts.dtype.type,
                         self.stops.dtype.type,
                         regular_flathead.dtype.type,
@@ -702,30 +683,39 @@
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
+            if (
+                self.parameter("__array__") == "string"
+                or self.parameter("__array__") == "bytestring"
+            ):
+                raise ValueError(
+                    "array of strings cannot be directly flattened. "
+                    'To flatten this array, drop the `"__array__"="string"` parameter using '
+                    "`ak.enforce_type`, `ak.with_parameter`, or `ak.without_parameters`/"
+                )
             listoffsetarray = self.to_ListOffsetArray64(True)
             stop = listoffsetarray.offsets[-1]
             content = listoffsetarray.content._getitem_range(0, stop)
             return (listoffsetarray.offsets, content)
 
         else:
             inneroffsets, flattened = self._content._offsets_and_flattened(
                 axis, depth + 1
             )
-            offsets = ak.index.Index64.zeros(
+            offsets = Index64.zeros(
                 0,
                 nplike=self._backend.index_nplike,
                 dtype=np.int64,
             )
 
             if inneroffsets.length is not unknown_length and inneroffsets.length == 0:
                 return (
@@ -734,32 +724,32 @@
                         self._offsets, flattened, parameters=self._parameters
                     ),
                 )
 
             elif (
                 self._offsets.length is not unknown_length and self._offsets.length == 1
             ):
-                tooffsets = ak.index.Index64([inneroffsets[0]])
+                tooffsets = Index64([inneroffsets[0]])
                 return (
                     offsets,
                     ListOffsetArray(tooffsets, flattened, parameters=self._parameters),
                 )
 
             else:
-                tooffsets = ak.index.Index64.empty(
+                tooffsets = Index64.empty(
                     self._offsets.length,
                     self._backend.index_nplike,
                     dtype=np.int64,
                 )
                 assert (
                     tooffsets.nplike is self._backend.index_nplike
                     and self._offsets.nplike is self._backend.index_nplike
                     and inneroffsets.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_flatten_offsets",
                         tooffsets.dtype.type,
                         self._offsets.dtype.type,
                         inneroffsets.dtype.type,
                     ](
                         tooffsets.data,
@@ -770,15 +760,15 @@
                     )
                 )
                 return (
                     offsets,
                     ListOffsetArray(tooffsets, flattened, parameters=self._parameters),
                 )
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
@@ -794,15 +784,15 @@
         ):
             return self._content._mergeable_next(other.content, mergebool)
         elif isinstance(other, ak.contents.NumpyArray) and len(other.shape) > 1:
             return self._mergeable_next(other._to_regular_primitive(), mergebool)
         else:
             return False
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
         listarray = ak.contents.ListArray(
             self.starts, self.stops, self._content, parameters=self._parameters
         )
         out = listarray._mergemany(others)
 
@@ -829,17 +819,17 @@
             if self._backend.nplike.known_data:
                 innerlength = index_nplike.index_as_shape_item(
                     offsets[index_nplike.shape_item_as_index(offsets.length) - 1]
                 )
             else:
                 self._touch_data(recursive=False)
                 innerlength = unknown_length
-            localindex = ak.index.Index64.empty(innerlength, index_nplike)
+            localindex = Index64.empty(innerlength, index_nplike)
             assert localindex.nplike is index_nplike and offsets.nplike is index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListArray_localindex",
                     localindex.dtype.type,
                     offsets.dtype.type,
                 ](
                     localindex.data,
                     offsets.data,
@@ -887,23 +877,23 @@
 
         if negaxis is None:
             return self._content._is_unique(negaxis, starts, parents, outlength)
 
         if not branch and (negaxis == depth):
             return self._content._is_unique(negaxis - 1, starts, parents, outlength)
         else:
-            nextparents = ak.index.Index64.empty(
+            nextparents = Index64.empty(
                 self._offsets[-1] - self._offsets[0], self._backend.index_nplike
             )
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_nextparents_64",
                     nextparents.dtype.type,
                     self._offsets.dtype.type,
                 ](
                     nextparents.data,
                     self._offsets.data,
@@ -958,22 +948,20 @@
             outcontent = nextcontent._unique(
                 negaxis - 1,
                 nextstarts,
                 nextparents,
                 maxnextparents[0] + 1,
             )
 
-            outcarry = ak.index.Index64.empty(
-                nextcarry.length, self._backend.index_nplike
-            )
+            outcarry = Index64.empty(nextcarry.length, self._backend.index_nplike)
             assert (
                 outcarry.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_local_preparenext_64",
                     outcarry.dtype.type,
                     nextcarry.dtype.type,
                 ](
                     outcarry.data,
                     nextcarry.data,
@@ -984,23 +972,23 @@
             return ak.contents.ListOffsetArray(
                 outcontent._compact_offsets64(True),
                 outcontent._content._carry(outcarry, False),
                 parameters=self._parameters,
             )
 
         else:
-            nextparents = ak.index.Index64.empty(
+            nextparents = Index64.empty(
                 self._offsets[-1] - self._offsets[0], self._backend.index_nplike
             )
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_nextparents_64",
                     nextparents.dtype.type,
                     self._offsets.dtype.type,
                 ](
                     nextparents.data,
                     self._offsets.data,
@@ -1042,27 +1030,27 @@
         ):
             if branch or (negaxis != depth):
                 raise AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
-                nextcarry = ak.index.Index64.empty(
+                nextcarry = Index64.empty(
                     self._offsets.length - 1, self._backend.index_nplike
                 )
 
                 self_starts, self_stops = self._offsets[:-1], self._offsets[1:]
                 assert (
                     nextcarry.nplike is self._backend.index_nplike
                     and parents.nplike is self._backend.index_nplike
                     and self._content.backend is self._backend
                     and self_starts.nplike is self._backend.index_nplike
                     and self_stops.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_argsort_strings",
                         nextcarry.dtype.type,
                         parents.dtype.type,
                         self._content.dtype.type,
                         self_starts.dtype.type,
                         self_stops.dtype.type,
@@ -1097,32 +1085,28 @@
                 maxcount,
                 maxnextparents,
                 nextcarry,
                 nextparents,
                 nextstarts,
             ) = self._rearrange_prepare_next(outlength, parents)
 
-            nummissing = ak.index.Index64.empty(maxcount, self._backend.index_nplike)
-            missing = ak.index.Index64.empty(
-                self._offsets[-1], self._backend.index_nplike
-            )
-            nextshifts = ak.index.Index64.empty(
-                nextcarry.length, self._backend.index_nplike
-            )
+            nummissing = Index64.empty(maxcount, self._backend.index_nplike)
+            missing = Index64.empty(self._offsets[-1], self._backend.index_nplike)
+            nextshifts = Index64.empty(nextcarry.length, self._backend.index_nplike)
             assert (
                 nummissing.nplike is self._backend.index_nplike
                 and missing.nplike is self._backend.index_nplike
                 and nextshifts.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
             )
 
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64",
                     nummissing.dtype.type,
                     missing.dtype.type,
                     nextshifts.dtype.type,
                     self._offsets.dtype.type,
                     starts.dtype.type,
@@ -1149,22 +1133,20 @@
                 nextshifts,
                 nextparents,
                 nextstarts.length,
                 ascending,
                 stable,
             )
 
-            outcarry = ak.index.Index64.empty(
-                nextcarry.length, self._backend.index_nplike
-            )
+            outcarry = Index64.empty(nextcarry.length, self._backend.index_nplike)
             assert (
                 outcarry.nplike is self._backend.index_nplike
                 and nextcarry.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_local_preparenext_64",
                     outcarry.dtype.type,
                     nextcarry.dtype.type,
                 ](
                     outcarry.data,
                     nextcarry.data,
@@ -1174,26 +1156,26 @@
 
             out_offsets = self._compact_offsets64(True)
             out = outcontent._carry(outcarry, False)
             return ak.contents.ListOffsetArray(
                 out_offsets, out, parameters=self._parameters
             )
         else:
-            nextparents = ak.index.Index64.empty(
+            nextparents = Index64.empty(
                 self._backend.index_nplike.index_as_shape_item(
                     self._offsets[-1] - self._offsets[0]
                 ),
                 self._backend.index_nplike,
             )
 
             assert (
                 nextparents.nplike is self._backend.index_nplike
                 and self._offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_nextparents_64",
                     nextparents.dtype.type,
                     self._offsets.dtype.type,
                 ](
                     nextparents.data,
                     self._offsets.data,
@@ -1227,27 +1209,25 @@
         ):
             if branch or (negaxis != depth):
                 raise AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
-                nextcarry = ak.index.Index64.empty(
-                    self._offsets.length - 1, index_nplike
-                )
+                nextcarry = Index64.empty(self._offsets.length - 1, index_nplike)
 
                 starts, stops = self._offsets[:-1], self._offsets[1:]
                 assert (
                     nextcarry.nplike is index_nplike
                     and parents.nplike is index_nplike
                     and self._content.backend is self._backend
                     and starts.nplike is index_nplike
                     and stops.nplike is index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_argsort_strings",
                         nextcarry.dtype.type,
                         parents.dtype.type,
                         self._content.dtype.type,
                         starts.dtype.type,
                         stops.dtype.type,
@@ -1290,17 +1270,17 @@
                 nextstarts,
                 nextparents,
                 maxnextparents + 1,
                 ascending,
                 stable,
             )
 
-            outcarry = ak.index.Index64.empty(nextcarry.length, index_nplike)
+            outcarry = Index64.empty(nextcarry.length, index_nplike)
             assert outcarry.nplike is index_nplike and nextcarry.nplike is index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_local_preparenext_64",
                     outcarry.dtype.type,
                     nextcarry.dtype.type,
                 ](
                     outcarry.data,
                     nextcarry.data,
@@ -1310,25 +1290,25 @@
 
             return ak.contents.ListOffsetArray(
                 self._compact_offsets64(True),
                 outcontent._carry(outcarry, False),
                 parameters=self._parameters,
             )
         else:
-            nextparents = ak.index.Index64.empty(
+            nextparents = Index64.empty(
                 index_nplike.index_as_shape_item(self._offsets[-1] - self._offsets[0]),
                 index_nplike,
             )
             lenstarts = self._offsets.length - 1
 
             assert (
                 nextparents.nplike is index_nplike
                 and self._offsets.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_nextparents_64",
                     nextparents.dtype.type,
                     self._offsets.dtype.type,
                 ](
                     nextparents.data,
                     self._offsets.data,
@@ -1364,26 +1344,26 @@
                 raise ValueError(
                     "ak.combinations does not compute combinations of the characters of a string; please split it into lists"
                 )
 
             starts = self.starts
             stops = self.stops
 
-            _totallen = ak.index.Index64.empty(1, index_nplike, dtype=np.int64)
-            offsets = ak.index.Index64.empty(
+            _totallen = Index64.empty(1, index_nplike, dtype=np.int64)
+            offsets = Index64.empty(
                 self.length + 1,
                 index_nplike,
                 dtype=np.int64,
             )
             assert (
                 offsets.nplike is index_nplike
                 and starts.nplike is index_nplike
                 and stops.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListArray_combinations_length",
                     _totallen.data.dtype.type,
                     offsets.data.dtype.type,
                     starts.data.dtype.type,
                     stops.data.dtype.type,
                 ](
@@ -1398,32 +1378,32 @@
             )
             totallen = self._backend.index_nplike.index_as_shape_item(_totallen[0])
 
             tocarryraw = ak.index.Index.empty(n, dtype=np.intp, nplike=index_nplike)
             tocarry = []
 
             for i in range(n):
-                ptr = ak.index.Index64.empty(
+                ptr = Index64.empty(
                     totallen,
                     nplike=index_nplike,
                     dtype=np.int64,
                 )
                 tocarry.append(ptr)
                 if self._backend.nplike.known_data:
                     tocarryraw[i] = ptr.ptr
 
-            toindex = ak.index.Index64.empty(n, index_nplike, dtype=np.int64)
-            fromindex = ak.index.Index64.empty(n, index_nplike, dtype=np.int64)
+            toindex = Index64.empty(n, index_nplike, dtype=np.int64)
+            fromindex = Index64.empty(n, index_nplike, dtype=np.int64)
             assert (
                 toindex.nplike is index_nplike
                 and fromindex.nplike is index_nplike
                 and starts.nplike is index_nplike
                 and stops.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListArray_combinations",
                     np.int64,
                     toindex.data.dtype.type,
                     fromindex.data.dtype.type,
                     starts.data.dtype.type,
                     stops.data.dtype.type,
@@ -1500,22 +1480,22 @@
                 maxcount,
                 maxnextparents,
                 nextcarry,
                 nextparents,
                 nextstarts,
             ) = self._rearrange_prepare_next(outlength, parents)
 
-            outstarts = ak.index.Index64.empty(outlength, index_nplike)
-            outstops = ak.index.Index64.empty(outlength, index_nplike)
+            outstarts = Index64.empty(outlength, index_nplike)
+            outstops = Index64.empty(outlength, index_nplike)
             assert (
                 outstarts.nplike is index_nplike
                 and outstops.nplike is index_nplike
                 and distincts.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64",
                     outstarts.dtype.type,
                     outstops.dtype.type,
                     distincts.dtype.type,
                 ](
                     outstarts.data,
@@ -1523,31 +1503,31 @@
                     distincts.data,
                     distincts.length,
                     outlength,
                 )
             )
 
             if reducer.needs_position:
-                nextshifts = ak.index.Index64.empty(nextcarry.length, index_nplike)
-                nummissing = ak.index.Index64.empty(maxcount, index_nplike)
-                missing = ak.index.Index64.empty(
+                nextshifts = Index64.empty(nextcarry.length, index_nplike)
+                nummissing = Index64.empty(maxcount, index_nplike)
+                missing = Index64.empty(
                     index_nplike.index_as_shape_item(self._offsets[-1]),
                     index_nplike,
                 )
                 assert (
                     nummissing.nplike is index_nplike
                     and missing.nplike is index_nplike
                     and nextshifts.nplike is index_nplike
                     and self._offsets.nplike is index_nplike
                     and starts.nplike is index_nplike
                     and parents.nplike is index_nplike
                     and nextcarry.nplike is index_nplike
                 )
 
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64",
                         nummissing.dtype.type,
                         missing.dtype.type,
                         nextshifts.dtype.type,
                         self._offsets.dtype.type,
                         starts.dtype.type,
@@ -1591,21 +1571,21 @@
 
             return out
 
         else:
             nextlen = index_nplike.index_as_shape_item(
                 self._offsets[-1] - self._offsets[0]
             )
-            nextparents = ak.index.Index64.empty(nextlen, index_nplike)
+            nextparents = Index64.empty(nextlen, index_nplike)
 
             assert (
                 nextparents.nplike is index_nplike
                 and self._offsets.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_nextparents_64",
                     nextparents.dtype.type,
                     self._offsets.dtype.type,
                 ](
                     nextparents.data,
                     self._offsets.data,
@@ -1624,17 +1604,17 @@
                 nextparents,
                 globalstarts_length,
                 mask,
                 keepdims,
                 behavior,
             )
 
-            outoffsets = ak.index.Index64.empty(outlength + 1, index_nplike)
+            outoffsets = Index64.empty(outlength + 1, index_nplike)
             assert outoffsets.nplike is index_nplike and parents.nplike is index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_outoffsets_64",
                     outoffsets.dtype.type,
                     parents.dtype.type,
                 ](
                     outoffsets.data,
                     parents.data,
@@ -1659,53 +1639,52 @@
 
             return ak.contents.ListOffsetArray(outoffsets, outcontent, parameters=None)
 
     def _rearrange_prepare_next(self, outlength, parents):
         index_nplike = self._backend.index_nplike
         nextlen = index_nplike.index_as_shape_item(self._offsets[-1] - self._offsets[0])
         lenstarts = self._offsets.length - 1
-        _maxcount = ak.index.Index64.empty(1, index_nplike)
-        offsetscopy = ak.index.Index64.empty(self.offsets.length, index_nplike)
+        _maxcount = Index64.empty(1, index_nplike)
+        offsetscopy = Index64.empty(self.offsets.length, index_nplike)
         assert (
             _maxcount.nplike is index_nplike
             and offsetscopy.nplike is index_nplike
             and self._offsets.nplike is index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64",
                 _maxcount.dtype.type,
                 offsetscopy.dtype.type,
                 self._offsets.dtype.type,
             ](
                 _maxcount.data,
                 offsetscopy.data,
                 self._offsets.data,
                 lenstarts,
             )
         )
         maxcount = index_nplike.index_as_shape_item(_maxcount[0])
 
-        # A "stable" sort is essential for the subsequent steps.
-        nextcarry = ak.index.Index64.empty(nextlen, nplike=index_nplike)
-        nextparents = ak.index.Index64.empty(nextlen, nplike=index_nplike)
-        _maxnextparents = ak.index.Index64.empty(1, index_nplike)
+        nextcarry = Index64.empty(nextlen, nplike=index_nplike)
+        nextparents = Index64.empty(nextlen, nplike=index_nplike)
+        _maxnextparents = Index64.empty(1, index_nplike)
         if maxcount is unknown_length or outlength is unknown_length:
-            distincts = ak.index.Index64.empty(unknown_length, index_nplike)
+            distincts = Index64.empty(unknown_length, index_nplike)
         else:
-            distincts = ak.index.Index64.empty(outlength * maxcount, index_nplike)
+            distincts = Index64.empty(outlength * maxcount, index_nplike)
 
         assert (
             _maxnextparents.nplike is index_nplike
             and distincts.nplike is index_nplike
             and self._offsets.nplike is index_nplike
             and offsetscopy.nplike is index_nplike
             and parents.nplike is index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListOffsetArray_reduce_nonlocal_preparenext_64",
                 nextcarry.dtype.type,
                 nextparents.dtype.type,
                 _maxnextparents.dtype.type,
                 distincts.dtype.type,
                 self._offsets.dtype.type,
@@ -1722,17 +1701,17 @@
                 self._offsets.data,
                 lenstarts,
                 parents.data,
                 maxcount,
             )
         )
         maxnextparents = index_nplike.index_as_shape_item(_maxnextparents[0])
-        nextstarts = ak.index.Index64.empty(maxnextparents + 1, index_nplike)
+        nextstarts = Index64.empty(maxnextparents + 1, index_nplike)
         assert nextstarts.nplike is index_nplike and nextparents.nplike is index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64",
                 nextstarts.dtype.type,
                 nextparents.dtype.type,
             ](
                 nextstarts.data,
                 nextparents.data,
@@ -1784,42 +1763,42 @@
         posaxis = maybe_posaxis(self, axis, depth)
         index_nplike = self._backend.index_nplike
 
         if posaxis is not None and posaxis + 1 == depth:
             return self._pad_none_axis0(target, clip)
         if posaxis is not None and posaxis + 1 == depth + 1:
             if not clip:
-                _tolength = ak.index.Index64.empty(1, index_nplike)
-                offsets_ = ak.index.Index64.empty(self._offsets.length, index_nplike)
+                _tolength = Index64.empty(1, index_nplike)
+                offsets_ = Index64.empty(self._offsets.length, index_nplike)
                 assert (
                     offsets_.nplike is index_nplike
                     and self._offsets.nplike is index_nplike
                     and _tolength.nplike is index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_rpad_length_axis1",
                         offsets_.dtype.type,
                         self._offsets.dtype.type,
                         _tolength.dtype.type,
                     ](
                         offsets_.data,
                         self._offsets.data,
                         self._offsets.length - 1,
                         target,
                         _tolength.data,
                     )
                 )
                 tolength = index_nplike.index_as_shape_item(_tolength[0])
-                outindex = ak.index.Index64.empty(tolength, index_nplike)
+                outindex = Index64.empty(tolength, index_nplike)
                 assert (
                     outindex.nplike is index_nplike
                     and self._offsets.nplike is index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_rpad_axis1",
                         outindex.dtype.type,
                         self._offsets.dtype.type,
                     ](
                         outindex.data,
                         self._offsets.data,
@@ -1830,45 +1809,45 @@
                 next = ak.contents.IndexedOptionArray.simplified(
                     outindex, self._content, parameters=self._parameters
                 )
                 return ak.contents.ListOffsetArray(
                     offsets_, next, parameters=self._parameters
                 )
             else:
-                starts_ = ak.index.Index64.empty(
+                starts_ = Index64.empty(
                     self._offsets.length - 1,
                     index_nplike,
                 )
-                stops_ = ak.index.Index64.empty(
+                stops_ = Index64.empty(
                     self._offsets.length - 1,
                     index_nplike,
                 )
                 assert starts_.nplike is index_nplike and stops_.nplike is index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_index_rpad_and_clip_axis1",
                         starts_.dtype.type,
                         stops_.dtype.type,
                     ](
                         starts_.data,
                         stops_.data,
                         target,
                         starts_.length,
                     )
                 )
 
-                outindex = ak.index.Index64.empty(
+                outindex = Index64.empty(
                     target * (self._offsets.length - 1),
                     index_nplike,
                 )
                 assert (
                     outindex.nplike is index_nplike
                     and self._offsets.nplike is index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_ListOffsetArray_rpad_and_clip_axis1",
                         outindex.dtype.type,
                         self._offsets.dtype.type,
                     ](
                         outindex.data,
                         self._offsets.data,
@@ -2018,45 +1997,45 @@
             return [self]
         else:
             content = self._content[self._offsets[0] : self._offsets[-1]]
             contents = content._remove_structure(backend, options)
             if options["keepdims"]:
                 return [
                     ListOffsetArray(
-                        ak.index.Index64(
+                        Index64(
                             backend.index_nplike.asarray(
                                 [0, backend.index_nplike.shape_item_as_index(c.length)]
                             )
                         ),
                         c,
                         parameters=self._parameters,
                     )
                     for c in contents
                 ]
             else:
                 return contents
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         if self._content.is_option:
             _, _, none_indexes = self._content._nextcarry_outindex()
             new_content = self._content._drop_none()
             return self._rebuild_without_nones(none_indexes, new_content)
         else:
             return self
 
     def _rebuild_without_nones(self, none_indexes, new_content):
-        new_offsets = ak.index.Index64.empty(self._offsets.length, self._backend.nplike)
+        new_offsets = Index64.empty(self._offsets.length, self._backend.nplike)
 
         assert (
             new_offsets.nplike is self._backend.index_nplike
             and self._offsets.nplike is self._backend.index_nplike
             and none_indexes.nplike is self._backend.index_nplike
         )
 
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_ListOffsetArray_drop_none_indexes",
                 new_offsets.dtype.type,
                 none_indexes.dtype.type,
                 self._offsets.dtype.type,
             ](
                 new_offsets.data,
@@ -2218,15 +2197,15 @@
                 content = ak.contents.NumpyArray(numbers)
 
                 if has_another_string:
                     union_tags = ak.index.Index8.zeros(
                         content.length, nplike=self._backend.index_nplike
                     )
                     content.backend.nplike.isnan(content._data, union_tags._data)
-                    union_index = ak.index.Index64(
+                    union_index = Index64(
                         self._backend.index_nplike.arange(
                             content.length, dtype=np.int64
                         ),
                         nplike=self._backend.index_nplike,
                     )
 
                     return ak.contents.UnionArray(
```

### Comparing `awkward-2.2.1/src/awkward/contents/numpyarray.py` & `awkward-2.2.2/src/awkward/contents/numpyarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import to_nplike
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem
 from awkward._nplikes.typetracer import TypeTracerArray
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.numpyform import NumpyForm
 from awkward.index import Index
 from awkward.types.numpytype import primitive_to_dtype
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
@@ -149,41 +152,48 @@
         )
 
     @classmethod
     def simplified(cls, data, *, parameters=None, backend=None):
         return cls(data, parameters=parameters, backend=backend)
 
     @property
-    def shape(self):
+    def shape(self) -> tuple[ShapeItem, ...]:
         return self._data.shape
 
     @property
-    def inner_shape(self):
+    def inner_shape(self) -> tuple[ShapeItem, ...]:
         return self._data.shape[1:]
 
     @property
-    def strides(self):
-        return self._data.strides
+    def strides(self) -> tuple[ShapeItem, ...]:
+        return self._backend.nplike.strides(self._data)
 
     @property
-    def dtype(self):
+    def dtype(self) -> np.dtype:
         return self._data.dtype
 
     def _raw(self, nplike=None):
         return to_nplike(self.data, nplike, from_nplike=self._backend.nplike)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> NumpyForm:
         return self.form_cls(
             ak.types.numpytype.dtype_to_primitive(self._data.dtype),
             self._data.shape[1:],
             parameters=self._parameters,
             form_key=getkey(self),
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "data")
         container[key] = ak._util.native_to_byteorder(
             self._raw(backend.nplike), byteorder
         )
 
     def _to_typetracer(self, forget_length: bool) -> Self:
@@ -191,24 +201,24 @@
         data = self._raw(backend.nplike)
         return NumpyArray(
             data.forget_length() if forget_length else data,
             parameters=self._parameters,
             backend=backend,
         )
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         if not self._backend.nplike.known_data:
             self._data.touch_data()
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         if not self._backend.nplike.known_data:
             self._data.touch_shape()
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._data.shape[0]
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<NumpyArray dtype="]
@@ -316,15 +326,17 @@
         assert isinstance(carry, ak.index.Index)
         try:
             nextdata = self._data[carry.data]
         except IndexError as err:
             raise ak._errors.index_error(self, carry.data, str(err)) from err
         return NumpyArray(nextdata, parameters=self._parameters, backend=self._backend)
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         if self._data.ndim == 1:
             raise ak._errors.index_error(
                 self,
                 ak.contents.ListArray(
                     slicestarts, slicestops, slicecontent, parameters=None
                 ),
                 "too many jagged slice dimensions for array",
@@ -401,26 +413,26 @@
         elif isinstance(head, ak.contents.IndexedOptionArray):
             next = self.to_RegularArray()
             return next._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
 
         elif len(self.shape) != 1:
             return self.to_RegularArray()._offsets_and_flattened(axis, depth)
 
         else:
             raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
@@ -461,15 +473,15 @@
                 return self.backend.nplike.can_cast(
                     self.dtype, other.dtype
                 ) or self.backend.nplike.can_cast(other.dtype, self.dtype)
 
         else:
             return False
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         if len(self.shape) > 1:
             return self.to_RegularArray()._mergemany(others)
 
         head, tail = self._merging_strategy(others)
@@ -533,15 +545,15 @@
     def is_contiguous(self) -> bool:
         return self._backend.nplike.is_c_contiguous(self._data)
 
     def _subranges_equal(self, starts, stops, length, sorted=True):
         is_equal = ak.index.Index64.zeros(1, nplike=self._backend.nplike)
 
         tmp = self._backend.nplike.empty(length, dtype=self.dtype)
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_NumpyArray_fill",
                 self.dtype.type,
                 self._data.dtype.type,
             ](
                 tmp,
                 0,
@@ -560,15 +572,15 @@
 
             assert (
                 tmp_beg_ptr.nplike is self._backend.index_nplike
                 and tmp_end_ptr.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
                 and stops.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_quick_sort",
                     self.dtype.type,
                     tmp_beg_ptr.dtype.type,
                     tmp_end_ptr.dtype.type,
                     starts.dtype.type,
                     stops.dtype.type,
@@ -583,15 +595,15 @@
                     ak._util.kMaxLevels,
                 )
             )
         assert (
             starts.nplike is self._backend.index_nplike
             and stops.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_NumpyArray_subrange_equal",
                 self.dtype.type,
                 starts.dtype.type,
                 stops.dtype.type,
                 np.bool_,
             ](
@@ -612,15 +624,15 @@
         )
         out = self._backend.nplike.empty(self.shape[0], dtype=self.dtype)
 
         assert (
             offsets.nplike is self._backend.index_nplike
             and outoffsets.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_NumpyArray_sort_asstrings_uint8",
                 self.dtype.type,
                 self._data.dtype.type,
                 offsets._data.dtype.type,
                 outoffsets.dtype.type,
             ](
@@ -637,15 +649,15 @@
         outlength = ak.index.Index64.empty(1, self._backend.index_nplike)
         nextoffsets = ak.index.Index64.empty(offsets.length, self._backend.index_nplike)
         assert (
             outoffsets.nplike is self._backend.index_nplike
             and nextoffsets.nplike is self._backend.index_nplike
             and outlength.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_NumpyArray_unique_strings",
                 self.dtype.type,
                 outoffsets.dtype.type,
                 nextoffsets.dtype.type,
                 outlength.dtype.type,
             ](
@@ -675,50 +687,55 @@
                 parameters=self._parameters,
                 backend=self._backend,
             )
 
     def _is_unique(self, negaxis, starts, parents, outlength):
         if self.length == 0:
             return True
-
-        elif len(self.shape) != 1 or not self.is_contiguous:
-            contiguous_self = self.to_contiguous()
-            return contiguous_self.to_RegularArray()._is_unique(
+        elif len(self.shape) != 1:
+            return self.to_RegularArray()._is_unique(
+                negaxis,
+                starts,
+                parents,
+                outlength,
+            )
+        elif not self.is_contiguous:
+            return self.to_contiguous()._is_unique(
                 negaxis,
                 starts,
                 parents,
                 outlength,
             )
         else:
             out = self._unique(negaxis, starts, parents, outlength)
             if isinstance(out, ak.contents.ListOffsetArray):
                 return out.content.length == self.length
-
-            return out.length == self.length
+            else:
+                return out.length == self.length
 
     def _unique(self, negaxis, starts, parents, outlength):
         if self.shape[0] == 0:
             return self
 
-        if len(self.shape) == 0:
+        elif len(self.shape) == 0:
             return self
 
-        if negaxis is None:
+        elif negaxis is None:
             contiguous_self = self.to_contiguous()
 
             offsets = ak.index.Index64.zeros(2, self._backend.index_nplike)
             offsets[1] = self._data.size
             dtype = (
                 np.dtype(np.int64)
                 if self._data.dtype.kind.upper() == "M"
                 else self._data.dtype
             )
             out = self._backend.nplike.empty(self._data.size, dtype=dtype)
             assert offsets.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sort",
                     dtype.type,
                     dtype.type,
                     offsets.dtype.type,
                 ](
                     out,
@@ -730,15 +747,15 @@
                     True,
                     False,
                 )
             )
 
             nextlength = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert nextlength.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_unique",
                     out.dtype.type,
                     nextlength.dtype.type,
                 ](
                     out,
                     out.shape[0],
@@ -749,30 +766,29 @@
             return ak.contents.NumpyArray(
                 self._backend.nplike.asarray(out[: nextlength[0]], dtype=self.dtype),
                 parameters=None,
                 backend=self._backend,
             )
 
         # axis is not None
-        if len(self.shape) != 1 or not self.is_contiguous:
-            contiguous_self = self.to_contiguous()
-            return contiguous_self.to_RegularArray()._unique(
+        elif len(self.shape) != 1:
+            return self.to_RegularArray()._unique(
                 negaxis,
                 starts,
                 parents,
                 outlength,
             )
         else:
             parents_length = parents.length
             offsets_length = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 offsets_length.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges_length",
                     offsets_length.dtype.type,
                     parents.dtype.type,
                 ](
                     offsets_length.data,
                     parents.data,
@@ -783,30 +799,30 @@
             offsets = ak.index.Index64.empty(
                 offsets_length[0], self._backend.index_nplike
             )
             assert (
                 offsets.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges",
                     offsets.dtype.type,
                     parents.dtype.type,
                 ](
                     offsets.data,
                     offsets_length[0],
                     parents.data,
                     parents_length,
                 )
             )
 
             out = self._backend.nplike.empty(self.length, dtype=self.dtype)
             assert offsets.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sort",
                     out.dtype.type,
                     self._data.dtype.type,
                     offsets.dtype.type,
                 ](
                     out,
@@ -823,15 +839,15 @@
             nextoffsets = ak.index.Index64.empty(
                 offsets.length, self._backend.index_nplike
             )
             assert (
                 offsets.nplike is self._backend.index_nplike
                 and nextoffsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_unique_ranges",
                     out.dtype.type,
                     offsets.dtype.type,
                     nextoffsets.dtype.type,
                 ](
                     out,
@@ -847,15 +863,15 @@
             )
 
             assert (
                 outoffsets.nplike is self._backend.index_nplike
                 and nextoffsets.nplike is self._backend.index_nplike
                 and starts.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_unique_offsets",
                     outoffsets.dtype.type,
                     nextoffsets.dtype.type,
                     starts.dtype.type,
                 ](
                     outoffsets.data,
@@ -869,30 +885,30 @@
             return ak.contents.ListOffsetArray(
                 outoffsets, ak.contents.NumpyArray(out), parameters=self._parameters
             )
 
     def _argsort_next(
         self, negaxis, starts, shifts, parents, outlength, ascending, stable
     ):
-        if len(self.shape) == 0:
-            raise TypeError(f"{type(self).__name__} attempting to argsort a scalar ")
-        elif len(self.shape) != 1 or not self.is_contiguous:
-            contiguous_self = self.to_contiguous()
-            return contiguous_self.to_RegularArray()._argsort_next(
+        if len(self.shape) != 1:
+            return self.to_RegularArray()._argsort_next(
+                negaxis, starts, shifts, parents, outlength, ascending, stable
+            )
+        elif not self.is_contiguous:
+            return self.to_contiguous()._argsort_next(
                 negaxis, starts, shifts, parents, outlength, ascending, stable
             )
-
         else:
             parents_length = parents.length
             _offsets_length = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _offsets_length.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges_length",
                     _offsets_length.dtype.type,
                     parents.dtype.type,
                 ](
                     _offsets_length.data,
                     parents.data,
@@ -904,15 +920,15 @@
             )
 
             offsets = ak.index.Index64.empty(offsets_length, self._backend.index_nplike)
             assert (
                 offsets.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges",
                     offsets.dtype.type,
                     parents.dtype.type,
                 ](
                     offsets.data,
                     offsets_length,
@@ -927,15 +943,15 @@
                 else self._data.dtype
             )
             nextcarry = ak.index.Index64.empty(self.length, self._backend.index_nplike)
             assert (
                 nextcarry.nplike is self._backend.index_nplike
                 and offsets.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_argsort",
                     nextcarry.dtype.type,
                     dtype.type,
                     offsets.dtype.type,
                 ](
                     nextcarry.data,
@@ -952,15 +968,15 @@
                 assert (
                     nextcarry.nplike is self._backend.index_nplike
                     and shifts.nplike is self._backend.index_nplike
                     and offsets.nplike is self._backend.index_nplike
                     and parents.nplike is self._backend.index_nplike
                     and starts.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_NumpyArray_rearrange_shifted",
                         nextcarry.dtype.type,
                         shifts.dtype.type,
                         offsets.dtype.type,
                         parents.dtype.type,
                         starts.dtype.type,
@@ -976,31 +992,31 @@
                         starts.length,
                     )
                 )
             out = NumpyArray(nextcarry.data, parameters=None, backend=self._backend)
             return out
 
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
-        if len(self.shape) == 0:
-            raise TypeError(f"{type(self).__name__} attempting to sort a scalar ")
-
-        elif len(self.shape) != 1 or not self.is_contiguous:
-            contiguous_self = self.to_contiguous()
-            return contiguous_self.to_RegularArray()._sort_next(
+        if len(self.shape) != 1:
+            return self.to_RegularArray()._sort_next(
+                negaxis, starts, parents, outlength, ascending, stable
+            )
+        elif not self.is_contiguous:
+            return self.to_contiguous()._sort_next(
                 negaxis, starts, parents, outlength, ascending, stable
             )
 
         else:
             parents_length = parents.length
             _offsets_length = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _offsets_length.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges_length",
                     _offsets_length.dtype.type,
                     parents.dtype.type,
                 ](
                     _offsets_length.data,
                     parents.data,
@@ -1013,15 +1029,15 @@
 
             offsets = ak.index.Index64.empty(offsets_length, self._backend.index_nplike)
 
             assert (
                 offsets.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sorting_ranges",
                     offsets.dtype.type,
                     parents.dtype.type,
                 ](
                     offsets.data,
                     offsets_length,
@@ -1033,15 +1049,15 @@
             dtype = (
                 np.dtype(np.int64)
                 if self._data.dtype.kind.upper() == "M"
                 else self._data.dtype
             )
             out = self._backend.nplike.empty(self.length, dtype=dtype)
             assert offsets.nplike is self._backend.index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_sort",
                     dtype.type,
                     dtype.type,
                     offsets.dtype.type,
                 ](
                     out,
@@ -1108,44 +1124,42 @@
                 behavior,
             )
 
         # Yes, we've just tested these, but we need to be explicit that they are invariants
         assert self.is_contiguous
         assert self._data.ndim == 1
 
-        out = self._backend.apply_reducer(reducer, self, parents, outlength)
+        out = reducer.apply(self, parents, outlength)
 
         if reducer.needs_position:
             if shifts is None:
                 assert (
-                    out.backend is self._backend
-                    and parents.nplike is self._backend.index_nplike
+                    parents.nplike is self._backend.index_nplike
                     and starts.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_NumpyArray_reduce_adjust_starts_64",
                         out.data.dtype.type,
                         parents.dtype.type,
                         starts.dtype.type,
                     ](
                         out.data,
                         outlength,
                         parents.data,
                         starts.data,
                     )
                 )
             else:
                 assert (
-                    out.backend is self._backend
-                    and parents.nplike is self._backend.index_nplike
+                    parents.nplike is self._backend.index_nplike
                     and starts.nplike is self._backend.index_nplike
                     and shifts.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_NumpyArray_reduce_adjust_starts_shifts_64",
                         out.data.dtype.type,
                         parents.dtype.type,
                         starts.dtype.type,
                         shifts.dtype.type,
                     ](
@@ -1159,27 +1173,26 @@
 
         if mask:
             outmask = ak.index.Index8.empty(outlength, self._backend.index_nplike)
             assert (
                 outmask.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_NumpyArray_reduce_mask_ByteMaskedArray_64",
                     outmask.dtype.type,
                     parents.dtype.type,
                 ](
                     outmask.data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
-
             out = ak.contents.ByteMaskedArray(outmask, out, False, parameters=None)
 
         if keepdims:
             out = ak.contents.RegularArray(out, 1, self.length, parameters=None)
 
         return out
 
@@ -1193,16 +1206,18 @@
             if stride % self.dtype.itemsize != 0:
                 return f"at {path} ({type(self)!r}): shape[{i}] % itemsize != 0"
         return ""
 
     def _pad_none(self, target, axis, depth, clip):
         if len(self.shape) == 0:
             raise ValueError("cannot apply ak.pad_none to a scalar")
-        elif len(self.shape) > 1 or not self.is_contiguous:
+        elif len(self.shape) > 1:
             return self.to_RegularArray()._pad_none(target, axis, depth, clip)
+        elif not self.is_contiguous:
+            return self.to_contiguous()._pad_none(target, axis, depth, clip)
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 != depth:
             raise AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         if not clip:
             if target < self.length:
                 return self
             else:
@@ -1373,15 +1388,14 @@
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         if numpyarray:
             return (
                 self._backend.nplike.array_equal(self.data, other.data)
                 and self.dtype == other.dtype
-                and self.is_contiguous == other.is_contiguous
                 and self.shape == other.shape
             )
         else:
             return True
 
     def _to_regular_primitive(self) -> ak.contents.RegularArray:
         # A length-1 slice in each dimension
```

### Comparing `awkward-2.2.1/src/awkward/contents/recordarray.py` & `awkward-2.2.2/src/awkward/contents/recordarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import json
-from collections.abc import Iterable
+from collections.abc import Iterable, MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._backends.numpy import NumpyBackend
 from awkward._backends.typetracer import TypeTracerBackend
 from awkward._behavior import find_record_reducer
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.recordform import RecordForm
 from awkward.index import Index
 from awkward.record import Record
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
-def _apply_record_reducer(
-    reducer, layout: RecordArray, mask: bool, offsets: ak.index.Index, behavior
-) -> Content:
+def _apply_record_reducer(reducer, layout: Content, mask: bool, behavior) -> Content:
     # Build a 1D list over these contents
-    array = wrap_layout(ak.contents.ListOffsetArray(offsets, layout), behavior=behavior)
+    array = wrap_layout(layout, behavior=behavior)
     # Perform the reduction
     return ak.to_layout(reducer(array, mask))
 
 
 @final
 class RecordArray(Content):
     """
@@ -311,24 +310,31 @@
         return self._fields is None
 
     def to_tuple(self) -> Self:
         return RecordArray(
             self._contents, None, self._length, parameters=None, backend=self._backend
         )
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> RecordForm:
         form_key = getkey(self)
         return self.form_cls(
             [x._form_with_key(getkey) for x in self._contents],
             self._fields,
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         if self._fields is None:
             for i, content in enumerate(self._contents):
                 content._to_buffers(
                     form.content(i), getkey, container, backend, byteorder
                 )
         else:
@@ -344,26 +350,26 @@
             contents,
             self._fields,
             unknown_length if forget_length else self._length,
             parameters=self._parameters,
             backend=backend,
         )
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         if recursive:
             for x in self._contents:
                 x._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         if recursive:
             for x in self._contents:
                 x._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<RecordArray is_tuple="]
@@ -434,18 +440,14 @@
         if not (self._length is unknown_length or (0 <= where < self._length)):
             raise ak._errors.index_error(self, where)
         return Record(self, where)
 
     def _getitem_range(self, start: SupportsIndex, stop: IndexType) -> Content:
         if not self._backend.nplike.known_data:
             self._touch_shape(recursive=False)
-            return self
-
-        if self._length is unknown_length:
-            return self
 
         start, stop, _, length = self._backend.index_nplike.derive_slice_for_length(
             slice(start, stop), self._length
         )
 
         if len(self._contents) == 0:
             return RecordArray(
@@ -539,15 +541,17 @@
                 contents,
                 self._fields,
                 length,
                 parameters=self._parameters,
                 backend=self._backend,
             )
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         contents = []
         for i in range(len(self._contents)):
             contents.append(
                 self.content(i)._getitem_next_jagged(
                     slicestarts, slicestops, slicecontent, tail
                 )
             )
@@ -598,15 +602,15 @@
                 contents,
                 self._fields,
                 parameters=parameters,
                 backend=self._backend,
             )
             return next._getitem_next(nexthead, nexttail, advanced)
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
             raise ValueError(
                 "arrays of records cannot be flattened (but their contents can be; try a different 'axis')"
@@ -634,15 +638,15 @@
                     self._fields,
                     self._length,
                     parameters=None,
                     backend=self._backend,
                 ),
             )
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
@@ -670,15 +674,15 @@
 
             else:
                 return False
 
         else:
             return False
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         head, tail = self._merging_strategy(others)
 
         parameters = self._parameters
         headless = head[1:]
@@ -898,49 +902,64 @@
         if reducer_recordclass is None:
             raise TypeError(
                 "no ak.{} overloads for custom types: {}".format(
                     reducer.name, ", ".join(self.fields)
                 )
             )
         else:
-            # Convert parents into offsets
-            outoffsets = ak.index.Index64.empty(
-                outlength + 1, self._backend.index_nplike
-            )
+            # Convert parents into offsets to build a list for axis=1 reduction
+            offsets = ak.index.Index64.empty(outlength + 1, self._backend.index_nplike)
             assert (
-                outoffsets.nplike is self._backend.index_nplike
+                offsets.nplike is self._backend.index_nplike
                 and parents.nplike is self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_outoffsets_64",
-                    outoffsets.dtype.type,
+                    offsets.dtype.type,
                     parents.dtype.type,
                 ](
-                    outoffsets.data,
+                    offsets.data,
                     parents.data,
                     parents.length,
                     outlength,
                 )
             )
+            layout_to_reduce = ak.contents.ListOffsetArray(offsets, self)
 
+            # Positional reducers ultimately need to do more work when rebuilding the result
+            # so asking for a mask doesn't help us!
+            reducer_should_mask = mask and not reducer.needs_position
             out = _apply_record_reducer(
-                reducer_recordclass, self, mask, outoffsets, behavior
-            )
+                reducer_recordclass,
+                layout_to_reduce,
+                reducer_should_mask,
+                behavior,
+            )
+            if out.is_option and not reducer_should_mask:
+                reason = (
+                    "reducer is positional"
+                    if reducer.needs_position
+                    else "mask is False"
+                )
+                raise TypeError(
+                    f"a custom implementation of the reducer {reducer.name} for {self.parameter('__record__')!r} "
+                    f"returned an option when it was not expected ({reason})"
+                )
 
             if reducer.needs_position:
                 assert isinstance(out, ak.contents.NumpyArray)
 
                 if shifts is None:
                     assert (
                         out.backend is self._backend
                         and parents.nplike is self._backend.index_nplike
                         and starts.nplike is self._backend.index_nplike
                     )
-                    self._handle_error(
+                    self._backend.maybe_kernel_error(
                         self._backend[
                             "awkward_NumpyArray_reduce_adjust_starts_64",
                             out.data.dtype.type,
                             parents.dtype.type,
                             starts.dtype.type,
                         ](
                             out.data,
@@ -952,15 +971,15 @@
                 else:
                     assert (
                         out.backend is self._backend
                         and parents.nplike is self._backend.index_nplike
                         and starts.nplike is self._backend.index_nplike
                         and shifts.nplike is self._backend.index_nplike
                     )
-                    self._handle_error(
+                    self._backend.maybe_kernel_error(
                         self._backend[
                             "awkward_NumpyArray_reduce_adjust_starts_shifts_64",
                             out.data.dtype.type,
                             parents.dtype.type,
                             starts.dtype.type,
                             shifts.dtype.type,
                         ](
@@ -974,15 +993,15 @@
 
             if mask:
                 outmask = ak.index.Index8.empty(outlength, self._backend.index_nplike)
                 assert (
                     outmask.nplike is self._backend.index_nplike
                     and parents.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_NumpyArray_reduce_mask_ByteMaskedArray_64",
                         outmask.dtype.type,
                         parents.dtype.type,
                     ](
                         outmask.data,
                         parents.data,
@@ -990,18 +1009,14 @@
                         outlength,
                     )
                 )
 
                 out = ak.contents.ByteMaskedArray.simplified(
                     outmask, out, False, parameters=None
                 )
-            elif out.is_option:
-                raise TypeError(
-                    "a custom reducer function returned an option when it was not expected"
-                )
 
             if keepdims:
                 out = ak.contents.RegularArray(out, 1, self.length, parameters=None)
 
             return out
 
     def _validity_error(self, path):
```

### Comparing `awkward-2.2.1/src/awkward/contents/regulararray.py` & `awkward-2.2.2/src/awkward/contents/regulararray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.regularform import RegularForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
+    from awkward.contents.listoffsetarray import ListOffsetArray
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 @final
 class RegularArray(Content):
@@ -162,15 +165,15 @@
         elif size != 0:
             self._length = content.length // size  # floor division
         else:
             self._length = zeros_length
         self._init(parameters, content.backend)
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     @property
     def size(self):
         return self._size
 
     form_cls: Final = RegularForm
@@ -193,56 +196,63 @@
         )
 
     @classmethod
     def simplified(cls, content, size, zeros_length=0, *, parameters=None):
         return cls(content, size, zeros_length, parameters=parameters)
 
     @property
-    def offsets(self):
+    def offsets(self) -> Index:
         return self._compact_offsets64(True)
 
     @property
-    def starts(self):
+    def starts(self) -> Index:
         return self._compact_offsets64(True)[:-1]
 
     @property
     def stops(self):
         return self._compact_offsets64(True)[1:]
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> RegularForm:
         form_key = getkey(self)
         return self.form_cls(
             self._content._form_with_key(getkey),
             self._size,
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         return RegularArray(
             self._content._to_typetracer(forget_length),
             self._size,
             unknown_length if forget_length else self._length,
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<RegularArray size="]
@@ -253,15 +263,15 @@
         out.extend(self._repr_extra(indent + "    "))
         out.append("\n")
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</RegularArray>")
         out.append(post)
         return "".join(out)
 
-    def to_ListOffsetArray64(self, start_at_zero=False):
+    def to_ListOffsetArray64(self, start_at_zero: bool = False) -> ListOffsetArray:
         offsets = self._compact_offsets64(start_at_zero)
         return self._broadcast_tooffsets64(offsets)
 
     def to_RegularArray(self):
         return self
 
     def maybe_to_NumpyArray(self) -> ak.contents.NumpyArray | None:
@@ -351,15 +361,15 @@
             )
         else:
             nextcarry = ak.index.Index64.empty(
                 where.shape[0] * self._size, self._backend.index_nplike
             )
 
         assert nextcarry.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._maybe_index_error(
             self._backend[
                 "awkward_RegularArray_getitem_carry",
                 nextcarry.dtype.type,
                 where.dtype.type,
             ](
                 nextcarry.data,
                 where,
@@ -373,82 +383,88 @@
             self._content._carry(nextcarry, allow_lazy),
             self._size,
             where.shape[0],
             parameters=self._parameters,
         )
 
     def _compact_offsets64(self, start_at_zero):
-        out = ak.index.Index64.empty(
-            self._length + 1,
-            self._backend.index_nplike,
-        )
-        assert out.nplike is self._backend.index_nplike
-        self._handle_error(
-            self._backend["awkward_RegularArray_compact_offsets", out.dtype.type](
-                out.data,
-                self._length,
-                self._size,
+        index_nplike = self._backend.index_nplike
+        if self._size is not unknown_length and self._size == 0:
+            return ak.index.Index64.zeros(self._length + 1, nplike=index_nplike)
+        else:
+            return ak.index.Index64(
+                index_nplike.arange(
+                    0,
+                    index_nplike.shape_item_as_index(self._length * self._size) + 1,
+                    index_nplike.shape_item_as_index(self._size),
+                    dtype=np.int64,
+                ),
+                nplike=index_nplike,
             )
-        )
-        return out
 
-    def _broadcast_tooffsets64(self, offsets):
-        if offsets.nplike.known_data and (offsets.length == 0 or offsets[0] != 0):
+    def _broadcast_tooffsets64(self, offsets: Index) -> ListOffsetArray:
+        self._touch_data(recursive=False)
+        offsets._touch_data()
+
+        index_nplike = self._backend.index_nplike
+        assert offsets.nplike is index_nplike
+        if offsets.length is not unknown_length and offsets.length == 0:
             raise AssertionError(
-                "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
-                    "(empty)" if offsets.length == 0 else str(offsets[0])
-                )
+                "broadcast_tooffsets64 can only be used with non-empty offsets"
             )
-
-        if offsets.nplike.known_data and offsets.length - 1 != self._length:
+        elif index_nplike.known_data and offsets[0] != 0:
+            raise AssertionError(
+                f"broadcast_tooffsets64 can only be used with offsets that start at 0, not {offsets[0]}"
+            )
+        elif (
+            offsets.length is not unknown_length
+            and self._length is not unknown_length
+            and offsets.length - 1 != self._length
+        ):
             raise AssertionError(
                 "cannot broadcast RegularArray of length {} to length {}".format(
                     self._length, offsets.length - 1
                 )
             )
 
-        if self._size == 1:
-            carrylen = self._backend.index_nplike.index_as_shape_item(offsets[-1])
-            nextcarry = ak.index.Index64.empty(carrylen, self._backend.index_nplike)
+        if self._size is not unknown_length and self._size == 1:
+            count = offsets.data[1:] - offsets.data[:-1]
+            # Sanity check that our kernel isn't losing values here
             assert (
-                nextcarry.nplike is self._backend.index_nplike
-                and offsets.nplike is self._backend.index_nplike
-            )
-            self._handle_error(
-                self._backend[
-                    "awkward_RegularArray_broadcast_tooffsets_size1",
-                    nextcarry.dtype.type,
-                    offsets.dtype.type,
-                ](
-                    nextcarry.data,
-                    offsets.data,
-                    offsets.length,
-                )
-            )
-            nextcontent = self._content._carry(nextcarry, True)
-            return ak.contents.ListOffsetArray(
-                offsets, nextcontent, parameters=self._parameters
+                not self._backend.index_nplike.known_data
+                or count.size is unknown_length
+                or count.size == 0
+                or count.dtype == np.intp
+                or self._backend.index_nplike.max(count) <= np.iinfo(np.intp).max
+            )
+            carry = ak.index.Index64(
+                index_nplike.repeat(
+                    index_nplike.arange(
+                        index_nplike.shape_item_as_index(self._length), dtype=np.int64
+                    ),
+                    index_nplike.astype(count, np.intp),
+                ),
+                nplike=index_nplike,
             )
-
+            next_content = self._content._carry(carry, True)
         else:
-            assert offsets.nplike is self._backend.index_nplike
-            self._handle_error(
-                self._backend[
-                    "awkward_RegularArray_broadcast_tooffsets", offsets.dtype.type
-                ](
-                    offsets.data,
-                    offsets.length,
-                    self._size,
-                )
-            )
-            return ak.contents.ListOffsetArray(
-                offsets, self._content, parameters=self._parameters
-            )
+            this_offsets = self._compact_offsets64(True)
+            if index_nplike.known_data and not index_nplike.array_equal(
+                offsets.data, this_offsets.data
+            ):
+                raise ValueError("cannot broadcast nested list")
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+            next_content = self._content[: offsets[-1]]
+        return ak.contents.ListOffsetArray(
+            offsets, next_content, parameters=self._parameters
+        )
+
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         out = self.to_ListOffsetArray64(True)
         return out._getitem_next_jagged(slicestarts, slicestops, slicecontent, tail)
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
         tail: tuple[SliceItem, ...],
@@ -459,15 +475,15 @@
         if head is NO_HEAD:
             return self
 
         elif is_integer_like(head):
             nexthead, nexttail = ak._slicing.head_tail(tail)
             nextcarry = ak.index.Index64.empty(self._length, index_nplike)
             assert nextcarry.nplike is index_nplike
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_RegularArray_getitem_next_at", nextcarry.dtype.type
                 ](
                     nextcarry.data,
                     head,
                     self._length,
                     self._size,
@@ -481,15 +497,15 @@
             nexthead, nexttail = ak._slicing.head_tail(tail)
             start, stop, step, nextsize = index_nplike.derive_slice_for_length(
                 head, length=self._size
             )
 
             nextcarry = ak.index.Index64.empty(self._length * nextsize, index_nplike)
             assert nextcarry.nplike is index_nplike
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_RegularArray_getitem_next_range",
                     nextcarry.dtype.type,
                 ](
                     nextcarry.data,
                     start,
                     step,
@@ -514,15 +530,15 @@
             else:
                 nextadvanced = ak.index.Index64.empty(nextcarry.length, index_nplike)
                 advanced = advanced.to_nplike(index_nplike)
                 assert (
                     nextadvanced.nplike is index_nplike
                     and advanced.nplike is index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_RegularArray_getitem_next_range_spreadadvanced",
                         nextadvanced.dtype.type,
                         advanced.dtype.type,
                     ](
                         nextadvanced.data,
                         advanced.data,
@@ -551,15 +567,15 @@
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.index.Index64):
             head = head.to_nplike(index_nplike)
             flathead = index_nplike.reshape(index_nplike.asarray(head.data), (-1,))
             regular_flathead = ak.index.Index64.empty(flathead.shape[0], index_nplike)
             assert regular_flathead.nplike is index_nplike
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_RegularArray_getitem_next_array_regularize",
                     regular_flathead.dtype.type,
                     flathead.dtype.type,
                 ](
                     regular_flathead.data,
                     flathead,
@@ -579,15 +595,15 @@
                 )
                 nextadvanced = ak.index.Index64.empty(nextcarry.length, index_nplike)
                 assert (
                     nextcarry.nplike is index_nplike
                     and nextadvanced.nplike is index_nplike
                     and regular_flathead.nplike is index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_RegularArray_getitem_next_array",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         regular_flathead.dtype.type,
                     ](
                         nextcarry.data,
@@ -621,15 +637,15 @@
                 advanced = advanced.to_nplike(index_nplike)
                 assert (
                     nextcarry.nplike is index_nplike
                     and nextadvanced.nplike is index_nplike
                     and advanced.nplike is index_nplike
                     and regular_flathead.nplike is index_nplike
                 )
-                self._handle_error(
+                self._maybe_index_error(
                     self._backend[
                         "awkward_RegularArray_getitem_next_array_advanced",
                         nextcarry.dtype.type,
                         nextadvanced.dtype.type,
                         advanced.dtype.type,
                         regular_flathead.dtype.type,
                     ](
@@ -670,15 +686,15 @@
                 head.length * self._length, index_nplike
             )
             multistops = ak.index.Index64.empty(
                 head.length * self._length, index_nplike
             )
 
             assert head.offsets.nplike is index_nplike
-            self._handle_error(
+            self._maybe_index_error(
                 self._backend[
                     "awkward_RegularArray_getitem_jagged_expand",
                     multistarts.dtype.type,
                     multistops.dtype.type,
                     head.offsets.dtype.type,
                 ](
                     multistarts.data,
@@ -699,18 +715,18 @@
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         return self.to_ListOffsetArray64(True)._offsets_and_flattened(axis, depth)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
@@ -726,15 +742,15 @@
         ):
             return self._content._mergeable_next(other.content, mergebool)
         elif isinstance(other, ak.contents.NumpyArray) and len(other.shape) > 1:
             return self._mergeable_next(other._to_regular_primitive(), mergebool)
         else:
             return False
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         if any(x.is_option for x in others):
             return ak.contents.UnmaskedArray(self)._mergemany(others)
 
         # Regularize NumpyArray into RegularArray (or NumpyArray if 1D)
@@ -774,15 +790,15 @@
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._local_index_axis0()
         elif posaxis is not None and posaxis + 1 == depth + 1:
             localindex = ak.index.Index64.empty(
                 self._length * self._size, nplike=self._backend.index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend["awkward_RegularArray_localindex", np.int64](
                     localindex.data,
                     self._size,
                     self._length,
                 )
             )
             return ak.contents.RegularArray(
@@ -918,15 +934,15 @@
             toindex = ak.index.Index64.empty(n, index_nplike, dtype=np.int64)
             fromindex = ak.index.Index64.empty(n, index_nplike, dtype=np.int64)
 
             if self._size != 0:
                 assert (
                     toindex.nplike is index_nplike and fromindex.nplike is index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_RegularArray_combinations_64",
                         np.int64,
                         toindex.data.dtype.type,
                         fromindex.data.dtype.type,
                     ](
                         tocarryraw,
@@ -976,45 +992,54 @@
         keepdims,
         behavior,
     ):
         index_nplike = self._backend.index_nplike
         branch, depth = self.branch_depth
         nextlen = self._length * self._size
         if not branch and negaxis == depth:
-            if self._size == 0:
-                nextstarts = ak.index.Index64(
-                    index_nplike.zeros(self._length, dtype=np.int64),
-                    nplike=index_nplike,
-                )
-            else:
-                nextstarts = ak.index.Index64(
-                    index_nplike.arange(0, nextlen, self._size),
-                    nplike=index_nplike,
-                )
-            assert nextstarts.length == self._length
-
             nextcarry = ak.index.Index64.empty(nextlen, nplike=index_nplike)
             nextparents = ak.index.Index64.empty(nextlen, nplike=index_nplike)
             assert (
                 parents.nplike is index_nplike
                 and nextcarry.nplike is index_nplike
                 and nextparents.nplike is index_nplike
             )
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_RegularArray_reduce_nonlocal_preparenext",
                     nextcarry.dtype.type,
                     nextparents.dtype.type,
                     parents.dtype.type,
                 ](
                     nextcarry.data,
                     nextparents.data,
                     parents.data,
                     self._size,
-                    len(self),
+                    self._length,
+                )
+            )
+            nextstarts = ak.index.Index64.empty(
+                # `starts` must have at least enough elements for the largest `nextparent` to index into
+                # The upper bound for this value is given by `nextlen` (each item in this list belonging
+                # to a distinct reduction), but the length of `starts` should equate to `maxnextparents - 1`.
+                starts.length * self._size,
+                nplike=index_nplike,
+            )
+            assert (
+                nextstarts.nplike is index_nplike and nextparents.nplike is index_nplike
+            )
+            self._backend.maybe_kernel_error(
+                self._backend[
+                    "awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64",
+                    nextstarts.dtype.type,
+                    nextparents.dtype.type,
+                ](
+                    nextstarts.data,
+                    nextparents.data,
+                    nextlen,
                 )
             )
 
             if reducer.needs_position:
                 # Regular arrays have the same length rows, so there can be no "missing" values
                 # unlike ragged list types
                 nextshifts = ak.index.Index64.zeros(
@@ -1045,15 +1070,15 @@
             if keepdims:
                 out = ak.contents.RegularArray(out, 1, self._length, parameters=None)
             return out
         else:
             nextparents = ak.index.Index64.empty(nextlen, index_nplike)
 
             assert nextparents.nplike is index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_RegularArray_reduce_local_nextparents",
                     nextparents.dtype.type,
                 ](
                     nextparents.data,
                     self._size,
                     self._length,
@@ -1134,15 +1159,15 @@
                         zeros_length=self._length,
                     )
                 else:
                     assert outcontent.is_regular
 
             outoffsets = ak.index.Index64.empty(outlength + 1, index_nplike)
             assert outoffsets.nplike is index_nplike and parents.nplike is index_nplike
-            self._handle_error(
+            self._backend.maybe_kernel_error(
                 self._backend[
                     "awkward_ListOffsetArray_reduce_local_outoffsets_64",
                     outoffsets.dtype.type,
                     parents.dtype.type,
                 ](
                     outoffsets.data,
                     parents.data,
@@ -1176,15 +1201,15 @@
 
             else:
                 index = ak.index.Index64.empty(
                     self._length * target,
                     self._backend.index_nplike,
                 )
                 assert index.nplike is self._backend.index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_RegularArray_rpad_and_clip_axis1", index.dtype.type
                     ](index.data, target, self._size, self._length)
                 )
                 next = ak.contents.IndexedOptionArray.simplified(
                     index, self._content, parameters=self._parameters
                 )
@@ -1301,15 +1326,15 @@
                 return [
                     RegularArray(c, size=c.length, parameters=self._parameters)
                     for c in contents
                 ]
             else:
                 return contents
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.to_ListOffsetArray64()._drop_none()
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if options["regular_to_jagged"]:
             return self.to_ListOffsetArray64(False)._recursively_apply(
@@ -1436,9 +1461,9 @@
         content = self._content.to_backend(backend)
         return RegularArray(
             content, self._size, zeros_length=self._length, parameters=self._parameters
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return self._size == other.size and self._content.is_equal_to(
-            self._content, index_dtype, numpyarray
+            other._content, index_dtype, numpyarray
         )
```

### Comparing `awkward-2.2.1/src/awkward/contents/unionarray.py` & `awkward-2.2.2/src/awkward/contents/unionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 # pylint: disable=consider-using-enumerate
 from __future__ import annotations
 
 import copy
 import ctypes
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable, MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.unionform import UnionForm
 from awkward.index import Index, Index8, Index64
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
@@ -263,15 +264,15 @@
                 for j, inner_cont in enumerate(innercontents):
                     unmerged = True
 
                     # For each "final" outer union content
                     for k in range(len(contents)):
                         # Try and merge inner union content with running outer-union contentca
                         if merge and contents[k]._mergeable_next(inner_cont, mergebool):
-                            Content._selfless_handle_error(
+                            backend.maybe_kernel_error(
                                 backend[
                                     "awkward_UnionArray_simplify",
                                     tags.dtype.type,
                                     index.dtype.type,
                                     self_tags.dtype.type,
                                     self_index.dtype.type,
                                     innertags.dtype.type,
@@ -292,15 +293,15 @@
                             )
                             contents[k] = contents[k]._mergemany([inner_cont])
                             unmerged = False
                             break
 
                     # Did we fail to merge any of the final outer contents with this inner union content?
                     if unmerged:
-                        Content._selfless_handle_error(
+                        backend.maybe_kernel_error(
                             backend[
                                 "awkward_UnionArray_simplify",
                                 tags.dtype.type,
                                 index.dtype.type,
                                 self_tags.dtype.type,
                                 self_index.dtype.type,
                                 innertags.dtype.type,
@@ -321,15 +322,15 @@
                         )
                         contents.append(inner_cont)
 
             else:
                 unmerged = True
                 for k in range(len(contents)):
                     if contents[k] is self_cont:
-                        Content._selfless_handle_error(
+                        backend.maybe_kernel_error(
                             backend[
                                 "awkward_UnionArray_simplify_one",
                                 tags.dtype.type,
                                 index.dtype.type,
                                 self_tags.dtype.type,
                                 self_index.dtype.type,
                             ](
@@ -343,15 +344,15 @@
                                 0,
                             )
                         )
                         unmerged = False
                         break
 
                     elif merge and contents[k]._mergeable_next(self_cont, mergebool):
-                        Content._selfless_handle_error(
+                        backend.maybe_kernel_error(
                             backend[
                                 "awkward_UnionArray_simplify_one",
                                 tags.dtype.type,
                                 index.dtype.type,
                                 self_tags.dtype.type,
                                 self_index.dtype.type,
                             ](
@@ -366,15 +367,15 @@
                             )
                         )
                         contents[k] = contents[k]._mergemany([self_cont])
                         unmerged = False
                         break
 
                 if unmerged:
-                    Content._selfless_handle_error(
+                    backend.maybe_kernel_error(
                         backend[
                             "awkward_UnionArray_simplify_one",
                             tags.dtype.type,
                             index.dtype.type,
                             self_tags.dtype.type,
                             self_index.dtype.type,
                         ](
@@ -417,25 +418,32 @@
                 contents,
                 parameters=parameters,
             )
 
     def content(self, index):
         return self._contents[index]
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> UnionForm:
         form_key = getkey(self)
         return self.form_cls(
             self._tags.form,
             self._index.form,
             [x._form_with_key(getkey) for x in self._contents],
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         key1 = getkey(self, form, "tags")
         key2 = getkey(self, form, "index")
         container[key1] = ak._util.native_to_byteorder(
             self._tags.raw(backend.index_nplike), byteorder
         )
         container[key2] = ak._util.native_to_byteorder(
@@ -450,32 +458,30 @@
         return UnionArray(
             tags.forget_length() if forget_length else tags,
             self._index.to_nplike(tt),
             [x._to_typetracer(False) for x in self._contents],
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._tags.data.touch_data()
-            self._index.data.touch_data()
+    def _touch_data(self, recursive: bool):
+        self._tags._touch_data()
+        self._index._touch_data()
         if recursive:
             for x in self._contents:
                 x._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
-        if not self._backend.index_nplike.known_data:
-            self._tags.data.touch_shape()
-            self._index.data.touch_shape()
+    def _touch_shape(self, recursive: bool):
+        self._tags._touch_shape()
+        self._index._touch_shape()
         if recursive:
             for x in self._contents:
                 x._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._tags.length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<UnionArray len="]
@@ -643,15 +649,15 @@
         tmpcarry = ak.index.Index64.empty(lentags, self._backend.index_nplike)
         assert (
             lenout.nplike is self._backend.index_nplike
             and tmpcarry.nplike is self._backend.index_nplike
             and self._tags.nplike is self._backend.index_nplike
             and self._index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_UnionArray_project",
                 lenout.dtype.type,
                 tmpcarry.dtype.type,
                 self._tags.dtype.type,
                 self._index.dtype.type,
             ](
@@ -678,15 +684,15 @@
         tags = tags.to_nplike(backend.index_nplike)
 
         lentags = tags.length
         _size = ak.index.Index64.empty(1, nplike=backend.index_nplike)
         assert (
             _size.nplike is backend.index_nplike and tags.nplike is backend.index_nplike
         )
-        Content._selfless_handle_error(
+        backend.maybe_kernel_error(
             backend[
                 "awkward_UnionArray_regular_index_getsize",
                 _size.dtype.type,
                 tags.dtype.type,
             ](
                 _size.data,
                 tags.data,
@@ -697,15 +703,15 @@
         current = index_cls.empty(size, nplike=backend.index_nplike)
         outindex = index_cls.empty(lentags, nplike=backend.index_nplike)
         assert (
             outindex.nplike is backend.index_nplike
             and current.nplike is backend.index_nplike
             and tags.nplike is backend.index_nplike
         )
-        Content._selfless_handle_error(
+        backend.maybe_kernel_error(
             backend[
                 "awkward_UnionArray_regular_index",
                 outindex.dtype.type,
                 current.dtype.type,
                 tags.dtype.type,
             ](
                 outindex.data,
@@ -747,15 +753,15 @@
         for tag, count in enumerate(counts):
             assert (
                 tags.nplike is index_nplike
                 and index.nplike is index_nplike
                 and f_offsets.nplike is index_nplike
                 and count.nplike is index_nplike
             )
-            Content._selfless_handle_error(
+            backend.maybe_kernel_error(
                 backend[
                     "awkward_UnionArray_nestedfill_tags_index",
                     tags.dtype.type,
                     index.dtype.type,
                     f_offsets.dtype.type,
                     count.dtype.type,
                 ](
@@ -776,15 +782,17 @@
                 ak.contents.ListArray(
                     slicestarts, slicestops, slicecontent, parameters=None
                 ),
                 "cannot apply jagged slices to irreducible union arrays",
             )
         return self._getitem_next_jagged(slicestarts, slicestops, slicecontent, tail)
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return self._getitem_next_jagged_generic(
             slicestarts, slicestops, slicecontent, tail
         )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
@@ -824,15 +832,15 @@
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
             raise AssertionError(repr(head))
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
 
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
 
         else:
             has_offsets = False
@@ -854,15 +862,15 @@
                     1, nplike=self._backend.index_nplike
                 )
                 assert (
                     total_length.nplike is self._backend.index_nplike
                     and self._tags.nplike is self._backend.index_nplike
                     and self._index.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_flatten_length",
                         total_length.dtype.type,
                         self._tags.dtype.type,
                         self._index.dtype.type,
                         np.int64,
                     ](
@@ -889,15 +897,15 @@
                 assert (
                     totags.nplike is self._backend.index_nplike
                     and toindex.nplike is self._backend.index_nplike
                     and tooffsets.nplike is self._backend.index_nplike
                     and self._tags.nplike is self._backend.index_nplike
                     and self._index.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_flatten_combine",
                         totags.dtype.type,
                         toindex.dtype.type,
                         tooffsets.dtype.type,
                         self._tags.dtype.type,
                         self._index.dtype.type,
@@ -937,15 +945,15 @@
                         self._tags,
                         self._index,
                         contents,
                         parameters=self._parameters,
                     ),
                 )
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         return True
 
     def _merging_strategy(self, others):
         if len(others) == 0:
             raise ValueError(
                 "to merge this array with 'others', at least one other must be provided"
             )
@@ -981,37 +989,37 @@
             nplike=self._backend.index_nplike,
         )
 
         contents = [other]
         contents.extend(self.contents)
 
         assert tags.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend["awkward_UnionArray_filltags_const", tags.dtype.type](
                 tags.data,
                 0,
                 theirlength,
                 0,
             )
         )
 
         assert index.nplike is self._backend.index_nplike
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend["awkward_UnionArray_fillindex_count", index.dtype.type](
                 index.data,
                 0,
                 theirlength,
             )
         )
 
         assert (
             tags.nplike is self._backend.index_nplike
             and self.tags.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_UnionArray_filltags",
                 tags.dtype.type,
                 self.tags.dtype.type,
             ](
                 tags.data,
                 theirlength,
@@ -1021,15 +1029,15 @@
             )
         )
 
         assert (
             index.nplike is self._backend.index_nplike
             and self.index.nplike is self._backend.index_nplike
         )
-        self._handle_error(
+        self._backend.maybe_kernel_error(
             self._backend[
                 "awkward_UnionArray_fillindex",
                 index.dtype.type,
                 self.index.dtype.type,
             ](
                 index.data,
                 theirlength,
@@ -1041,15 +1049,15 @@
         if len(contents) > 2**7:
             raise AssertionError("FIXME: handle UnionArray with more than 127 contents")
 
         return ak.contents.UnionArray.simplified(
             tags, index, contents, parameters=self._parameters
         )
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         head, tail = self._merging_strategy(others)
 
         total_length = 0
         for array in head:
@@ -1075,15 +1083,15 @@
                 union_tags = array.tags
                 union_index = array.index
                 union_contents = array.contents
                 assert (
                     nexttags.nplike is self._backend.index_nplike
                     and union_tags.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_filltags",
                         nexttags.dtype.type,
                         union_tags.dtype.type,
                     ](
                         nexttags.data,
                         length_so_far,
@@ -1092,15 +1100,15 @@
                         len(nextcontents),
                     )
                 )
                 assert (
                     nextindex.nplike is self._backend.index_nplike
                     and union_index.nplike is self._backend.index_nplike
                 )
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_fillindex",
                         nextindex.dtype.type,
                         union_index.dtype.type,
                     ](
                         nextindex.data,
                         length_so_far,
@@ -1110,28 +1118,28 @@
                 )
                 length_so_far += array.length
 
                 nextcontents.extend(union_contents)
 
             else:
                 assert nexttags.nplike is self._backend.index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_filltags_const",
                         nexttags.dtype.type,
                     ](
                         nexttags.data,
                         length_so_far,
                         array.length,
                         len(nextcontents),
                     )
                 )
 
                 assert nextindex.nplike is self._backend.index_nplike
-                self._handle_error(
+                self._backend.maybe_kernel_error(
                     self._backend[
                         "awkward_UnionArray_fillindex_count", nextindex.dtype.type
                     ](nextindex.data, length_so_far, array.length)
                 )
 
                 length_so_far += array.length
```

### Comparing `awkward-2.2.1/src/awkward/contents/unmaskedarray.py` & `awkward-2.2.2/src/awkward/contents/unmaskedarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import math
+from collections.abc import MutableMapping, Sequence
 
 import awkward as ak
 from awkward._backends.backend import Backend
 from awkward._errors import AxisError
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyMetadata
+from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
+from awkward._nplikes.shape import ShapeItem
 from awkward._nplikes.typetracer import MaybeNone
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
     type_parameters_equal,
 )
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
-from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
+from awkward._typing import TYPE_CHECKING, Callable, Final, Self, SupportsIndex, final
 from awkward._util import UNSET
 from awkward.contents.content import Content
+from awkward.forms.form import Form
 from awkward.forms.unmaskedform import UnmaskedForm
 from awkward.index import Index
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
+    from awkward.contents import IndexedOptionArray
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 @final
 class UnmaskedArray(Content):
@@ -80,15 +84,15 @@
                     type(self).__name__, type(content).__name__
                 )
             )
         self._content = content
         self._init(parameters, content.backend)
 
     @property
-    def content(self):
+    def content(self) -> Content:
         return self._content
 
     form_cls: Final = UnmaskedForm
 
     def copy(self, content=UNSET, *, parameters=UNSET):
         return UnmaskedArray(
             self._content if content is UNSET else content,
@@ -114,42 +118,49 @@
         elif content.is_indexed or content.is_option:
             return content.copy(
                 parameters=parameters_union(content._parameters, parameters)
             )
         else:
             return cls(content, parameters=parameters)
 
-    def _form_with_key(self, getkey):
+    def _form_with_key(self, getkey: Callable[[Content], str | None]) -> UnmaskedForm:
         form_key = getkey(self)
         return self.form_cls(
             self._content._form_with_key(getkey),
             parameters=self._parameters,
             form_key=form_key,
         )
 
-    def _to_buffers(self, form, getkey, container, backend, byteorder):
+    def _to_buffers(
+        self,
+        form: Form,
+        getkey: Callable[[Content, Form, str], str],
+        container: MutableMapping[str, ArrayLike],
+        backend: Backend,
+        byteorder: str,
+    ):
         assert isinstance(form, self.form_cls)
         self._content._to_buffers(form.content, getkey, container, backend, byteorder)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         return UnmaskedArray(
             self._content._to_typetracer(forget_length),
             parameters=self._parameters,
         )
 
-    def _touch_data(self, recursive):
+    def _touch_data(self, recursive: bool):
         if recursive:
             self._content._touch_data(recursive)
 
-    def _touch_shape(self, recursive):
+    def _touch_shape(self, recursive: bool):
         if recursive:
             self._content._touch_shape(recursive)
 
     @property
-    def length(self):
+    def length(self) -> ShapeItem:
         return self._content.length
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<UnmaskedArray len="]
@@ -158,15 +169,15 @@
         out.extend(self._repr_extra(indent + "    "))
         out.append("\n")
         out.append(self._content._repr(indent + "    ", "<content>", "</content>\n"))
         out.append(indent + "</UnmaskedArray>")
         out.append(post)
         return "".join(out)
 
-    def to_IndexedOptionArray64(self):
+    def to_IndexedOptionArray64(self) -> IndexedOptionArray:
         arange = self._backend.index_nplike.arange(self._content.length, dtype=np.int64)
         return ak.contents.IndexedOptionArray(
             ak.index.Index64(arange, nplike=self._backend.index_nplike),
             self._content,
             parameters=self._parameters,
         )
 
@@ -242,15 +253,17 @@
         )
 
     def _carry(self, carry: Index, allow_lazy: bool) -> Content:
         return UnmaskedArray.simplified(
             self._content._carry(carry, allow_lazy), parameters=self._parameters
         )
 
-    def _getitem_next_jagged(self, slicestarts, slicestops, slicecontent, tail):
+    def _getitem_next_jagged(
+        self, slicestarts: Index, slicestops: Index, slicecontent: Content, tail
+    ) -> Content:
         return UnmaskedArray(
             self._content._getitem_next_jagged(
                 slicestarts, slicestops, slicecontent, tail
             ),
             parameters=self._parameters,
         )
 
@@ -293,45 +306,45 @@
         if mask is not None:
             return ak.contents.ByteMaskedArray(
                 mask, self._content, False, parameters=self._parameters
             ).project()
         else:
             return self._content
 
-    def _offsets_and_flattened(self, axis, depth):
+    def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             raise AxisError("axis=0 not allowed for flatten")
         else:
             offsets, flattened = self._content._offsets_and_flattened(axis, depth)
             if offsets.length == 0:
                 return (
                     offsets,
                     UnmaskedArray(flattened, parameters=self._parameters),
                 )
 
             else:
                 return (offsets, flattened)
 
-    def _mergeable_next(self, other, mergebool):
+    def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(
                 other.content, mergebool
             ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
-    def _mergemany(self, others):
+    def _mergemany(self, others: Sequence[Content]) -> Content:
         if len(others) == 0:
             return self
 
         if all(isinstance(x, UnmaskedArray) for x in others):
             parameters = self._parameters
             tail_contents = []
             for x in others:
@@ -473,15 +486,15 @@
     def _remove_structure(self, backend, options):
         branch, depth = self.branch_depth
         if branch or options["drop_nones"] or depth > 1:
             return self.project()._remove_structure(backend, options)
         else:
             return [self]
 
-    def _drop_none(self):
+    def _drop_none(self) -> Content:
         return self.to_ByteMaskedArray(True)._drop_none()
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if options["return_array"]:
             if options["return_simplified"]:
```

### Comparing `awkward-2.2.1/src/awkward/forms/__init__.py` & `awkward-2.2.2/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/bitmaskedform.py` & `awkward-2.2.2/src/awkward/forms/bitmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/bytemaskedform.py` & `awkward-2.2.2/src/awkward/forms/bytemaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/emptyform.py` & `awkward-2.2.2/src/awkward/forms/emptyform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward as ak
 from awkward._errors import deprecate
-from awkward._typing import final
+from awkward._nplikes.shape import ShapeItem
+from awkward._typing import Iterator, final
 from awkward._util import UNSET
 from awkward.forms.form import Form, JSONMapping
 
 
 @final
 class EmptyForm(Form):
     is_numpy = True
@@ -99,7 +100,10 @@
     def _select_columns(self, index, specifier, matches, output):
         if any(match and index >= len(item) for item, match in zip(specifier, matches)):
             output.append(None)
         return self
 
     def _column_types(self) -> tuple[str, ...]:
         return ("empty",)
+
+    def _length_one_buffer_lengths(self) -> Iterator[ShapeItem]:
+        yield 0
```

### Comparing `awkward-2.2.1/src/awkward/forms/form.py` & `awkward-2.2.2/src/awkward/forms/form.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 from collections.abc import Mapping
 
 import awkward as ak
 from awkward._backends.numpy import NumpyBackend
 from awkward._errors import deprecate
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward._nplikes.shape import unknown_length
+from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._parameters import parameters_union
 from awkward._typing import Final, JSONMapping, JSONSerializable
 
 np = NumpyMetadata.instance()
 numpy_backend = NumpyBackend.instance()
 
 
@@ -449,26 +449,106 @@
             byteorder=ak._util.native_byteorder,
             highlevel=highlevel,
             behavior=behavior,
             simplify=False,
         )
 
     def length_one_array(self, *, backend=numpy_backend, highlevel=True, behavior=None):
-        # A length-1 array will need at least N bytes, where N is the largest dtype (e.g. 256 bit complex)
-        # Similarly, a length-1 array will need no more than 2*N bytes, as all contents need at most two
-        # index-types e.g. `ListOffsetArray.offsets` for their various index metadata. Therefore, we
-        # create a buffer of this length (2N) and instruct all contents to use it (via `buffer_key=""`).
-        # At the same time, with all index-like metadata set to 0, the list types will have zero lengths
-        # whilst unions, indexed, and option types will contain a single value.
+        # The naive implementation of a length-1 array requires that we have a sufficiently
+        # large buffer to be able to build _any_ subtree.
+        def max_prefer_unknown(this: ShapeItem, that: ShapeItem) -> ShapeItem:
+            if this is unknown_length:
+                return this
+            if that is unknown_length:
+                return that
+            return max(this, that)
+
+        container = {}
+
+        def prepare(form, multiplier):
+            form_key = f"node-{len(container)}"
+
+            if isinstance(form, (ak.forms.BitMaskedForm, ak.forms.ByteMaskedForm)):
+                if form.valid_when:
+                    container[form_key] = b"\x00" * multiplier
+                else:
+                    container[form_key] = b"\xff" * multiplier
+                return form.copy(form_key=form_key)  # DO NOT RECURSE
+
+            elif isinstance(form, ak.forms.IndexedOptionForm):
+                container[form_key] = b"\xff\xff\xff\xff\xff\xff\xff\xff"  # -1
+                return form.copy(form_key=form_key)  # DO NOT RECURSE
+
+            elif isinstance(form, ak.forms.EmptyForm):
+                # no error if protected by non-recursing node type
+                raise TypeError(
+                    "cannot generate a length_one_array from a Form with an "
+                    "unknowntype that cannot be hidden (EmptyForm not within "
+                    "BitMaskedForm, ByteMaskedForm, or IndexedOptionForm)"
+                )
+
+            elif isinstance(form, ak.forms.UnmaskedForm):
+                return form.copy(content=prepare(form.content, multiplier))
+
+            elif isinstance(form, (ak.forms.IndexedForm, ak.forms.ListForm)):
+                container[form_key] = b"\x00" * (8 * multiplier)
+                return form.copy(
+                    content=prepare(form.content, multiplier), form_key=form_key
+                )
+
+            elif isinstance(form, ak.forms.ListOffsetForm):
+                # offsets length == array length + 1
+                container[form_key] = b"\x00" * (8 * (multiplier + 1))
+                return form.copy(
+                    content=prepare(form.content, multiplier), form_key=form_key
+                )
+
+            elif isinstance(form, ak.forms.RegularForm):
+                size = form.size
+
+                # https://github.com/scikit-hep/awkward/pull/2499#discussion_r1220503454
+                if size is unknown_length:
+                    size = 1
+
+                return form.copy(content=prepare(form.content, multiplier * size))
+
+            elif isinstance(form, ak.forms.NumpyForm):
+                dtype = ak.types.numpytype.primitive_to_dtype(form._primitive)
+                size = multiplier * dtype.itemsize
+                for x in form.inner_shape:
+                    if x is not unknown_length:
+                        size *= x
+
+                container[form_key] = b"\x00" * size
+                return form.copy(form_key=form_key)
+
+            elif isinstance(form, ak.forms.RecordForm):
+                return form.copy(
+                    # recurse down all contents
+                    contents=[prepare(x, multiplier) for x in form.contents]
+                )
+
+            elif isinstance(form, ak.forms.UnionForm):
+                # both tags and index will get this buffer, but index is 8 bytes
+                container[form_key] = b"\x00" * (8 * multiplier)
+                return form.copy(
+                    # only recurse down contents[0] because all index == 0
+                    contents=(
+                        [prepare(form.contents[0], multiplier)] + form.contents[1:]
+                    ),
+                    form_key=form_key,
+                )
+
+            else:
+                raise AssertionError(f"not a Form: {form!r}")
+
         return ak.operations.ak_from_buffers._impl(
-            form=self,
+            form=prepare(self, 1),
             length=1,
-            container={
-                "": b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
-            },
-            buffer_key="",
+            container=container,
+            buffer_key="{form_key}",
             backend=backend,
             byteorder=ak._util.native_byteorder,
             highlevel=highlevel,
             behavior=behavior,
             simplify=False,
         )
```

### Comparing `awkward-2.2.1/src/awkward/forms/indexedform.py` & `awkward-2.2.2/src/awkward/forms/indexedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/indexedoptionform.py` & `awkward-2.2.2/src/awkward/forms/indexedoptionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/listform.py` & `awkward-2.2.2/src/awkward/forms/listform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/listoffsetform.py` & `awkward-2.2.2/src/awkward/forms/listoffsetform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+from __future__ import annotations
+
 import awkward as ak
 from awkward._parameters import type_parameters_equal
-from awkward._typing import final
+from awkward._typing import JSONMapping, final
 from awkward._util import UNSET
 from awkward.forms.form import Form
 
 
 @final
 class ListOffsetForm(Form):
     is_list = True
 
-    def __init__(self, offsets, content, *, parameters=None, form_key=None):
+    def __init__(
+        self,
+        offsets: str,
+        content: Form,
+        *,
+        parameters: JSONMapping | None = None,
+        form_key: str | None = None,
+    ):
         if not isinstance(offsets, str):
             raise TypeError(
                 "{} 'offsets' must be of type str, not {}".format(
                     type(self).__name__, repr(offsets)
                 )
             )
```

### Comparing `awkward-2.2.1/src/awkward/forms/numpyform.py` & `awkward-2.2.2/src/awkward/forms/numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/recordform.py` & `awkward-2.2.2/src/awkward/forms/recordform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/regularform.py` & `awkward-2.2.2/src/awkward/forms/regularform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/unionform.py` & `awkward-2.2.2/src/awkward/forms/unionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/forms/unmaskedform.py` & `awkward-2.2.2/src/awkward/forms/unmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/__init__.py` & `awkward-2.2.2/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_all.py` & `awkward-2.2.2/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_almost_equal.py` & `awkward-2.2.2/src/awkward/operations/ak_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_any.py` & `awkward-2.2.2/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_argcartesian.py` & `awkward-2.2.2/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_argcombinations.py` & `awkward-2.2.2/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_argmax.py` & `awkward-2.2.2/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_argmin.py` & `awkward-2.2.2/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_argsort.py` & `awkward-2.2.2/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_backend.py` & `awkward-2.2.2/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.2.2/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.2.2/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_cartesian.py` & `awkward-2.2.2/src/awkward/operations/ak_cartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_categories.py` & `awkward-2.2.2/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_combinations.py` & `awkward-2.2.2/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_concatenate.py` & `awkward-2.2.2/src/awkward/operations/ak_concatenate.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 __all__ = ("concatenate",)
 import awkward as ak
 from awkward._backends.dispatch import backend_of
 from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward._regularize import is_integer, regularize_axis
+from awkward._nplikes.shape import unknown_length
+from awkward._regularize import regularize_axis
 from awkward._typing import Sequence
 from awkward.contents import Content
 from awkward.operations.ak_fill_none import fill_none
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
@@ -128,42 +129,55 @@
                 parameters=out._parameters,
                 mergebool=mergebool,
             )
 
     else:
 
         def action(inputs, depth, **kwargs):
-            if depth == posaxis and any(
-                isinstance(x, ak.contents.Content) and x.is_option for x in inputs
+            if any(
+                x.minmax_depth == (1, 1)
+                for x in inputs
+                if isinstance(x, ak.contents.Content)
             ):
+                raise ValueError(
+                    "at least one array is not deep enough to concatenate at "
+                    "axis={}".format(axis)
+                )
+
+            if depth != posaxis:
+                return
+
+            if any(isinstance(x, ak.contents.Content) and x.is_option for x in inputs):
                 nextinputs = []
                 for x in inputs:
                     if x.is_option and x.content.is_list:
                         nextinputs.append(fill_none(x, [], axis=0, highlevel=False))
                     else:
                         nextinputs.append(x)
                 inputs = nextinputs
 
-            if depth == posaxis:
-                backend = backend_of(*inputs, default=cpu)
-
-                length = None
-                for x in inputs:
-                    if isinstance(x, ak.contents.Content):
-                        if not is_integer(length):
-                            length = x.length
-                        elif length != x.length and is_integer(x.length):
-                            raise ValueError(
-                                "all arrays must have the same length for "
-                                "axis={}".format(axis)
-                            )
+            # Ensure the lengths agree, taking known lengths over unknown lengths
+            length = None
+            for x in inputs:
+                if isinstance(x, ak.contents.Content):
+                    if length is None:
+                        length = x.length
+                    elif x.length is unknown_length:
+                        continue
+                    elif length is unknown_length:
+                        length = x.length
+                    elif length != x.length:
+                        raise ValueError(
+                            "all arrays must have the same length for "
+                            "axis={}".format(axis)
+                        )
+            assert length is not None
 
-            if depth == posaxis and all(
-                isinstance(x, ak.contents.Content)
-                and x.is_regular
+            if all(
+                (isinstance(x, ak.contents.Content) and x.is_regular)
                 or (isinstance(x, ak.contents.NumpyArray) and x.data.ndim > 1)
                 or not isinstance(x, ak.contents.Content)
                 for x in inputs
             ):
                 regulararrays = []
                 sizes = []
                 for x in inputs:
@@ -186,26 +200,33 @@
 
                 prototype = backend.index_nplike.empty(sum(sizes), dtype=np.int8)
                 start = 0
                 for tag, size in enumerate(sizes):
                     prototype[start : start + size] = tag
                     start += size
 
-                tags = ak.index.Index8(backend.index_nplike.tile(prototype, length))
+                tags = ak.index.Index8(
+                    backend.index_nplike.reshape(
+                        backend.index_nplike.broadcast_to(
+                            prototype, (length, prototype.size)
+                        ),
+                        (-1,),
+                    )
+                )
                 index = ak.contents.UnionArray.regular_index(tags, backend=backend)
                 inner = ak.contents.UnionArray.simplified(
                     tags,
                     index,
                     [x._content for x in regulararrays],
                     mergebool=mergebool,
                 )
 
-                return (ak.contents.RegularArray(inner, len(prototype)),)
+                return (ak.contents.RegularArray(inner, prototype.size),)
 
-            elif depth == posaxis and all(
+            elif all(
                 isinstance(x, ak.contents.Content)
                 and x.is_list
                 or (isinstance(x, ak.contents.NumpyArray) and x.data.ndim > 1)
                 or not isinstance(x, ak.contents.Content)
                 for x in inputs
             ):
                 nextinputs = []
@@ -213,15 +234,18 @@
                     if isinstance(x, ak.contents.Content):
                         nextinputs.append(x)
                     else:
                         nextinputs.append(
                             ak.contents.ListOffsetArray(
                                 ak.index.Index64(
                                     backend.index_nplike.arange(
-                                        length + 1, dtype=np.int64
+                                        backend.index_nplike.shape_item_as_index(
+                                            length + 1
+                                        ),
+                                        dtype=np.int64,
                                     ),
                                     nplike=backend.index_nplike,
                                 ),
                                 ak.contents.NumpyArray(
                                     backend.nplike.broadcast_to(
                                         backend.nplike.asarray([x]), (length,)
                                     )
@@ -259,24 +283,14 @@
 
                 inner = ak.contents.UnionArray.simplified(
                     tags, index, all_flatten, mergebool=mergebool
                 )
 
                 return (ak.contents.ListOffsetArray(offsets, inner),)
 
-            elif any(
-                x.minmax_depth == (1, 1)
-                for x in inputs
-                if isinstance(x, ak.contents.Content)
-            ):
-                raise ValueError(
-                    "at least one array is not deep enough to concatenate at "
-                    "axis={}".format(axis)
-                )
-
             else:
                 return None
 
         out = ak._broadcasting.broadcast_and_apply(
             content_or_others,
             action,
             behavior=behavior,
@@ -293,20 +307,20 @@
     length = sum([c.length for c in contents])
     first = contents[0]
     tags = ak.index.Index8.empty(length, first.backend.index_nplike)
     index = ak.index.Index64.empty(length, first.backend.index_nplike)
 
     offset = 0
     for i, content in enumerate(contents):
-        content._handle_error(
+        content.backend.maybe_kernel_error(
             content.backend["awkward_UnionArray_filltags_const", tags.dtype.type](
                 tags.data, offset, content.length, i
             )
         )
-        content._handle_error(
+        content.backend.maybe_kernel_error(
             content.backend["awkward_UnionArray_fillindex_count", index.dtype.type](
                 index.data, offset, content.length
             )
         )
         offset += content.length
 
     return ak.contents.UnionArray.simplified(
```

### Comparing `awkward-2.2.1/src/awkward/operations/ak_copy.py` & `awkward-2.2.2/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_corr.py` & `awkward-2.2.2/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_count.py` & `awkward-2.2.2/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.2.2/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_covar.py` & `awkward-2.2.2/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_drop_none.py` & `awkward-2.2.2/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_enforce_type.py` & `awkward-2.2.2/src/awkward/operations/ak_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_fields.py` & `awkward-2.2.2/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_fill_none.py` & `awkward-2.2.2/src/awkward/operations/ak_fill_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_firsts.py` & `awkward-2.2.2/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_flatten.py` & `awkward-2.2.2/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_arrow.py` & `awkward-2.2.2/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.2.2/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.2.2/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_buffers.py` & `awkward-2.2.2/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_categorical.py` & `awkward-2.2.2/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_cupy.py` & `awkward-2.2.2/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_iter.py` & `awkward-2.2.2/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_jax.py` & `awkward-2.2.2/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_json.py` & `awkward-2.2.2/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_numpy.py` & `awkward-2.2.2/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_parquet.py` & `awkward-2.2.2/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.2.2/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_from_regular.py` & `awkward-2.2.2/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_full_like.py` & `awkward-2.2.2/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_is_categorical.py` & `awkward-2.2.2/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_is_none.py` & `awkward-2.2.2/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_is_tuple.py` & `awkward-2.2.2/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_is_valid.py` & `awkward-2.2.2/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_isclose.py` & `awkward-2.2.2/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_linear_fit.py` & `awkward-2.2.2/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_local_index.py` & `awkward-2.2.2/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_mask.py` & `awkward-2.2.2/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_max.py` & `awkward-2.2.2/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_mean.py` & `awkward-2.2.2/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.2.2/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.2.2/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.2.2/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_min.py` & `awkward-2.2.2/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_moment.py` & `awkward-2.2.2/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.2.2/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.2.2/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_num.py` & `awkward-2.2.2/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_ones_like.py` & `awkward-2.2.2/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_pad_none.py` & `awkward-2.2.2/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_parameters.py` & `awkward-2.2.2/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_prod.py` & `awkward-2.2.2/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_ptp.py` & `awkward-2.2.2/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_ravel.py` & `awkward-2.2.2/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_run_lengths.py` & `awkward-2.2.2/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_singletons.py` & `awkward-2.2.2/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_softmax.py` & `awkward-2.2.2/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_sort.py` & `awkward-2.2.2/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_std.py` & `awkward-2.2.2/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_strings_astype.py` & `awkward-2.2.2/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_sum.py` & `awkward-2.2.2/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_arrow.py` & `awkward-2.2.2/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.2.2/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_backend.py` & `awkward-2.2.2/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_buffers.py` & `awkward-2.2.2/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_categorical.py` & `awkward-2.2.2/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_cupy.py` & `awkward-2.2.2/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.2.2/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_jax.py` & `awkward-2.2.2/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_json.py` & `awkward-2.2.2/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_layout.py` & `awkward-2.2.2/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_list.py` & `awkward-2.2.2/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_numpy.py` & `awkward-2.2.2/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_packed.py` & `awkward-2.2.2/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_parquet.py` & `awkward-2.2.2/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.2.2/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_to_regular.py` & `awkward-2.2.2/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_transform.py` & `awkward-2.2.2/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_type.py` & `awkward-2.2.2/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_unflatten.py` & `awkward-2.2.2/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_unzip.py` & `awkward-2.2.2/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_validity_error.py` & `awkward-2.2.2/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_values_astype.py` & `awkward-2.2.2/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_var.py` & `awkward-2.2.2/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_where.py` & `awkward-2.2.2/src/awkward/operations/ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_with_field.py` & `awkward-2.2.2/src/awkward/operations/ak_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_with_name.py` & `awkward-2.2.2/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_with_parameter.py` & `awkward-2.2.2/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_without_field.py` & `awkward-2.2.2/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_without_parameters.py` & `awkward-2.2.2/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_zeros_like.py` & `awkward-2.2.2/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/operations/ak_zip.py` & `awkward-2.2.2/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/__init__.py` & `awkward-2.2.2/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.2.2/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/arraytype.py` & `awkward-2.2.2/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/listtype.py` & `awkward-2.2.2/src/awkward/types/listtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,21 @@
         if typestr is not None:
             out = [typestr]
         else:
             params = self._str_parameters()
             if params is None:
                 out = ["var * ", *self._content._str(indent, compact, behavior)]
             else:
-                out = ["[var * ", *self._content._str(indent, compact, behavior)] + [
-                    f", {params}]"
+                out = [
+                    "[var * ",
+                    *self._content._str(indent, compact, behavior),
+                    f", {params}]",
                 ]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
         compare_parameters = (
```

### Comparing `awkward-2.2.1/src/awkward/types/numpytype.py` & `awkward-2.2.2/src/awkward/types/numpytype.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                     units = units + ", "
                 elif units is None:
                     units = ""
                 elif params is None:
                     params = ""
                 out = [self._primitive, "[", units, params, "]"]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._primitive), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool) -> bool:
         compare_parameters = (
```

### Comparing `awkward-2.2.1/src/awkward/types/optiontype.py` & `awkward-2.2.2/src/awkward/types/optiontype.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,19 +80,21 @@
                 else:
                     head = ["?"]
 
             else:
                 head = ["option["]
                 tail = [f", {params}]"]
 
-        return (
-            [*head, self._str_categorical_begin(), *content_out]
-            + [self._str_categorical_end()]
-            + tail
-        )
+        return [
+            *head,
+            self._str_categorical_begin(),
+            *content_out,
+            self._str_categorical_end(),
+            *tail,
+        ]
 
     def __repr__(self):
         args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def simplify_option_union(self):
         if isinstance(self._content, UnionType):
```

### Comparing `awkward-2.2.1/src/awkward/types/recordtype.py` & `awkward-2.2.2/src/awkward/types/recordtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,49 +158,39 @@
                     pairs.append([key_str, ": ", *v])
                 flat_pairs = [y for x in pairs for y in x]
 
             if params is None:
                 if self.is_tuple:
                     flat_children = [y for x in children for y in x]
                     if name is None:
-                        out = ["(", pre, *flat_children] + [post, ")"]
+                        out = ["(", pre, *flat_children, post, ")"]
                     else:
-                        out = [name, "[", pre, *flat_children] + [post, "]"]
+                        out = [name, "[", pre, *flat_children, post, "]"]
                 else:
                     if name is None:
-                        out = ["{", pre, *flat_pairs] + [post, "}"]
+                        out = ["{", pre, *flat_pairs, post, "}"]
                     else:
-                        out = [name, "[", pre, *flat_pairs] + [post, "]"]
+                        out = [name, "[", pre, *flat_pairs, post, "]"]
 
             else:
                 if self.is_tuple:
                     flat_children = [y for x in children for y in x]
                     if name is None:
-                        out = ["tuple[[", pre, *flat_children] + [
-                            post,
-                            "], ",
-                            params,
-                            "]",
-                        ]
+                        out = ["tuple[[", pre, *flat_children, post, "], ", params, "]"]
                     else:
                         c = "" if len(self._contents) == 0 else ", "
-                        out = [name, "[", pre, *flat_children] + [c, post, params, "]"]
+                        out = [name, "[", pre, *flat_children, c, post, params, "]"]
                 else:
                     if name is None:
-                        out = ["struct[{", pre, *flat_pairs] + [
-                            post,
-                            "}, ",
-                            params,
-                            "]",
-                        ]
+                        out = ["struct[{", pre, *flat_pairs, post, "}, ", params, "]"]
                     else:
                         c = "" if len(self._contents) == 0 else ", "
-                        out = [name, "[", pre, *flat_pairs] + [c, post, params, "]"]
+                        out = [name, "[", pre, *flat_pairs, c, post, params, "]"]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._contents), repr(self._fields), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool) -> bool:
         if not isinstance(other, type(self)):
```

### Comparing `awkward-2.2.1/src/awkward/types/regulartype.py` & `awkward-2.2.2/src/awkward/types/regulartype.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,20 @@
                 ]
             else:
                 out = [
                     "[",
                     str(self._size),
                     " * ",
                     *self._content._str(indent, compact, behavior),
-                ] + [", ", params, "]"]
+                    ", ",
+                    params,
+                    "]",
+                ]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._content), repr(self._size), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool) -> bool:
         compare_parameters = (
```

### Comparing `awkward-2.2.1/src/awkward/types/scalartype.py` & `awkward-2.2.2/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/type.py` & `awkward-2.2.2/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/src/awkward/types/uniontype.py` & `awkward-2.2.2/src/awkward/types/uniontype.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,19 +92,19 @@
                         y = x._str(indent + "    ", compact, behavior)
                 children.append(y)
 
             flat_children = [y for x in children for y in x]
             params = self._str_parameters()
 
             if params is None:
-                out = ["union[", pre, *flat_children] + [post, "]"]
+                out = ["union[", pre, *flat_children, post, "]"]
             else:
-                out = ["union[", pre, *flat_children] + [", ", post, params, "]"]
+                out = ["union[", pre, *flat_children, ", ", post, params, "]"]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._contents), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
         compare_parameters = (
```

### Comparing `awkward-2.2.1/src/awkward/types/unknowntype.py` & `awkward-2.2.2/src/awkward/types/unknowntype.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         else:
             params = self._str_parameters()
             if params is None:
                 out = ["unknown"]
             else:
                 out = ["unknown[", params, "]"]
 
-        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
+        return [self._str_categorical_begin(), *out, self._str_categorical_end()]
 
     def __repr__(self):
         args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
     def _is_equal_to(self, other, all_parameters: bool):
         compare_parameters = (
```

### Comparing `awkward-2.2.1/tests/test_0002_minimal_listarray.py` & `awkward-2.2.2/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0008_slices_and_getitem.py` & `awkward-2.2.2/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0011_listarray.py` & `awkward-2.2.2/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0013_error_handling_struct.py` & `awkward-2.2.2/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0014_finish_up_getitem.py` & `awkward-2.2.2/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0018_fromiter_fillable.py` & `awkward-2.2.2/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0019_use_json_library.py` & `awkward-2.2.2/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.2.2/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0021_emptyarray.py` & `awkward-2.2.2/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0023_regular_array.py` & `awkward-2.2.2/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0024_use_regular_array.py` & `awkward-2.2.2/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0025_record_array.py` & `awkward-2.2.2/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0028_add_dressed_types.py` & `awkward-2.2.2/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0032_replace_dressedtype.py` & `awkward-2.2.2/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0046_start_indexedarray.py` & `awkward-2.2.2/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.2.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0057_introducing_forms.py` & `awkward-2.2.2/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0070_argmin_and_argmax.py` & `awkward-2.2.2/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0072_fillna_operation.py` & `awkward-2.2.2/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0074_argsort_and_sort.py` & `awkward-2.2.2/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0077_zip_operation.py` & `awkward-2.2.2/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0078_argcross_and_cross.py` & `awkward-2.2.2/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0079_argchoose_and_choose.py` & `awkward-2.2.2/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.2.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0084_start_unionarray.py` & `awkward-2.2.2/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0086_nep13_ufunc.py` & `awkward-2.2.2/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0089_numpy_functions.py` & `awkward-2.2.2/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.2.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0107_assign_fields_to_records.py` & `awkward-2.2.2/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.2.2/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0115_generic_reducer_operation.py` & `awkward-2.2.2/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0118_numba_cpointers.py` & `awkward-2.2.2/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.2.2/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0124_strings_in_numba.py` & `awkward-2.2.2/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0127_tomask_operation.py` & `awkward-2.2.2/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.2.2/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0138_emptyarray_type.py` & `awkward-2.2.2/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0150_flatten.py` & `awkward-2.2.2/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0163_negative_axis_wrap.py` & `awkward-2.2.2/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.2.2/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0173_astype_operation.py` & `awkward-2.2.2/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0184_concatenate_operation.py` & `awkward-2.2.2/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.2.2/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.2.2/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0222_count_with_axis0.py` & `awkward-2.2.2/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0224_arrow_to_awkward.py` & `awkward-2.2.2/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0264_reduce_last_empty.py` & `awkward-2.2.2/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0273_path_for_with_field.py` & `awkward-2.2.2/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.2.2/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.2.2/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0315_integerindex.py` & `awkward-2.2.2/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0331_pandas_indexedarray.py` & `awkward-2.2.2/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.2.2/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.2.2/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0348_form_keys.py` & `awkward-2.2.2/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0355_mixins.py` & `awkward-2.2.2/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0395_complex_type_arrays.py` & `awkward-2.2.2/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.2.2/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.2.2/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.2.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0404_array_validity_check.py` & `awkward-2.2.2/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.2.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.2.2/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.2.2/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.2.2/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.2.2/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0496_provide_local_index.py` & `awkward-2.2.2/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.2.2/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.2.2/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.2.2/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.2.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0549_numba_array_asarray.py` & `awkward-2.2.2/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0557_min_max_initial_argument.py` & `awkward-2.2.2/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.2.2/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0572_numba_array_ndim.py` & `awkward-2.2.2/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.2.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0583_implement_unflatten_function.py` & `awkward-2.2.2/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.2.2/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.2.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.2.2/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0674_categorical_validation.py` & `awkward-2.2.2/tests/test_0674_categorical_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     batch = pyarrow.RecordBatch.from_arrays([dict_array], ["year"])
     batch_new_schema = pyarrow.RecordBatch.from_arrays(
         [dict_array_new_schema], ["year"]
     )
 
     batches = [batch] * 3
-    batches_mixed_schema = [batch] + [batch_new_schema]
+    batches_mixed_schema = [batch, batch_new_schema]
 
     table = pyarrow.Table.from_batches(batches)
     table_mixed_schema = pyarrow.Table.from_batches(batches_mixed_schema)
 
     array = ak.operations.from_arrow(table)
     array_mixed_schema = ak.operations.from_arrow(table_mixed_schema)
```

### Comparing `awkward-2.2.1/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.2.2/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.2.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.2.2/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0733_run_lengths.py` & `awkward-2.2.2/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.2.2/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.2.2/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0773_typeparser.py` & `awkward-2.2.2/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.2.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.2.2/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0803_argsort_fix_type.py` & `awkward-2.2.2/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.2.2/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.2.2/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.2.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0828_arrow_datatype_null.py` & `awkward-2.2.2/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0835_datetime_type.py` & `awkward-2.2.2/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0835_datetime_type_pandas.py` & `awkward-2.2.2/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.2.2/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0850_argsort_mask_array.py` & `awkward-2.2.2/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.2.2/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0875_arrow_null_type.py` & `awkward-2.2.2/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0879_non_primitive_with_field.py` & `awkward-2.2.2/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.2.2/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0889_ptp.py` & `awkward-2.2.2/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0896_content_classes_refactoring.py` & `awkward-2.2.2/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.2.2/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.2.2/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.2.2/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.2.2/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0912_packed.py` & `awkward-2.2.2/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0914_types_and_forms.py` & `awkward-2.2.2/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0916_datetime_values_astype.py` & `awkward-2.2.2/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.2.2/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.2.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.2.2/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.2.2/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0959__getitem_array_implementation.py` & `awkward-2.2.2/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.2.2/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.2.2/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.2.2/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0984_ravel.py` & `awkward-2.2.2/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.2.2/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.2.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.2.2/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1030_mixin_class_name.py` & `awkward-2.2.2/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1031_start_getitem_next.py` & `awkward-2.2.2/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.2.2/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1049_concatenate_single_array.py` & `awkward-2.2.2/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.2.2/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1059_localindex.py` & `awkward-2.2.2/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.2.2/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.2.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1072_sort.py` & `awkward-2.2.2/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1074_combinations.py` & `awkward-2.2.2/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1075_validityerror.py` & `awkward-2.2.2/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1110_type_tracer_1.py` & `awkward-2.2.2/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1116_project_maskedarrays.py` & `awkward-2.2.2/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.2.2/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.2.2/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.2.2/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1135_rpad_operation.py` & `awkward-2.2.2/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.2.2/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1137_num.py` & `awkward-2.2.2/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1142_numbers_to_type.py` & `awkward-2.2.2/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1149_datetime_sort.py` & `awkward-2.2.2/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.2.2/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1162_ak_from_json_schema.py` & `awkward-2.2.2/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.2.2/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.2.2/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.2.2/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1193_is_none_nested_option.py` & `awkward-2.2.2/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1233_ak_with_name.py` & `awkward-2.2.2/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.2.2/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def roundtrip(layout):
     assert isinstance(layout, ak.contents.Content)
 
     lookup = ak._lookup.Lookup(layout)
     assert isinstance(lookup, ak._lookup.Lookup)
 
-    numbatype = ak_numba_arrayview.tonumbatype(layout.form)
+    numbatype = ak_numba_arrayview.to_numbatype(layout.form)
     assert isinstance(numbatype, ak_numba_layout.ContentType)
 
     layout2 = numbatype.tolayout(lookup, 0, ())
     assert isinstance(layout2, ak.contents.Content)
 
     assert layout.to_list() == layout2.to_list()
     assert layout.form.type == layout2.form.type
```

### Comparing `awkward-2.2.1/tests/test_1259_simplify_optiontype.py` & `awkward-2.2.2/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.2.2/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1271_fix_4D_reducers.py` & `awkward-2.2.2/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1294_to_and_from_parquet.py` & `awkward-2.2.2/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.2.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.2.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1300b_same_for_numba.py` & `awkward-2.2.2/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1308_zip_after_option.py` & `awkward-2.2.2/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1318_array_function_types.py` & `awkward-2.2.2/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1320_mask_identity_defaults.py` & `awkward-2.2.2/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.2.2/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1345_avro_reader.py` & `awkward-2.2.2/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1351_is_tuple.py` & `awkward-2.2.2/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1374_to_rdataframe.py` & `awkward-2.2.2/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1377_ravel_string.py` & `awkward-2.2.2/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.2.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1399_from_jax.py` & `awkward-2.2.2/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1399_to_jax.py` & `awkward-2.2.2/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1405_slicing_untested_cases.py` & `awkward-2.2.2/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1415_behaviour_forwarding.py` & `awkward-2.2.2/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.2.2/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.2.2/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.2.2/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.2.2/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1473_from_rdataframe.py` & `awkward-2.2.2/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.2.2/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.2.2/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.2.2/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1504_typetracer_like.py` & `awkward-2.2.2/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.2.2/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1511_set_attribute.py` & `awkward-2.2.2/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.2.2/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.2.2/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.2.2/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.2.2/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.2.2/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.2.2/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.2.2/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1607_no_reducers_on_records.py` & `awkward-2.2.2/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1613_generator_tolayout_records.py` & `awkward-2.2.2/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.2.2/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1620_layout_builders.py` & `awkward-2.2.2/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.2.2/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.2.2/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.2.2/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1671_categorical_type.py` & `awkward-2.2.2/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1672_broadcast_parameters.py` & `awkward-2.2.2/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1677_array_builder_in_numba.py` & `awkward-2.2.2/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.2.2/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.2.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1688_pack_categorical.py` & `awkward-2.2.2/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1703_fill_none_typetracer.py` & `awkward-2.2.2/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.2.2/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.2.2/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.2.2/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.2.2/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1762_jax_behavior_support.py` & `awkward-2.2.2/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1764_jax_jacobian.py` & `awkward-2.2.2/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.2.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1766_record_form_fields.py` & `awkward-2.2.2/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.2.2/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.2.2/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1790_reduce_regulararray.py` & `awkward-2.2.2/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.2.2/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.2.2/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.2.2/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.2.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.2.2/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.2.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.2.2/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1904_drop_none.py` & `awkward-2.2.2/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.2.2/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.2.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.2.2/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1936_with_field_broadcasting.py` & `awkward-2.2.2/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1940_ak_backend.py` & `awkward-2.2.2/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1943_regular_indexing.py` & `awkward-2.2.2/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.2.2/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_1961_ak_without_field.py` & `awkward-2.2.2/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2020_reduce_axis_none.py` & `awkward-2.2.2/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.2.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2023_from_rdataframe.py` & `awkward-2.2.2/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.2.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.2.2/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2055_array_builder_check.py` & `awkward-2.2.2/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2058_merge_numpy_array.py` & `awkward-2.2.2/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2064_fill_none_record.py` & `awkward-2.2.2/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.2.2/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2070_to_layout_string.py` & `awkward-2.2.2/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.2.2/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2078_array_function_wrap.py` & `awkward-2.2.2/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2082_broadcast_zero_size.py` & `awkward-2.2.2/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2096_ak_scalar_type.py` & `awkward-2.2.2/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2101_pickle_behavior_class.py` & `awkward-2.2.2/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2104_numpy_merge_option.py` & `awkward-2.2.2/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2106_pickle_class.py` & `awkward-2.2.2/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2108_fill_none_indexed.py` & `awkward-2.2.2/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2115_fix_up_typetracers.py` & `awkward-2.2.2/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2125_type_of_scalar.py` & `awkward-2.2.2/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.2.2/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2179_parameter_merging_rules.py` & `awkward-2.2.2/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2185_merge_union_of_records.py` & `awkward-2.2.2/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.2.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2198_almost_equal.py` & `awkward-2.2.2/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.2.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2214_offset_bool_index.py` & `awkward-2.2.2/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.2.2/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2229_getitem_range_slice.py` & `awkward-2.2.2/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.2.2/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.2.2/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.2.2/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2246_slice_not_packed.py` & `awkward-2.2.2/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2250_full_like_bool.py` & `awkward-2.2.2/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.2.2/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2263_to_packed_list.py` & `awkward-2.2.2/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2266_fix_nan_to_num.py` & `awkward-2.2.2/tests/test_2266_fix_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2267_broadcast_fields.py` & `awkward-2.2.2/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2293_unflatten_typetracer.py` & `awkward-2.2.2/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2296_duplicate_field.py` & `awkward-2.2.2/tests/test_2296_duplicate_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2297_common_backend.py` & `awkward-2.2.2/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.2.2/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2306_cppyy_git.py` & `awkward-2.2.2/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2319_from_buffers_array.py` & `awkward-2.2.2/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2327_array_interface.py` & `awkward-2.2.2/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.2.2/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.2.2/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2354_ufunc_same_backend.py` & `awkward-2.2.2/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2355_to_backend_record.py` & `awkward-2.2.2/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.2.2/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2364_empty_list_of_string.py` & `awkward-2.2.2/tests/test_2364_empty_list_of_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2365_enforce_type.py` & `awkward-2.2.2/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2368_type_is_equal.py` & `awkward-2.2.2/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2373_unzip_touching.py` & `awkward-2.2.2/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2374_cartesian_touching.py` & `awkward-2.2.2/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2385_with_field_empty_record.py` & `awkward-2.2.2/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2395_copy_asarray_touch.py` & `awkward-2.2.2/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2410_string_broadcast.py` & `awkward-2.2.2/tests/test_2410_string_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.2.2/tests/test_2411_cartesian_axis_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2417_bytemasked_singletons.py` & `awkward-2.2.2/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2424_almost_equal_union_record.py` & `awkward-2.2.2/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2425_forms_from_type.py` & `awkward-2.2.2/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/test_2426_is_equal_to.py` & `awkward-2.2.2/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/list-depths-records-list.parquet` & `awkward-2.2.2/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/list-depths-records.parquet` & `awkward-2.2.2/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/list-depths-strings.parquet` & `awkward-2.2.2/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/list-depths.parquet` & `awkward-2.2.2/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nonnullable-depths.parquet` & `awkward-2.2.2/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-depths.parquet` & `awkward-2.2.2/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-levels.parquet` & `awkward-2.2.2/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.2.2/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.2.2/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.2.2/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-list-depths.parquet` & `awkward-2.2.2/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/nullable-record-primitives.parquet` & `awkward-2.2.2/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/record-primitives.parquet` & `awkward-2.2.2/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/test-nan-inf.json` & `awkward-2.2.2/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/test-two-arrays.json` & `awkward-2.2.2/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests/samples/test.json` & `awkward-2.2.2/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests-cuda/test_1276_cuda_num.py` & `awkward-2.2.2/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.2.2/tests-cuda/test_1276_cuda_transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import cupy as cp  # noqa: F401
 import numpy as np
-import pytest
 
 import awkward as ak
 
 
 def test_tocuda():
     content = ak.Array(
         ["one", "two", "three", "four", "five", "six", "seven", "eight", "nine"]
@@ -41,17 +40,14 @@
     array = ak.contents.EmptyArray()
     cuda_array = ak.to_backend(array, "cuda")
     copyback_array = ak.to_backend(cuda_array, "cpu")
     assert ak.to_list(cuda_array) == ak.to_list(array)
     assert ak.to_list(copyback_array) == ak.to_list(array)
 
 
-@pytest.mark.skip(
-    reason="Can't test this right now because of unimplemented CUDA Kernels (awkward_ListOffsetArray_compact_offsets)"
-)
 def test_tocuda_unimplementedkernels():
     content = ak.contents.NumpyArray(
         np.array([1.1, 2.2, 3.3, 4.4, 5.5, 6.6, 7.7, 8.8, 9.9])
     )
     offsets = ak.index.Index64(np.array([0, 3, 3, 5, 6, 9]))
     array = ak.contents.ListOffsetArray(offsets, content)
     cuda_array = ak.to_backend(array, "cuda")
```

### Comparing `awkward-2.2.1/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.2.2/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests-cuda/test_1276_from_cupy.py` & `awkward-2.2.2/tests-cuda/test_1276_from_cupy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import cupy as cp
 import numpy as np
-import pytest
 
 import awkward as ak
 
 
 def test_from_cupy():
     cupy_array_1d = cp.arange(10)
     cupy_array_2d = cp.array([[1.1, 2.2], [3.3, 4.4], [5.5, 6.6], [7.7, 8.8]])
@@ -31,17 +30,14 @@
 
 
 def test_NumpyArray_constructor():
     assert ak.backend(ak.contents.NumpyArray(np.array([1, 2, 3]))) == "cpu"
     assert ak.backend(ak.contents.NumpyArray(cp.array([1, 2, 3]))) == "cuda"
 
 
-@pytest.mark.skip(
-    reason="Can't test this right now because of unimplemented CUDA Kernels (awkward_ListOffsetArray_compact_offsets"
-)
 def test_add():
     one = ak.Array([[1.1, 2.2, 3.3], [], [4.4, 5.5]], backend="cuda")
     two = ak.Array([100, 200, 300], backend="cuda")
     assert ak.backend(one) == "cuda"
     assert ak.backend(two) == "cuda"
     three = one + two
     assert ak.to_list(three) == [[101.1, 102.2, 103.3], [], [304.4, 305.5]]
```

### Comparing `awkward-2.2.1/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.2.2/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests-cuda/test_1381_check_errors.py` & `awkward-2.2.2/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.2.2/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/.gitignore` & `awkward-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/LICENSE` & `awkward-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.2.1/pyproject.toml` & `awkward-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.2.1"
+version = "2.2.2"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,15 +36,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==15",
+    "awkward_cpp==16",
     "importlib_resources;python_version < \"3.9\"",
     "numpy>=1.17.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.1"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.2.2"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -11,15 +11,15 @@
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==15",
+Utilities", ] dependencies = [ "awkward_cpp==16",
 "importlib_resources;python_version < \"3.9\"", "numpy>=1.17.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
```

### Comparing `awkward-2.2.1/PKG-INFO` & `awkward-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.2.1
+Version: 2.2.2
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,15 +32,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==15
+Requires-Dist: awkward-cpp==16
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.2.1 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.2.2 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,15 +18,15 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==15 Requires-Dist: importlib-resources;
+Requires-Dist: awkward-cpp==16 Requires-Dist: importlib-resources;
 python_version < '3.9' Requires-Dist: numpy>=1.17.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
```

