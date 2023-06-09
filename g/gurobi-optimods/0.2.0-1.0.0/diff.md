# Comparing `tmp/gurobi_optimods-0.2.0.tar.gz` & `tmp/gurobi_optimods-1.0.0.tar.gz`

## Comparing `gurobi_optimods-0.2.0.tar` & `gurobi_optimods-1.0.0.tar`

### file list

```diff
@@ -1,92 +1,90 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/Makefile
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tox.ini
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/new_mod.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/doc-build.yml
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/doc-tests.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.github/workflows/wheel-tests.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/make.bat
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/adding.rst
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/api.rst
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/contact.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/dev-reference.rst
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/gallery.rst
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/license.rst
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/usage.rst
--rw-r--r--   0        0        0     8660 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/bipartite-matching.rst
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/lad-regression.rst
--rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/min-cost-flow.rst
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/mwis.rst
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/portfolio.rst
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/qubo.rst
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/workforce.rst
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-example.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-figs.py
--rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-flow.png
--rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-result.png
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-coeffs.png
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-errors.png
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/lad-regression-coeffs.png
--rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/min-cost-flow-result.png
--rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/mvp.png
--rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/mwis.png
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/pie.png
--rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/qubo.png
--rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/figures/shortest-path-result.png
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/mods/icons/lad-regression.png
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/graphs.bib
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/portfolio.bib
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/qubo.bib
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/regression.bib
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/docs/source/refs/workforce.bib
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/__init__.py
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/bipartite_matching.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/datasets.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/min_cost_flow.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/mwis.py
--rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/portfolio.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/qubo.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/regression.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/utils.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/workforce.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/edge_data1.csv
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/edge_data2.csv
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/node_data1.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/graphs/node_data2.csv
--rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/portfolio/portfolio.csv
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/preferences.csv
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/worker_limits.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_bipartite_matching.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_graph_utils.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_min_cost_flow.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_mwis.py
--rw-r--r--   0        0        0    31002 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_portfolio.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_qubo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_regression.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/test_workforce.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/NOTICE
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/README.md
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 gurobi_optimods-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/Makefile
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tox.ini
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/new_mod.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/doc-build.yml
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/doc-tests.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.github/workflows/wheel-tests.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/adding.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/api.rst
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/contact.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/dev-reference.rst
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/gallery.rst
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/index.rst
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/license.rst
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/bipartite-matching.rst
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/lad-regression.rst
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/min-cost-flow.rst
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/mwis.rst
+-rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/portfolio.rst
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/qubo.rst
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/workforce.rst
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-example.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-figs.py
+-rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-flow.png
+-rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-result.png
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-coeffs.png
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-errors.png
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/lad-regression-coeffs.png
+-rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/min-cost-flow-result.png
+-rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/mvp.png
+-rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/mwis.png
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/pie.png
+-rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/qubo.png
+-rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/figures/shortest-path-result.png
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/mods/icons/lad-regression.png
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/graphs.bib
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/portfolio.bib
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/qubo.bib
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/regression.bib
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/docs/source/refs/workforce.bib
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/__init__.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/bipartite_matching.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/datasets.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/min_cost_flow.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/mwis.py
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/portfolio.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/qubo.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/regression.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/utils.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/workforce.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/graphs/simple_graph_edges.csv
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/graphs/simple_graph_nodes.csv
+-rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/portfolio/portfolio.csv
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/preferences.csv
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/worker_limits.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_bipartite_matching.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_graph_utils.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_min_cost_flow.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_mwis.py
+-rw-r--r--   0        0        0    32785 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_portfolio.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_qubo.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_regression.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/test_workforce.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/tests/utils.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/NOTICE
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.0/PKG-INFO
```

### Comparing `gurobi_optimods-0.2.0/CODE_OF_CONDUCT.md` & `gurobi_optimods-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/CONTRIBUTING.md` & `gurobi_optimods-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/pull_request_template.md` & `gurobi_optimods-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/ISSUE_TEMPLATE/new_mod.md` & `gurobi_optimods-1.0.0/.github/ISSUE_TEMPLATE/new_mod.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/code-quality.yml` & `gurobi_optimods-1.0.0/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/doc-build.yml` & `gurobi_optimods-1.0.0/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/doc-tests.yml` & `gurobi_optimods-1.0.0/.github/workflows/doc-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/publish-pypi.yml` & `gurobi_optimods-1.0.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/python-tests.yml` & `gurobi_optimods-1.0.0/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/release.yml` & `gurobi_optimods-1.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.github/workflows/wheel-tests.yml` & `gurobi_optimods-1.0.0/.github/workflows/wheel-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/Makefile` & `gurobi_optimods-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/make.bat` & `gurobi_optimods-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/adding.rst` & `gurobi_optimods-1.0.0/docs/source/adding.rst`

 * *Files 6% similar despite different names*

```diff
@@ -112,18 +112,18 @@
 should also add an icon to the gallery card for your mod.
 
 Your documentation page must contain example codes that new users can
 immediately used, with presentation of the results included in the documentation
 page.
 
 The implementation of the Mod (description of the mathematical model or
-algorithms used) should be hidden from the user at first glance. We use tabs to
-do this. Any mathematical and algorithmic details should be placed in a tab and
-clearly indicate that this is advanced detail the user does not need to fully
-understand in order to use the Mod.
+algorithms used) should be hidden from the user at first glance. We use the ``..
+dropdown:`` directive for this. Any mathematical and algorithmic details should
+be placed in a dropdown and clearly indicate that this is advanced detail the
+user does not need to fully understand in order to use the Mod.
 
 Including datasets
 ------------------
 
 Some of your examples may rely on datasets. These can be packaged with the
 optimods to enable users to quickly reproduce the examples in your documentation.
```

### Comparing `gurobi_optimods-0.2.0/docs/source/api.rst` & `gurobi_optimods-1.0.0/docs/source/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 API Reference
 =============
 
 .. automodule:: gurobi_optimods.bipartite_matching
    :members: maximum_bipartite_matching
 
 .. automodule:: gurobi_optimods.min_cost_flow
-   :members: min_cost_flow, min_cost_flow_networkx, min_cost_flow_scipy
+   :members: min_cost_flow_pandas, min_cost_flow_networkx, min_cost_flow_scipy
 
 .. automodule:: gurobi_optimods.mwis
    :members: maximum_weighted_independent_set
 
 .. automodule:: gurobi_optimods.portfolio
    :members: MeanVariancePortfolio, PortfolioResult
```

### Comparing `gurobi_optimods-0.2.0/docs/source/conf.py` & `gurobi_optimods-1.0.0/docs/source/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,28 +65,23 @@
     "refs/graphs.bib",
     "refs/portfolio.bib",
     "refs/qubo.bib",
     "refs/regression.bib",
     "refs/workforce.bib",
 ]
 
-rst_prolog = """.. warning::
-    This code is in a pre-release state. It may not be fully functional and breaking changes
-    can occur without notice.
-"""
-
 # -- numpydoc magic linking
 
 numpydoc_xref_param_type = True
 numpydoc_xref_aliases = {
     "DataFrame": "pandas.DataFrame",
-    "spmatrix": "scipy.sparse.spmatrix",
-    "QuboResult": "gurobi_optimods.qubo.QuboResult",
-    "Graph": "networkx.Graph",
     "DiGraph": "networkx.DiGraph",
+    "Graph": "networkx.Graph",
+    "LinAlgError": "numpy.linalg.LinAlgError",
+    "spmatrix": "scipy.sparse.spmatrix",
 }
 numpydoc_xref_ignore = {"optional", "or", "of"}
 
 
 # -- Docstring preprocessing for autodoc
 
 autodoc_typehints = "none"
@@ -107,51 +102,50 @@
         print(f"Modified signature of {name}")
         return new_signature, return_annotation
 
     return signature, return_annotation
 
 
 boilerplate = """
-:param verbose: ``verbose=False`` suppresses all console output (optional, defaults to ``True``)
-:type verbose: :class:`bool`
-:param logfile: Write all mod output to the given file path (optional, defaults to ``None``: no log)
-:type logfile: :class:`str`
-:param solver_params: Gurobi parameters to be passed to the solver (optional)
-:type solver_params: :class:`dict`
+    **verbose** : :ref:`bool <python:bltin-boolean-values>`, optional
+        ``verbose=False`` suppresses all console output
+
+    **logfile** : :class:`python:str`, optional
+        Write all mod output to the given file path
+
+    **solver_params** : :class:`python:dict`, optional
+        Gurobi parameters to be passed to the solver
 """
-boilerplate = boilerplate.strip().split("\n")
+boilerplate = boilerplate.split("\n")
 
 
 def process_docstring(app, what, name, obj, options, lines):
     """Add parameter entries for decorated mods"""
 
     if what in ["function", "method"] and hasattr(obj, "_decorated_mod"):
         # Find where the last input parameter is listed
         in_paramlist = False
         lineno = None
         for i, line in enumerate(lines):
-            if line.startswith(":return"):
-                lineno = i - 1
-                break
-            if line.startswith(":type") or line.startswith(":param"):
+            if ":Parameters:" in line:
                 in_paramlist = True
-            if in_paramlist and not line.strip():
+            elif in_paramlist and (
+                ":Returns:" in line or "processed by numpydoc" in line
+            ):
                 lineno = i - 1
                 break
 
         if lineno is None:
             raise ValueError(f"Failed to find param list for {name}")
 
-        print(f"Added params to {name} after line {lineno}: '{lines[lineno]}'")
-
         # Insert boilerplate bits
         for line in reversed(boilerplate):
             lines.insert(lineno, line)
 
     if what == "module":
         lines.append("")
         lines.append(f"The following mods can be imported from ``{name}``:")
 
 
-# def setup(app):
-#     app.connect("autodoc-process-signature", process_signature)
-#     app.connect("autodoc-process-docstring", process_docstring)
+def setup(app):
+    app.connect("autodoc-process-signature", process_signature)
+    app.connect("autodoc-process-docstring", process_docstring)
```

### Comparing `gurobi_optimods-0.2.0/docs/source/contributing.rst` & `gurobi_optimods-1.0.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/dev-reference.rst` & `gurobi_optimods-1.0.0/docs/source/dev-reference.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 Developer Reference
 ===================
 
-.. warning::
-    This page is under construction
-
-A place for detailed information on the tools/packages we use, to guide
+This page contains further information on the tools/packages we use, to guide
 developers who are working on mods.
 
+The ``@optimod`` decorator
+--------------------------
+
+The ``@optimod`` decorator should be added to any Mod functions which need to
+create Gurobi models. :doc:`adding` provides a template for how to apply the
+decorator. The decorator provides the following arguments automatically:
+
+* ``verbose``, enabling users to shut off output;
+* ``logfile``, enabling users to send Mod logs to a file; and
+* ``solver_params``, enabling users to pass a dictionary of parameters to the
+  Gurobi Optimizer.
+
+As a Mod developer, your Mod must take a keyword argument ``create_env``. This
+function should be called to create a Gurobi environment inside your Mod, and
+all gurobipy ``Model`` objects should use this environment. The environment must
+be properly closed before your Mod function returns (this is best achieved by
+using context managers).
+
 Adding Citations
 ----------------
 
 We use
 `sphinxcontrib-bibtex <https://sphinxcontrib-bibtex.readthedocs.io/en/latest/index.html>`_
 for citations. To add citations in your mod documentation page:
```

### Comparing `gurobi_optimods-0.2.0/docs/source/gallery.rst` & `gurobi_optimods-1.0.0/docs/source/gallery.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/index.rst` & `gurobi_optimods-1.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/installation.rst` & `gurobi_optimods-1.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/license.rst` & `gurobi_optimods-1.0.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/usage.rst` & `gurobi_optimods-1.0.0/docs/source/usage.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Usage
 =====
 
-The best way to get started with the optimods is to try one out! Check out the
-:doc:`gallery` first to find a mod that suits you. Each mod comes complete with
+The best way to get started with the OptiMods is to try one out! Check out the
+:doc:`gallery` first to find a Mod that suits you. Each Mod comes complete with
 a page of explanatory documentation which provides background on the problem it
 is intended to solve. The docs also include runnable example codes and datasets
-to get you started.
+to help get you started.
 
-Note that you may need to install additional dependencies for some examples. The
-quick way to ensure you have a Python environment which can execute all the
-example snippets in the docs is to run the following::
+Note that you may need to install additional dependencies for some examples, as
+they use optional packages which are not direct dependencies of
+``gurobi-optimods``. The quick way to ensure you have a Python environment which
+can execute all the example snippets in the docs is to run the following::
 
    python -m pip install gurobi-optimods[examples]
 
-Each mod is designed to be self-contained, with a clean data-in data-out API.
+Each Mod is designed to be self-contained, with a clean data-in data-out API.
 Munge your data into the appropriate format using Python tools you already know,
-and run the mod as outlined in its documentation page to get back a solution.
+and run the Mod as outlined in its documentation page to get back a solution.
 
-The documentation pages also included details of the mathematical model
-underlying the mod, should you be interested to learn more about the
+The documentation pages also include details of the mathematical model
+underlying the Mod, should you be interested to learn more about the
 implementation. These details are explained in sections marked "Background". It
-is not necessary to read and understand these sections in order to use the mod
-effectively. You can also browse :ghsrc:`the mod source <src/gurobi_optimods>`
-to find out how the model is implemented in code.
+is not necessary to read and understand these sections in order to use the Mod
+effectively. You can also browse :ghsrc:`the Mod source <src/gurobi_optimods>`
+to find out how the mathematical models are implemented in code.
 
-Finally, we welcome contributions of new mods, bug fixes and new features for
-existing mods, and improvements to the documentation. This is intended to be a
+Finally, we welcome contributions of new Mods, bug fixes and new features for
+existing Mods, and improvements to the documentation. This is intended to be a
 community project that grows over time to handle a wide range of optimization
-use-cases across a different fields. See :doc:`contributing` for more details.
+use-cases across many different fields. See :doc:`contributing` for more
+details.
```

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/bipartite-matching.rst` & `gurobi_optimods-1.0.0/docs/source/mods/bipartite-matching.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Maximum Bipartite Matching
 ==========================
 
-The maximum matching problem is a fundamental problem in graph theory (ref).
-Given a graph, as a set of nodes connected to one another by edges, a matching
+The maximum matching problem is a fundamental problem in graph theory. Given
+a graph, as a set of nodes connected to one another by edges, a matching
 is any subset of those edges which have no vertex in common. The goal of
 maximum matching is to find the largest possible such matching of a given
 graph.
 
 In this mod we consider the special case of maximum cardinality matching on
 bipartite graphs. This problem can be applied to solve exclusive assignment
 problems in practice, such as the assignment of workers or resources to tasks.
@@ -65,15 +65,15 @@
 The ``maximum_bipartite_matching`` function supports scipy sparse arrays, pandas
 dataframes, and networkx graphs as possible inputs. The user must also provide
 the bipartite partitioning of the input graph. In all cases, the matching is
 returned as a sub-graph of the input data structure.
 
 .. tabs::
 
-    .. group-tab:: scipy
+    .. group-tab:: scipy.sparse
 
         When given a scipy sparse array representing the adjacency matrix of
         the graph, the user must also provide the two disjoint node sets as
         numpy arrays. The mod will return the adjacency matrix of the matching
         as a scipy sparse array.
 
         .. testcode:: bipartite_matching_sp
@@ -165,15 +165,15 @@
 using a network primal simplex algorithm.
 
 Solution
 --------
 
 .. tabs::
 
-    .. group-tab:: scipy
+    .. group-tab:: scipy.sparse
 
         The maximum matching is returned as a subgraph of the original bipartite
         graph, as a ``scipy.sparse`` array. Inspecting the result, it is clear that
         this is a maximum matching, since no two edges share a node in common, and
         all nodes in the second set are incident to an edge in the matching.
 
         .. doctest:: bipartite_matching_sp
```

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/lad-regression.rst` & `gurobi_optimods-1.0.0/docs/source/mods/lad-regression.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/min-cost-flow.rst` & `gurobi_optimods-1.0.0/docs/source/mods/min-cost-flow.rst`

 * *Files 6% similar despite different names*

```diff
@@ -77,56 +77,61 @@
 * NetworkX: using a ``nx.DiGraph`` or ``nx.Graph``;
 * SciPy.sparse: using some ``sp.sparray`` matrices and NumPy's ``np.ndarray``.
 
 An example of these inputs with their respective requirements is shown below.
 
 .. tabs::
 
-  .. group-tab:: pandas
+  .. group-tab:: scipy.sparse
 
-      .. doctest:: load_graph
+      .. doctest:: load_graph_scipy
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
-          >>> edge_data, node_data = datasets.load_graph()
-          >>> edge_data
-                         capacity  cost
-          source target
-          0      1              2     9
-                 2              2     7
-          1      3              1     1
-          2      3              1    10
-                 4              2     6
-          3      5              2     1
-          4      5              2     1
-          >>> node_data
-             demand
-          0      -2
-          1       0
-          2      -1
-          3       1
-          4       0
-          5       2
-
-      The ``edge_data`` DataFrame is indexed by ``source`` and ``target``
-      nodes and contains columns labelled ``capacity`` and ``cost`` with the
-      edge attributes.
-
-      The ``node_data`` DataFrame is indexed by node and contains columns
-      labelled ``demand``.
+          >>> G, capacities, cost, demands = datasets.simple_graph_scipy()
+          >>> G
+          <5x6 sparse matrix of type '<class 'numpy.int64'>'
+                  with 7 stored elements in COOrdinate format>
+          >>> print(G)
+            (0, 1)        1
+            (0, 2)        1
+            (1, 3)        1
+            (2, 3)        1
+            (2, 4)        1
+            (3, 5)        1
+            (4, 5)        1
+          >>> print(capacities)
+            (0, 1)        2
+            (0, 2)        2
+            (1, 3)        1
+            (2, 3)        1
+            (2, 4)        2
+            (3, 5)        2
+            (4, 5)        2
+          >>> print(cost)
+            (0, 1)        9
+            (0, 2)        7
+            (1, 3)        1
+            (2, 3)        10
+            (2, 4)        6
+            (3, 5)        1
+            (4, 5)        1
+          >>> print(demands)
+          [-2  0 -1  1  0  2]
 
-      We assume that nodes labels are integers from :math:`0,\dots,|V|-1`.
+      Three separate sparse matrices including the adjacency matrix, edge
+      capacity and cost, and a single array with the demands per node.
 
-  .. group-tab:: NetworkX
+  .. group-tab:: networkx
 
       .. doctest:: load_graph_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
-          >>> G = datasets.load_graph_networkx()
+          >>> G = datasets.simple_graph_networkx()
           >>> for e in G.edges(data=True):
           ...     print(e)
           ...
           (0, 1, {'capacity': 2, 'cost': 9})
           (0, 2, {'capacity': 2, 'cost': 7})
           (1, 3, {'capacity': 1, 'cost': 1})
           (2, 3, {'capacity': 1, 'cost': 10})
@@ -142,132 +147,124 @@
           (3, {'demand': 1})
           (4, {'demand': 0})
           (5, {'demand': 2})
 
       Edges have attributes ``capacity`` and ``cost`` and nodes have
       attributes ``demand``.
 
-  .. group-tab:: scipy.sparse
+  .. group-tab:: pandas
 
-      .. doctest:: load_graph_scipy
+      .. doctest:: load_graph
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
-          >>> G, capacities, cost, demands = datasets.load_graph_scipy()
-          >>> G
-          <5x6 sparse matrix of type '<class 'numpy.int64'>'
-                  with 7 stored elements in COOrdinate format>
-          >>> print(G)
-            (0, 1)        1
-            (0, 2)        1
-            (1, 3)        1
-            (2, 3)        1
-            (2, 4)        1
-            (3, 5)        1
-            (4, 5)        1
-          >>> print(capacities)
-            (0, 1)        2
-            (0, 2)        2
-            (1, 3)        1
-            (2, 3)        1
-            (2, 4)        2
-            (3, 5)        2
-            (4, 5)        2
-          >>> print(cost)
-            (0, 1)        9
-            (0, 2)        7
-            (1, 3)        1
-            (2, 3)        10
-            (2, 4)        6
-            (3, 5)        1
-            (4, 5)        1
-          >>> print(demands)
-          [-2  0 -1  1  0  2]
+          >>> edge_data, node_data = datasets.simple_graph_pandas()
+          >>> edge_data
+                         capacity  cost
+          source target
+          0      1              2     9
+                 2              2     7
+          1      3              1     1
+          2      3              1    10
+                 4              2     6
+          3      5              2     1
+          4      5              2     1
+          >>> node_data
+             demand
+          0      -2
+          1       0
+          2      -1
+          3       1
+          4       0
+          5       2
 
-      Three separate sparse matrices including the adjacency matrix, edge
-      capacity and cost, and a single array with the demands per node.
+      The ``edge_data`` DataFrame is indexed by ``source`` and ``target``
+      nodes and contains columns labelled ``capacity`` and ``cost`` with the
+      edge attributes.
 
-|
+      The ``node_data`` DataFrame is indexed by node and contains columns
+      labelled ``demand``.
+
+      We assume that nodes labels are integers from :math:`0,\dots,|V|-1`.
 
 Solution
 --------
 
 Depending on the input of choice, the solution also comes with different
 formats.
 
 .. tabs::
 
-  .. group-tab:: pandas
+  .. group-tab:: scipy.sparse
 
-      .. doctest:: min_cost_flow
+      .. doctest:: min_cost_flow_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
-          >>> from gurobi_optimods.min_cost_flow import min_cost_flow
-          >>> edge_data, node_data = datasets.load_graph()
-          >>> obj, sol = min_cost_flow(edge_data, node_data, verbose=False)
+          >>> from gurobi_optimods.min_cost_flow import min_cost_flow_scipy
+          >>> G, capacities, cost, demands = datasets.simple_graph_scipy()
+          >>> obj, sol = min_cost_flow_scipy(G, capacities, cost, demands, verbose=False)
           >>> obj
           31.0
           >>> sol
-          source  target
-          0       1         1.0
-                  2         1.0
-          1       3         1.0
-          2       3         0.0
-                  4         2.0
-          3       5         0.0
-          4       5         2.0
-          Name: flow, dtype: float64
-
-      The ``min_cost_flow`` function returns the cost of the solution as well
-      as ``pd.Series`` with the flow per edge. Similarly as the input
-      DataFrame the resulting series is indexed by ``source`` and ``target``.
+          <5x6 sparse matrix of type '<class 'numpy.float64'>'
+                  with 5 stored elements in COOrdinate format>
+          >>> print(sol)
+            (0, 1)        1.0
+            (0, 2)        1.0
+            (1, 3)        1.0
+            (2, 4)        2.0
+            (4, 5)        2.0
 
+      The ``min_cost_flow_scipy`` function returns the cost of the solution as
+      well as a ``sp.sparray`` with the edges where the data is the amount of
+      non-zero flow in the solution.
 
-  .. group-tab:: NetworkX
+  .. group-tab:: networkx
 
       .. doctest:: min_cost_flow_networkx
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
           >>> from gurobi_optimods.min_cost_flow import min_cost_flow_networkx
-          >>> G = datasets.load_graph_networkx()
+          >>> G = datasets.simple_graph_networkx()
           >>> obj, sol = min_cost_flow_networkx(G, verbose=False)
           >>> obj
           31.0
           >>> list(sol.edges(data=True))
           [(0, 1, {'flow': 1.0}), (0, 2, {'flow': 1.0}), (1, 3, {'flow': 1.0}), (2, 4, {'flow': 2.0}), (4, 5, {'flow': 2.0})]
 
       The ``min_cost_flow_networkx`` function returns the cost of the solution
       as well as a dictionary indexed by edge with the non-zero flow.
 
-  .. group-tab:: scipy.sparse
+  .. group-tab:: pandas
 
-      .. doctest:: min_cost_flow_networkx
+      .. doctest:: min_cost_flow
           :options: +NORMALIZE_WHITESPACE
 
           >>> from gurobi_optimods import datasets
-          >>> from gurobi_optimods.min_cost_flow import min_cost_flow_scipy
-          >>> G, capacities, cost, demands = datasets.load_graph_scipy()
-          >>> obj, sol = min_cost_flow_scipy(G, capacities, cost, demands, verbose=False)
+          >>> from gurobi_optimods.min_cost_flow import min_cost_flow_pandas
+          >>> edge_data, node_data = datasets.simple_graph_pandas()
+          >>> obj, sol = min_cost_flow_pandas(edge_data, node_data, verbose=False)
           >>> obj
           31.0
           >>> sol
-          <5x6 sparse matrix of type '<class 'numpy.float64'>'
-                  with 5 stored elements in COOrdinate format>
-          >>> print(sol)
-            (0, 1)        1.0
-            (0, 2)        1.0
-            (1, 3)        1.0
-            (2, 4)        2.0
-            (4, 5)        2.0
+          source  target
+          0       1         1.0
+                  2         1.0
+          1       3         1.0
+          2       3         0.0
+                  4         2.0
+          3       5         0.0
+          4       5         2.0
+          Name: flow, dtype: float64
 
-      The ``min_cost_flow_scipy`` function returns the cost of the solution as
-      well as a ``sp.sparray`` with the edges where the data is the amount of
-      non-zero flow in the solution.
+      The ``min_cost_flow_pandas`` function returns the cost of the solution as well
+      as ``pd.Series`` with the flow per edge. Similarly as the input
+      DataFrame the resulting series is indexed by ``source`` and ``target``.
 
 The solution for this example is shown in the figure below. The edge labels
 denote the edge capacity, cost and resulting flow: :math:`(B_{ij}, c_{ij},
 x^*_{ij})`. Edges with non-zero flow are highlighted in red. Also the demand for
 each vertex is shown on top of the vertex in red.
 
 .. image:: figures/min-cost-flow-result.png
```

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/mwis.rst` & `gurobi_optimods-1.0.0/docs/source/mods/mwis.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/portfolio.rst` & `gurobi_optimods-1.0.0/docs/source/mods/portfolio.rst`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,17 @@
     ...
     Presolved: 1 rows, 10 columns, 10 nonzeros
     ...
 
 Solution
 --------
 
-The return value of the ``efficient_portfolio`` method is a data class instance
-containing information on the computed portfolio.  It has the following
-attributes:
+The method ``efficient_portfolio`` returns a
+:class:`~gurobi_optimods.portfolio.PortfolioResult` instance, containing
+information on the computed portfolio.  It has the following attributes:
 
 * ``x`` : The relative investments :math:`x` for each asset
 * ``ret`` : The estimated return :math:`\mu^T x`
 * ``risk`` : The estimated risk :math:`x^T \Sigma x`
 
 In this example the solution suggests to spread the investments over five
 positions (AA, DD, GG, HH, II).  The other allocations are negligible.
@@ -177,54 +177,64 @@
 .. _factor models:
 
 Using factor models as input
 ----------------------------
 
 In the preceding discussion we have assumed that we the covariance matrix
 :math:`\Sigma` was explicitly given.  In many cases, however, the covariance is
-naturally given through a *factor model*.  Mathematically this means that a
+naturally given through a *factor model*.  Mathematically, this means that a
 decomposition
 
 .. math::
 
     \begin{align*}
-    \Sigma = F_1 F_1^T + F_2 F_2^T + \cdots + F_l F_l^T
+    \Sigma = B K B^T + \mbox{diag}(d)
     \end{align*}
 
-is known.  Examples for this are single- or multi-factor models that divide the
-individual covariances into a general market movement, and an idiosyncratic
-risk component for each asset.  See `Efficient frontier(s) with cardinality
-constraints`_ for an example.
-
-Rather than computing the covariance matrix explcitly from the decomposition,
-it is adivised to input the individual factor matrices directly through the
-``cov_factors`` keyword argurment as in the following example, which mimicks a
-single-factor model:
+of the covariance matrix is known where
+
+* :math:`B` is an :math:`n`-by-:math:`k` matrix of factor exposures (or "betas" or "factor
+  loadings"),
+* :math:`K` is the :math:`k`-by-:math:`k` covariance matrix of the factor return rates,
+* :math:`d` is the vector of idiosyncratic risk for each asset,
+
+and :math:`\mbox{diag}(d)` denotes the :math:`n`-by-:math:`n` diagonal matrix having diagonal values
+:math:`d`.
+
+Examples for this are single- or multi-factor models that divide the individual
+covariances into a general market movement, and an idiosyncratic risk component
+for each asset.  Also CAPM priors and risk factors obtained from principal
+component analysis can be phrased in this form. See `Efficient frontier(s) with
+cardinality constraints`_ for an example of a synthetic multi-factor model.
+
+Rather than computing the covariance matrix explicitly from the decomposition,
+it is adivised for performance and accuracy reasons to input the individual
+factor matrices directly through the ``cov_factors`` keyword argurment as in
+the following example, which mimics a single-factor model:
 
 .. testcode:: mod
 
     import numpy as np
     from gurobi_optimods.portfolio import MeanVariancePortfolio
 
     mu = np.array([0.23987036, 0.24402181, 0.15069203])
     market_variance = 0.25
     # Factors relating market variance to assets
     beta = np.array([[0.93797928], [1.71942161], [1.15652896]])
     # Idiosyncratic risk
-    asset_risk = np.array([0.23745675, 0.19140259, 0.34325066])
+    asset_risk = np.array([0.23745675, 0.19140259, 0.34325066])**2
 
     # Full covariance matrix according to single factor model
-    Sigma = beta @ beta.T * market_variance**2 + np.diag(asset_risk**2)
+    Sigma = beta @ beta.T * market_variance**2 + np.diag(asset_risk)
     mvp_matrix = MeanVariancePortfolio(mu, cov_matrix=Sigma)
     x_matrix = mvp_matrix.efficient_portfolio(20).x
 
-    # Better use known factorization
-    F1 = beta * market_variance
-    F2 = np.diag(asset_risk)
-    mvp_factors = MeanVariancePortfolio(mu, cov_factors=(F1, F2))
+    # Same model, but taking advantage of the factor structure
+    mvp_factors = MeanVariancePortfolio(mu, cov_factors=(
+        beta, market_variance**2 * np.eye(1), asset_risk))
     x_factors = mvp_factors.efficient_portfolio(20).x
 
 .. testoutput:: mod
     :hide:
 
     ...
     Optimize a model with 26 rows, 28 columns and 57 nonzeros
@@ -743,15 +753,15 @@
 :footcite:t:`cornuéjols_peña_tütüncü_2018`, Sect. 6.6.  The important effect on the input
 data for the mean-variance model we want to point out though is that the
 covariance matrix decomposes algebraically as follows:
 
 .. math::
 
     \begin{equation*}
-      \Sigma = F F^T + \mbox{cov}(u)
+      \Sigma = B K B^T + \mbox{cov}(u)
     \end{equation*}
 
 That is, :math:`\Sigma` is given by the sum of a low-rank term and a diagonal
 term; we will take advantage of this structure further below.  The following
 code snippet generates synthetic data based on a multiple-factor model
 incorporating this particular structure:
 
@@ -760,47 +770,45 @@
     import numpy as np
     np.random.seed(0xacac)  # Fix seed for reproducibility
 
     num_assets = 16
     num_factors = 4
     timesteps = 24
 
-    # Generate random factor model parameters
-    sigma_factor = np.diag(np.sqrt(1 + np.arange(num_factors) + np.random.rand(num_factors)))
+    # Generate random factor model, risk is B * sigma_factor * B.T + cov(u)
+    sigma_factor = np.diag(1 + np.arange(num_factors) + np.random.rand(num_factors))
     B = np.random.normal(size=(num_assets, num_factors))
     alpha = np.random.normal(loc=1, size=(num_assets, 1))
     u = np.random.multivariate_normal(np.zeros(num_assets), np.eye(num_assets), timesteps).T
+    risk_specific = np.diag(np.cov(u))
 
     # Time series in factor space
-    TS_factor = np.random.multivariate_normal(np.zeros(num_factors), sigma_factor**2, timesteps).T
+    TS_factor = np.random.multivariate_normal(np.zeros(num_factors), sigma_factor, timesteps).T
 
     # Estimate mu from time series in full space
     mu = np.mean(alpha + B @ TS_factor + u, axis=1)
 
-    # Final covariance data
-    F = B @ sigma_factor
-    risk_specific = np.diag(np.sqrt(np.diag(np.cov(u))))
-
-Note that the matrices ``F`` and ``risk_specific`` are already in the format for the
-optimization model as described in `Using factor models as input`_.
+Note that ``B``, ``sigma_factor`` and ``risk_specific`` are already in the
+format for the optimization model as described in `Using factor models as
+input`_.
 
 Computing frontiers
 ~~~~~~~~~~~~~~~~~~~
 
 To compute the efficient frontier(s), we simple range over a series of values
 for :math:`\gamma` and compute various optimal portfolios with different
 cardinality constraints::
 
     from gurobi_optimods.portfolio import MeanVariancePortfolio
     gammas = np.logspace(-1, 1, 256)**2
     rr_pairs_unc = []
     rr_pairs_con = {1: [], 2: [], 3: []}
 
     for g in gammas:
-        mvp = MeanVariancePortfolio(mu, cov_factors=(F, risk_specific))
+        mvp = MeanVariancePortfolio(mu, cov_factors=(B, sigma_factor, risk_specific))
         # Optimal portfolio w/o cardinality constraints
         pf = mvp.efficient_portfolio(g, verbose=False)
         rr_pairs_unc.append((pf.risk, pf.ret))
         for max_positions in [1, 2, 3]:
             # Optimal portfolio with cardinality constraints
             pf = mvp.efficient_portfolio(g, max_positions=max_positions, verbose=False)
             rr_pairs_con[max_positions].append((pf.risk, pf.ret))
```

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/qubo.rst` & `gurobi_optimods-1.0.0/docs/source/mods/qubo.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/workforce.rst` & `gurobi_optimods-1.0.0/docs/source/mods/workforce.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-example.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-example.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-figs.py` & `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-figs.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-flow.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-flow.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/bipartite-matching-result.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/bipartite-matching-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-coeffs.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-outlier-errors.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-outlier-errors.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/lad-regression-coeffs.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/lad-regression-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/min-cost-flow-result.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/min-cost-flow-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/mvp.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/mvp.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/mwis.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/mwis.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/pie.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/pie.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/qubo.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/qubo.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/figures/shortest-path-result.png` & `gurobi_optimods-1.0.0/docs/source/mods/figures/shortest-path-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/mods/icons/lad-regression.png` & `gurobi_optimods-1.0.0/docs/source/mods/icons/lad-regression.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/refs/graphs.bib` & `gurobi_optimods-1.0.0/docs/source/refs/graphs.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/docs/source/refs/qubo.bib` & `gurobi_optimods-1.0.0/docs/source/refs/qubo.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/bipartite_matching.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/bipartite_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Bipartite Matching
 ------------------
 """
 
 
 import logging
-from typing import List, overload
 
 import gurobipy as gp
 import gurobipy_pandas as gppd
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 from gurobipy import GRB
@@ -20,65 +19,38 @@
     nx = None
 
 from gurobi_optimods.utils import optimod
 
 logger = logging.getLogger(__name__)
 
 
-@overload
-def maximum_bipartite_matching(
-    graph: sp.spmatrix,
-    nodes1: np.ndarray,
-    nodes2: np.ndarray,
-) -> sp.spmatrix:
-    ...
-
-
-@overload
-def maximum_bipartite_matching(
-    graph: pd.DataFrame,
-    nodes1: str,
-    nodes2: str,
-) -> pd.DataFrame:
-    ...
-
-
-if nx is not None:
-
-    @overload
-    def maximum_bipartite_matching(
-        graph: nx.Graph,
-        nodes1: List,
-        nodes2: List,
-    ) -> nx.Graph:
-        ...
-
-
 @optimod()
 def maximum_bipartite_matching(graph, nodes1, nodes2, *, create_env):
     """Solve a maximum cardinality bipartite matching problem on the
     given graph.
 
     Parameters
     ----------
     graph : spmatrix or Graph or DataFrame
         A graph, specified either as a scipy.sparse adjacency matrix, networkx
         graph, or pandas dataframe.
     nodes1 : ndarray or str
-        Nodes in the first bipartite set. If ``graph`` is a pandas dataframe,
-        nodes1 must be a column name. Otherwise, it is a numpy array of nodes in
-        the first bipartite set.
+        Nodes in the first bipartite set. If ``graph`` is a scipy sparse matrix,
+        ``nodes1`` must be a numpy array. If ``graph`` is a pandas dataframe,
+        ``nodes1`` must be a column name. If ``graph`` is a networkx graph,
+        ``nodes1`` must be a list.
     nodes2 : ndarray or str
-        Nodes in the second bipartite set. If ``graph`` is a pandas dataframe,
-        nodes2 must be a column name. Otherwise, it is a numpy array of nodes in
-        the second bipartite set.
+        Nodes in the first bipartite set. If ``graph`` is a scipy sparse matrix,
+        ``nodes2`` must be a numpy array. If ``graph`` is a pandas dataframe,
+        ``nodes2`` must be a column name. If ``graph`` is a networkx graph,
+        ``nodes2`` must be a list.
 
     Returns
     -------
-    DataFrame or Graph
+    spmatrix or Graph or DataFrame
         A subgraph of the original ``graph`` (with the same data type) specifying
         the maximum matching
     """
     if isinstance(graph, sp.spmatrix):
         return _maximum_bipartite_matching_scipy(graph, nodes1, nodes2, create_env)
     elif isinstance(graph, pd.DataFrame):
         return _maximum_bipartite_matching_pandas(graph, nodes1, nodes2, create_env)
```

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/datasets.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,61 +37,52 @@
         ),
         worker_limits=pd.read_csv(
             DATA_FILE_DIR / "workforce/worker_limits.csv",
         ),
     )
 
 
-def load_graph(drop_pos=True, capacity=True, cost=True, demand=True):
-    edge_data = pd.read_csv(DATA_FILE_DIR / "graphs/edge_data1.csv").set_index(
+def _load_simple_graph_pandas(drop_pos=True, capacity=True, cost=True, demand=True):
+    edge_data = pd.read_csv(DATA_FILE_DIR / "graphs/simple_graph_edges.csv").set_index(
         ["source", "target"]
     )
-    node_data = pd.read_csv(DATA_FILE_DIR / "graphs/node_data1.csv", index_col=0)
+    node_data = pd.read_csv(
+        DATA_FILE_DIR / "graphs/simple_graph_nodes.csv", index_col=0
+    )
     if drop_pos:
         node_data.drop(columns=["posx", "posy"], inplace=True)
     if not capacity:
         edge_data.drop(columns=["capacity"], inplace=True)
     if not cost:
         edge_data.drop(columns=["cost"], inplace=True)
     if not demand:
         node_data.drop(columns=["demand"], inplace=True)
     return edge_data, node_data
 
 
-def load_graph_networkx(capacity=True, cost=True, demand=True):
-    edge_data, node_data = load_graph(capacity=capacity, cost=cost, demand=demand)
-    return _convert_pandas_to_digraph(
-        edge_data, node_data, capacity=capacity, cost=cost, demand=demand
-    )
+def simple_graph_pandas():
+    return _load_simple_graph_pandas(capacity=True, cost=True, demand=True)
 
 
-def load_graph_scipy(capacity=True, cost=True, demand=True):
-    edge_data, node_data = load_graph(capacity=capacity, cost=cost, demand=demand)
-    return _convert_pandas_to_scipy(
-        edge_data, node_data, capacity=capacity, cost=cost, demand=demand
+def simple_graph_networkx():
+    edge_data, node_data = _load_simple_graph_pandas(
+        capacity=True, cost=True, demand=True
     )
-
-
-def load_graph2():
-    return (
-        pd.read_csv(DATA_FILE_DIR / "graphs/edge_data2.csv").set_index(
-            ["source", "target"]
-        ),
-        pd.read_csv(DATA_FILE_DIR / "graphs/node_data2.csv", index_col=0),
+    return _convert_pandas_to_digraph(
+        edge_data, node_data, capacity=True, cost=True, demand=True
     )
 
 
-def load_graph2_networkx():
-    edge_data, node_data = load_graph2()
-    return _convert_pandas_to_digraph(edge_data, node_data)
-
-
-def load_graph2_scipy():
-    edge_data, node_data = load_graph2()
-    return _convert_pandas_to_scipy(edge_data, node_data)
+def simple_graph_scipy(capacity=True, cost=True, demand=True):
+    edge_data, node_data = _load_simple_graph_pandas(
+        capacity=True, cost=True, demand=True
+    )
+    return _convert_pandas_to_scipy(
+        edge_data, node_data, capacity=True, cost=True, demand=True
+    )
 
 
 def load_portfolio():
     fn = DATA_FILE_DIR / "portfolio/portfolio.csv"
     return pd.read_csv(fn, index_col=0)
```

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/min_cost_flow.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/min_cost_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
 from gurobi_optimods.utils import optimod
 
 logger = logging.getLogger(__name__)
 
 
 @optimod()
-def min_cost_flow(arc_data: pd.DataFrame, demand_data: pd.DataFrame, *, create_env):
+def min_cost_flow_pandas(
+    arc_data: pd.DataFrame, demand_data: pd.DataFrame, *, create_env
+):
     """Solve the minimum cost flow problem for a given graph.
 
     The inputs adhere to the following structure::
 
         arc_data = pd.DataFrame(
             [
                 {"from": 0, "to": 1, "capacity": 16, "cost": 0}, {"from": 1,
```

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/mwis.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/portfolio.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/portfolio.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,56 +25,66 @@
     Parameters
     ----------
     mu : 1-d ndarray
         Vector of expected returns for each asset
     cov_matrix : 2-d ndarray
         Covariance matrix :math:`\Sigma`
     cov_factors : tuple of ndarray
-        Covariance factors that constitute :math:`\Sigma`. Typically each
-        element ``F`` of ``cov_matrix`` will either be a
+        Covariance factors that constitute :math:`\Sigma = B K B^T + diag(d)`.
 
-            * n-by-k dense matrix, or a
-            * n-by-n diagonal matrix.
-
-        Each element ``F`` of ``cov_factors`` contributes the term ``F @ F.T``
-        to :math:`\Sigma`; see also :ref:`factor models`
+            * ``cov_factors[0]``: (n, k) ndarray :math:`B`
+            * ``cov_factors[1]``: (k, k) ndarray :math:`K`, SPD
+            * ``cov_factors[2]``: (n,) ndarray :math:`d`, nonnegative
+
+    Raises
+    ------
+    LinAlgError
+        If the matrix K is not positive definite
 
     """
 
     def __init__(
         self,
         mu,
         cov_matrix=None,
         cov_factors=None,
     ):
         if cov_matrix is not None and cov_factors is not None:
             raise TypeError("Both cov_matrix and cov_factors given")
 
         if cov_matrix is not None:
             if isinstance(cov_matrix, pd.DataFrame):
-                self.resultType = "pandas"
-                self.index = cov_matrix.index
-                self.covariance = cov_matrix.to_numpy()
+                self._result_type = "pandas"
+                self._index = cov_matrix.index
+                self._covariance = cov_matrix.to_numpy()
             elif isinstance(cov_matrix, np.ndarray):
-                self.covariance = cov_matrix
-                self.resultType = "numpy"
+                self._covariance = cov_matrix
+                self._result_type = "numpy"
             else:
                 raise TypeError("Incompatible type of cov_matrix")
         elif cov_factors is not None:
-            self.covariance = cov_factors
-            self.index = None
+            # Given: (B, K, d) such that Sigma = B @ K @ B.T + diag(d)
+            # Internally we store (F, sqrt(d)) with F = B @ chol(K) so that
+            # Sigma = F @ F.T + diag(d)
+            #
+            # As part of the transformation it is checked whether K is SPD,
+            # and we let a possible error from chol propagate.
+            B, K, d = cov_factors
+            F = B @ np.linalg.cholesky(K)
+            self._covariance = (F, np.sqrt(d))
+            self._index = None
         else:
             raise TypeError("No covariace data given")
 
         if isinstance(mu, pd.Series):
-            self.resultType = "pandas"
-            self.mu = mu.to_numpy()
+            self._result_type = "pandas"
+            self._mu = mu.to_numpy()
         elif isinstance(mu, np.ndarray):
-            self.mu = mu
-            self.resultType = "numpy"
+            self._mu = mu
+            self._result_type = "numpy"
         else:
             raise TypeError("Incompatible type of mu")
 
     @optimod()
     def efficient_portfolio(
         self,
         gamma,
@@ -161,15 +171,15 @@
         costs_sell = self._homogenize_input(costs_sell)
         initial_holdings = self._homogenize_input(initial_holdings)
 
         if initial_holdings is not None:
             if initial_holdings.sum() > 1.0:
                 raise ValueError("Initial holding's sum must not exceed 1.0")
         else:
-            initial_holdings = np.zeros(self.mu.shape)
+            initial_holdings = np.zeros(self._mu.shape)
 
         with create_env() as env, gp.Model("efficient_portfolio", env=env) as m:
             x, x_rf = self._populate_model(
                 m,
                 gamma,
                 max_trades,
                 max_positions,
@@ -252,32 +262,32 @@
         #    x_sell >=0 (relative sell)
         #    b_long \in {0,1} (indicator variable for x_long)
         #    b_short \in {0,1} (indicator variable for x_short)
         #    b_buy \in {0,1} (indicator variable for x_buy)
         #    b_sell \in {0,1} (indicator variable for x_sell)
 
         # Portfolio vector x is split into long and short positions
-        x = m.addMVar(shape=self.mu.shape, lb=-float("inf"), name="x")
-        x_long = m.addMVar(shape=self.mu.shape, name="x_long")
-        x_short = m.addMVar(shape=self.mu.shape, name="x_short")
+        x = m.addMVar(shape=self._mu.shape, lb=-float("inf"), name="x")
+        x_long = m.addMVar(shape=self._mu.shape, name="x_long")
+        x_short = m.addMVar(shape=self._mu.shape, name="x_short")
         m.addConstr(x == x_long - x_short)
 
         # Dummy variable for investment in risk-free asset,
         x_rf = m.addVar(lb=0.0, ub=0.0, name="x_rf")
 
-        x_buy = m.addMVar(shape=self.mu.shape, name="x_buy")
-        x_sell = m.addMVar(shape=self.mu.shape, name="x_sell")
+        x_buy = m.addMVar(shape=self._mu.shape, name="x_buy")
+        x_sell = m.addMVar(shape=self._mu.shape, name="x_sell")
         m.addConstr(x - initial_holdings == x_buy - x_sell)
 
         # Binaries used to enforce VUB and minimum position/trade size
-        b_long = m.addMVar(shape=self.mu.shape, vtype="B", name="position_long")
-        b_short = m.addMVar(shape=self.mu.shape, vtype="B", name="position_short")
+        b_long = m.addMVar(shape=self._mu.shape, vtype="B", name="position_long")
+        b_short = m.addMVar(shape=self._mu.shape, vtype="B", name="position_short")
 
-        b_buy = m.addMVar(shape=self.mu.shape, vtype="B", name="trade_buy")
-        b_sell = m.addMVar(shape=self.mu.shape, vtype="B", name="trade_sell")
+        b_buy = m.addMVar(shape=self._mu.shape, vtype="B", name="trade_buy")
+        b_sell = m.addMVar(shape=self._mu.shape, vtype="B", name="trade_sell")
 
         m.update()
 
         # Define VUB constraints for x_long and x_short.
         #
         # Going short by alpha means that each long position is upper
         # bounded by 1 + alpha, and each short position by alpha.
@@ -323,79 +333,78 @@
             m.addConstr(x_buy >= min_long * b_buy, name="min_buy")
 
         if min_short is not None:
             m.addConstr(x_sell >= min_short * b_sell, name="min_sell")
 
         m.addConstr(investment == 1, name="fully_invested")
 
-        if not isinstance(self.covariance, tuple):
+        if not isinstance(self._covariance, tuple):
             # Basic mean-variance weighted objective
-            objexpr = self.mu @ x - 0.5 * gamma * x @ self.covariance @ x
+            objexpr = self._mu @ x - 0.5 * gamma * x @ self._covariance @ x
         else:
-            # Idea:   We have given  Sigma =
-            #
-            #   factors[0] @ factors[0].T + ... + factors[l] @ factors[l].T
-            #   =: F_0 @ F_0.T + ... + F_l @ F_l
-            #
-            # so that for each contributing term we can set
-            #
-            #   (x.T @ F_i) @ (F_i.T @ x) =: y_i @ y_i
-            #
-            # giving
-            #
-            #   min \sum_i gamma * y_i @ y_i
-            #   s.t. y_i = F_i.T @ x  for all i
+            F, sqrt_d = self._covariance
+            # We have given Sigma = F @ F.T + diag(sqrt_d) @ diag(sqrt_d)
+            # Auxiliary variables y_F, y_d:
+            #   F.T @ x = y_F
+            #   sqrt_d * x = y_d
+
+            objexpr = self._mu @ x
+
+            y_F = m.addMVar(F.shape[1], lb=-float("inf"), name=f"yF")
+            m.addConstr(F.T @ x == y_F, name=f"link_yF_x")
 
-            objexpr = self.mu @ x
+            y_d = m.addMVar(self._mu.size, lb=-float("inf"), name=f"yd")
+            m.addConstr(sqrt_d * x == y_d, name=f"link_yd_x")
 
-            for idx, F in enumerate(self.covariance):
-                y = m.addMVar(F.shape[1], lb=-float("inf"), name=f"factor{idx:d}")
-                m.addConstr(F.T @ x == y, name=f"link_factor{idx:d}_x")
-                objexpr -= 0.5 * gamma * y @ y
+            objexpr -= 0.5 * gamma * (y_F @ y_F + y_d @ y_d)
 
         if rf_return is not None:
             objexpr += rf_return * x_rf
 
         m.setObjective(objexpr, GRB.MAXIMIZE)
         return (x, x_rf)
 
     def _construct_result(self, x, x_rf, rf_return):
-        if self.resultType == "numpy":
+        if self._result_type == "numpy":
             pass
-        elif self.resultType == "pandas":
-            x = pd.Series(x, index=self.index)
+        elif self._result_type == "pandas":
+            x = pd.Series(x, index=self._index)
         else:
             assert False
 
-        ret = self.mu @ x
+        ret = self._mu @ x
 
-        if not isinstance(self.covariance, tuple):
-            risk = x @ self.covariance @ x
+        if not isinstance(self._covariance, tuple):
+            risk = x @ self._covariance @ x
         else:
+            F, sqrt_d = self._covariance
             risk = 0.0
-            for F in self.covariance:
-                y = x @ F
-                risk += y @ y
+
+            y = x @ F
+            risk += y @ y
+
+            y = x * sqrt_d
+            risk += y @ y
 
         if rf_return is not None:
             x_rf = x_rf
             ret += rf_return * x_rf
         else:
             x_rf = None
 
         return PortfolioResult(x, ret, risk, x_rf)
 
     def _homogenize_input(self, input_data):
         # Check and unpack if input_data is a Series
         if isinstance(input_data, pd.Series):
-            if self.index is not None:
-                if any(self.index != input_data.index):
+            if self._index is not None:
+                if any(self._index != input_data.index):
                     raise ValueError("Misaligned Series indexes: " + input_data.index)
             else:
-                self.index = input_data.index
+                self._index = input_data.index
             input_data = input_data.to_numpy()
 
         return input_data
 
 
 @dataclass
 class PortfolioResult:
```

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/qubo.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/qubo.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/regression.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/utils.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-# One possible idea for handling output suppression/file logging. Mods need
-# to be decorated with @optimod and accept a create_env keyword argument. This
-# factory function should be used to create the mod's gurobi environments.
-#
-#   @optimod(mod_logger=logger)  # pass the mod's module logger
-#   def my_mod(inputs, *, create_env):
-#       with create_env() as env, gp.Model(env=env) as model:
-#           # do stuff with model
-#
-# The mod then gets two arguments for free: `verbose`, where `verbose=False`
-# suppresses all output, and logfile=<file-path>, which creates a log file
-# including logger output from the mod and gurobi output.
-#
-# Note that this won't handle multi-threaded stuff well (context manipulates
-# global logger handlers). But it's simpler to implement in the mods than
-# passing some funky log collecting object around.
+"""
+Mods must be decorated with @optimod and accept a create_env keyword argument.
+This factory function should be used to create the mod's gurobi environments::
+
+   @optimod()
+   my_mod(inputs, *, create_env):
+       with create_env() as env, gp.Model(env=env) as model:
+           # formulate and solve model
+
+The mod then gets some arguments for free:
+
+- `verbose`, where `verbose=False` suppresses all output;
+- logfile=<file-path>, which writes output to a log file; and
+- solver_params, which the Mod caller can use to pass parameters to Gurobi.
+
+Parameters can also be passed as a dictionary to create_env if the Mod requires
+some specific settings.
+
+Note that this captures output via the gurobipy and optimod python loggers. It
+may not work as expected when multithreading in Python.
+"""
 
 import functools
 import logging
 import re
 import sys
 from contextlib import contextmanager
 from typing import Dict, Optional
```

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/workforce.py` & `gurobi_optimods-1.0.0/src/gurobi_optimods/workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/data/portfolio/portfolio.csv` & `gurobi_optimods-1.0.0/src/gurobi_optimods/data/portfolio/portfolio.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/src/gurobi_optimods/data/workforce/preferences.csv` & `gurobi_optimods-1.0.0/src/gurobi_optimods/data/workforce/preferences.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_bipartite_matching.py` & `gurobi_optimods-1.0.0/tests/test_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_graph_utils.py` & `gurobi_optimods-1.0.0/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_min_cost_flow.py` & `gurobi_optimods-1.0.0/tests/test_min_cost_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import unittest
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 
 try:
@@ -14,34 +15,73 @@
 
 from .test_graph_utils import (
     check_solution_networkx,
     check_solution_pandas,
     check_solution_scipy,
 )
 
+edge_data2 = """
+source,target,capacity,cost
+0,1,15,4
+0,2,8,4
+1,3,4,2
+1,2,20,2
+1,4,10,6
+2,3,15,1
+2,4,5,3
+3,4,20,2
+"""
+
+
+node_data2 = """
+,demand
+0,-20
+1,0
+2,0
+3,5
+4,15
+"""
+
+
+def load_graph2_pandas():
+    return (
+        pd.read_csv(io.StringIO(edge_data2)).set_index(["source", "target"]),
+        pd.read_csv(io.StringIO(node_data2), index_col=0),
+    )
+
+
+def load_graph2_networkx():
+    edge_data, node_data = load_graph2_pandas()
+    return datasets._convert_pandas_to_digraph(edge_data, node_data)
+
+
+def load_graph2_scipy():
+    edge_data, node_data = load_graph2_pandas()
+    return datasets._convert_pandas_to_scipy(edge_data, node_data)
+
 
 class TestMinCostFlow(unittest.TestCase):
     def test_pandas(self):
-        edge_data, node_data = datasets.load_graph()
-        cost, sol = mcf.min_cost_flow(edge_data, node_data)
+        edge_data, node_data = datasets.simple_graph_pandas()
+        cost, sol = mcf.min_cost_flow_pandas(edge_data, node_data)
         sol = sol[sol > 0]
         self.assertEqual(cost, 31)
         candidate = {(0, 1): 1.0, (0, 2): 1.0, (1, 3): 1.0, (2, 4): 2.0, (4, 5): 2.0}
         self.assertIsInstance(sol, pd.Series)
         self.assertTrue(check_solution_pandas(sol, [candidate]))
 
     def test_infeasible(self):
-        edge_data, node_data = datasets.load_graph()
+        edge_data, node_data = datasets.simple_graph_pandas()
         # Add a node requesting more flow than is available.
         node_data["demand"].values[-1] = 10.0
         with self.assertRaisesRegex(ValueError, "Unsatisfiable flows"):
-            obj, sol = mcf.min_cost_flow(edge_data, node_data)
+            obj, sol = mcf.min_cost_flow_pandas(edge_data, node_data)
 
     def test_scipy(self):
-        G, cap, cost, demands = datasets.load_graph_scipy()
+        G, cap, cost, demands = datasets.simple_graph_scipy()
         cost, sol = mcf.min_cost_flow_scipy(G, cap, cost, demands)
         self.assertEqual(cost, 31)
         candidate = np.array(
             [
                 [0.0, 1.0, 1.0, 0.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
                 [0.0, 0.0, 0.0, 0.0, 2.0, 0.0],
@@ -50,30 +90,30 @@
             ]
         )
         self.assertIsInstance(sol, sp.spmatrix)
         self.assertTrue(check_solution_scipy(sol, [candidate]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx(self):
-        G = datasets.load_graph_networkx()
+        G = datasets.simple_graph_networkx()
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 31)
         expected = {
             (0, 1): {"flow": 1.0},
             (0, 2): {"flow": 1.0},
             (1, 3): {"flow": 1.0},
             (2, 4): {"flow": 2.0},
             (4, 5): {"flow": 2.0},
         }
         self.assertIsInstance(sol, nx.Graph)
         self.assertTrue(check_solution_networkx(sol, [expected]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx_renamed(self):
-        G = datasets.load_graph_networkx()
+        G = datasets.simple_graph_networkx()
         G = nx.relabel_nodes(G, {0: "s", 5: "t"})
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 31)
         expected = {
             ("s", 1): {"flow": 1.0},
             ("s", 2): {"flow": 1.0},
             (1, 3): {"flow": 1.0},
@@ -82,16 +122,16 @@
         }
         self.assertIsInstance(sol, nx.Graph)
         self.assertTrue(check_solution_networkx(sol, [expected]))
 
 
 class TestMinCostFlow2(unittest.TestCase):
     def test_pandas(self):
-        edge_data, node_data = datasets.load_graph2()
-        cost, sol = mcf.min_cost_flow(edge_data, node_data)
+        edge_data, node_data = load_graph2_pandas()
+        cost, sol = mcf.min_cost_flow_pandas(edge_data, node_data)
         sol = sol[sol > 0]
         self.assertEqual(cost, 150)
         candidate = {
             (0, 1): 12.0,
             (0, 2): 8.0,
             (1, 3): 4.0,
             (1, 2): 8.0,
@@ -107,30 +147,30 @@
             (2, 3): 11.0,
             (2, 4): 5.0,
             (3, 4): 10.0,
         }
         self.assertTrue(check_solution_pandas(sol, [candidate, candidate2]))
 
     def test_scipy(self):
-        G, cap, cost, demands = datasets.load_graph2_scipy()
+        G, cap, cost, demands = load_graph2_scipy()
         cost, sol = mcf.min_cost_flow_scipy(G, cap, cost, demands)
         self.assertEqual(cost, 150)
         expected = np.array(
             [
                 [0.0, 12.0, 8.0, 0.0, 0.0],
                 [0.0, 0.0, 8.0, 4.0, 0.0],
                 [0.0, 0.0, 0.0, 11.0, 5.0],
                 [0.0, 0.0, 0.0, 0.0, 10.0],
             ]
         )
         self.assertTrue(check_solution_scipy(sol, [expected]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx(self):
-        G = datasets.load_graph2_networkx()
+        G = load_graph2_networkx()
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 150)
         candidate = {
             (0, 1): {"flow": 12.0},
             (0, 2): {"flow": 8.0},
             (1, 2): {"flow": 8.0},
             (1, 3): {"flow": 4.0},
@@ -147,15 +187,15 @@
             (2, 4): {"flow": 1.0},
             (3, 4): {"flow": 14.0},
         }
         self.assertTrue(check_solution_networkx(sol, [candidate, candidate2]))
 
     @unittest.skipIf(nx is None, "networkx is not installed")
     def test_networkx_renamed(self):
-        G = datasets.load_graph2_networkx()
+        G = load_graph2_networkx()
         G = nx.relabel_nodes(G, {0: "s", 4: "t"})
         cost, sol = mcf.min_cost_flow_networkx(G)
         self.assertEqual(cost, 150)
         candidate = {
             ("s", 1): {"flow": 12.0},
             ("s", 2): {"flow": 8.0},
             (1, 2): {"flow": 8.0},
```

### Comparing `gurobi_optimods-0.2.0/tests/test_mwis.py` & `gurobi_optimods-1.0.0/tests/test_mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_portfolio.py` & `gurobi_optimods-1.0.0/tests/test_portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,68 @@
 
     def test_init_1(self):
         # Specifying both cov_matrix and cov_factors is disallowed
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
         L = np.linalg.cholesky(cov_matrix)
+        K = np.eye(L.shape[0])
+        e = np.zeros(mu.size)
 
         with self.assertRaises(TypeError):
-            mvp = MeanVariancePortfolio(mu, cov_matrix=cov_matrix, cov_factors=(L,))
+            mvp = MeanVariancePortfolio(
+                mu, cov_matrix=cov_matrix, cov_factors=(L, K, e)
+            )
+
+    def test_init_2(self):
+        # cov_factors must always be a triple
+        data = load_portfolio()
+        cov_matrix = data.cov()
+        mu = data.mean()
+        L = np.linalg.cholesky(cov_matrix)
+        K = np.eye(L.shape[0])
+        e = np.zeros(mu.size)
+
+        with self.assertRaises(ValueError):
+            mvp = MeanVariancePortfolio(mu, cov_factors=tuple())
+
+        with self.assertRaises(ValueError):
+            mvp = MeanVariancePortfolio(mu, cov_factors=(L,))
+
+        with self.assertRaises(ValueError):
+            mvp = MeanVariancePortfolio(mu, cov_factors=(L, K))
+
+    def test_init_3(self):
+        # Example input that ought to succeed
+        B = np.random.rand(8, 2)
+        K = np.diag([0.5, 2])
+        d = np.ones(8)
+        mu = np.ones(8)
+        mvp = MeanVariancePortfolio(mu, cov_factors=(B, K, d))
+        # Nothing to test, but shouldn't error
+
+    def test_init_4(self):
+        # cov_factors[1] must be positive definite, this is semi-definite
+        B = np.random.rand(8, 2)
+        K = np.diag([1, 0])
+        d = np.ones(8)
+        mu = np.ones(8)
+
+        with self.assertRaises(np.linalg.LinAlgError):
+            mvp = MeanVariancePortfolio(mu, cov_factors=(B, K, d))
+
+    def test_init_5(self):
+        # cov_factors[1] must be positive definite, this is indefinite
+        B = np.random.rand(8, 2)
+        K = np.diag([1, -1])
+        d = np.ones(8)
+        mu = np.ones(8)
+
+        with self.assertRaises(np.linalg.LinAlgError):
+            mvp = MeanVariancePortfolio(mu, cov_factors=(B, K, d))
 
     def test_outputflag(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         mu = data.mean()
 
         mvp = MeanVariancePortfolio(mu, cov_matrix)
@@ -643,34 +694,38 @@
 
         self.assertAlmostEqual(x[x < 0].sum(), -0.1)
 
     def test_risk_factors_equivalent_0(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         L = np.linalg.cholesky(cov_matrix)
+        K = np.eye(L.shape[0])
         mu = data.mean()
+        e = np.zeros(mu.size)
         gamma = 100.0
 
         # Two equivalent setups: Sigma itself, and its Cholesky factor
-        mvp_factors = MeanVariancePortfolio(mu, None, cov_factors=(L,))
+        mvp_factors = MeanVariancePortfolio(mu, None, cov_factors=(L, K, e))
         mvp_Sigma = MeanVariancePortfolio(mu, cov_matrix)
 
         x_factors = mvp_factors.efficient_portfolio(gamma).x
         x_Sigma = mvp_Sigma.efficient_portfolio(gamma).x
 
         assert_allclose(x_factors, x_Sigma, atol=1e-6)
 
     def test_risk_factors_auxdata_0(self):
         data = load_portfolio()
         cov_matrix = data.cov()
         L = np.linalg.cholesky(cov_matrix)
+        K = np.eye(L.shape[0])
         mu = data.mean()
+        e = np.zeros(mu.size)
         gamma = 100.0
 
-        mvp = MeanVariancePortfolio(mu, None, cov_factors=(L,))
+        mvp = MeanVariancePortfolio(mu, None, cov_factors=(L, K, e))
         pf = mvp.efficient_portfolio(gamma)
 
         self.assertAlmostEqual(pf.ret, mu.to_numpy() @ pf.x)
         self.assertAlmostEqual(pf.risk, cov_matrix.to_numpy() @ pf.x @ pf.x)
 
     def test_risk_factors_equivalent_1(self):
         # Use case: Data that would emerge from a Single factor model
@@ -683,37 +738,37 @@
         # We don't bother simulating any such data, we just make up the data.
 
         n = 3
 
         mu = 0.2 + (0.2 * np.random.rand(3) - 0.1)
         s = (0.1 + 0.2 * np.random.rand(3)).reshape((3, 1))
         d = 0.05 + 0.3 * np.random.rand(3)
-        D = np.diag(d)
         cov_matrix = s @ s.T + np.diag(d**2)
 
         # Two equivalent setups: Sigma itself, and its Cholesky factor
         gamma = 20
-        mvp_factors = MeanVariancePortfolio(mu, None, cov_factors=(s, D))
+        mvp_factors = MeanVariancePortfolio(
+            mu, None, cov_factors=(s, np.eye(1), d**2)
+        )
         mvp_Sigma = MeanVariancePortfolio(mu, cov_matrix)
 
         x_factors = mvp_factors.efficient_portfolio(gamma).x
         x_Sigma = mvp_Sigma.efficient_portfolio(gamma).x
 
         assert_allclose(x_factors, x_Sigma, atol=1e-5)
 
     def test_risk_factors_auxdata_1(self):
         n = 3
         mu = 0.2 + (0.2 * np.random.rand(3) - 0.1)
         s = (0.1 + 0.2 * np.random.rand(3)).reshape((3, 1))
         d = 0.05 + 0.3 * np.random.rand(3)
-        D = np.diag(d)
         cov_matrix = s @ s.T + np.diag(d**2)
 
         gamma = 20
-        mvp = MeanVariancePortfolio(mu, None, cov_factors=(s, D))
+        mvp = MeanVariancePortfolio(mu, None, cov_factors=(s, np.eye(1), d**2))
         pf = mvp.efficient_portfolio(gamma)
 
         self.assertAlmostEqual(pf.ret, mu @ pf.x)
         self.assertAlmostEqual(pf.risk, cov_matrix @ pf.x @ pf.x)
 
     def test_costs_per_asset_long(self):
         data = load_portfolio()
```

### Comparing `gurobi_optimods-0.2.0/tests/test_qubo.py` & `gurobi_optimods-1.0.0/tests/test_qubo.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_regression.py` & `gurobi_optimods-1.0.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_utils.py` & `gurobi_optimods-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/test_workforce.py` & `gurobi_optimods-1.0.0/tests/test_workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/tests/utils.py` & `gurobi_optimods-1.0.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/.gitignore` & `gurobi_optimods-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/LICENSE` & `gurobi_optimods-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/NOTICE` & `gurobi_optimods-1.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-0.2.0/README.md` & `gurobi_optimods-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
 [![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=latest)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest)
 
-**⚠ Warning**
-
-```This code is in a pre-release state. It may not be fully functional and breaking changes can occur without notice.```
-
 # gurobi-optimods: nice APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gurobi_optimods-0.2.0/pyproject.toml` & `gurobi_optimods-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 [project]
 name = "gurobi-optimods"
 description = "Nice APIs for common optimization tasks"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
-keywords = ["optimization", "gurobipy", "pandas"]
+keywords = ["optimization", "gurobipy", "pandas", "scipy"]
 authors = [
     { name = "Simon Bowly", email = "bowly@gurobi.com" },
     { name = "Robert Luce", email = "luce@gurobi.com" },
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "gurobipy>=10.0.0",
+    "gurobipy>=10.0.1",
     "gurobipy-pandas>=1.0.0",
     "numpy",
     "pandas",
-    "scipy",
+    "scipy>=1.8.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 examples = [
     "networkx",
     "matplotlib",
```

### Comparing `gurobi_optimods-0.2.0/PKG-INFO` & `gurobi_optimods-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 Metadata-Version: 2.1
 Name: gurobi-optimods
-Version: 0.2.0
+Version: 1.0.0
 Summary: Nice APIs for common optimization tasks
 Author-email: Simon Bowly <bowly@gurobi.com>, Robert Luce <luce@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
-Keywords: gurobipy,optimization,pandas
-Classifier: Development Status :: 4 - Beta
+Keywords: gurobipy,optimization,pandas,scipy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: gurobipy-pandas>=1.0.0
-Requires-Dist: gurobipy>=10.0.0
+Requires-Dist: gurobipy>=10.0.1
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: scipy
+Requires-Dist: scipy>=1.8.0
 Provides-Extra: examples
 Requires-Dist: matplotlib; extra == 'examples'
 Requires-Dist: networkx; extra == 'examples'
 Requires-Dist: scikit-learn; extra == 'examples'
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
 [![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=latest)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/latest)
 
-**⚠ Warning**
-
-```This code is in a pre-release state. It may not be fully functional and breaking changes can occur without notice.```
-
 # gurobi-optimods: nice APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

