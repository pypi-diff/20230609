# Comparing `tmp/pyproject2conda-0.1.2.tar.gz` & `tmp/pyproject2conda-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.1.2.tar", last modified: Wed Jun  7 21:01:46 2023, max compression
+gzip compressed data, was "pyproject2conda-0.2.0.tar", last modified: Fri Jun  9 14:08:47 2023, max compression
```

## Comparing `pyproject2conda-0.1.2.tar` & `pyproject2conda-0.2.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.938294 pyproject2conda-0.1.2/
--rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.1.2/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.883517 pyproject2conda-0.1.2/.github/
--rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.1.2/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      465 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11480 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/Makefile
--rw-r--r--   0 wpk      (42033)    36681    14929 2023-06-07 21:01:46.937458 pyproject2conda-0.1.2/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681    12136 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.883962 pyproject2conda-0.1.2/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.884371 pyproject2conda-0.1.2/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.885176 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.890953 pyproject2conda-0.1.2/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.870567 pyproject2conda-0.1.2/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.891501 pyproject2conda-0.1.2/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.893232 pyproject2conda-0.1.2/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.897324 pyproject2conda-0.1.2/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.901163 pyproject2conda-0.1.2/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.903355 pyproject2conda-0.1.2/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.904833 pyproject2conda-0.1.2/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.905703 pyproject2conda-0.1.2/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.906452 pyproject2conda-0.1.2/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.915353 pyproject2conda-0.1.2/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.1.2/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.1.2/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.1.2/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.1.2/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.1.2/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.916065 pyproject2conda-0.1.2/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.916831 pyproject2conda-0.1.2/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.922848 pyproject2conda-0.1.2/scripts/
--rw-r--r--   0 wpk      (42033)    36681      846 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681       38 2023-06-07 21:01:46.938481 pyproject2conda-0.1.2/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.873853 pyproject2conda-0.1.2/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.927662 pyproject2conda-0.1.2/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033)    36681      648 2023-06-07 15:56:44.000000 pyproject2conda-0.1.2/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     3091 2023-06-07 21:01:07.000000 pyproject2conda-0.1.2/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033)    36681    12606 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.933031 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033)    36681    14929 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681       60 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033)    36681      109 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       16 2023-06-07 21:01:46.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.1.2/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-07 21:01:46.936422 pyproject2conda-0.1.2/tests/
--rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.1.2/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      611 2023-06-07 02:50:51.000000 pyproject2conda-0.1.2/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681     2694 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tests/test_cli.py
--rw-r--r--   0 wpk      (42033)    36681     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tests/test_parser.py
--rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.1.2/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.302221 pyproject2conda-0.2.0/
+-rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.2.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.237643 pyproject2conda-0.2.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.2.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      465 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    16062 2023-06-09 14:08:47.301422 pyproject2conda-0.2.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681    13269 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.238282 pyproject2conda-0.2.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.239162 pyproject2conda-0.2.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.241114 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.248235 pyproject2conda-0.2.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.222678 pyproject2conda-0.2.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.248739 pyproject2conda-0.2.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.250835 pyproject2conda-0.2.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.256856 pyproject2conda-0.2.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.261140 pyproject2conda-0.2.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.263679 pyproject2conda-0.2.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.265127 pyproject2conda-0.2.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.265775 pyproject2conda-0.2.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.266542 pyproject2conda-0.2.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.278245 pyproject2conda-0.2.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.2.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.2.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.2.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.2.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.2.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.279565 pyproject2conda-0.2.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.280511 pyproject2conda-0.2.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.287460 pyproject2conda-0.2.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      846 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-06-09 14:08:47.302406 pyproject2conda-0.2.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.226108 pyproject2conda-0.2.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.290284 pyproject2conda-0.2.0/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033)    36681      648 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     6563 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033)    36681    15006 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.296674 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    16062 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681       60 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033)    36681      109 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       16 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.300387 pyproject2conda-0.2.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      611 2023-06-07 02:50:51.000000 pyproject2conda-0.2.0/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681     6093 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033)    36681     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.2.0/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.2.0/tox.ini
```

### Comparing `pyproject2conda-0.1.2/.cruft.json` & `pyproject2conda-0.2.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/.editorconfig` & `pyproject2conda-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/.gitignore` & `pyproject2conda-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/.pre-commit-config.yaml` & `pyproject2conda-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/CONTRIBUTING.md` & `pyproject2conda-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/LICENSE` & `pyproject2conda-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/Makefile` & `pyproject2conda-0.2.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -316,7 +316,13 @@
 
 # Note that this requires `auto-changelog`, which can be installed with pip(x)
 auto-changelog: ## autogenerate changelog and print to stdout
 	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
 
 commitizen-changelog:
 	cz changelog --unreleased-version unreleased --dry-run --incremental
+
+# --- cog output -- --------------------------------------------------------------------
+
+.PHONY: cog-readme
+cog-readme: ## apply cog to README.md
+	cog -rP README.md
```

### Comparing `pyproject2conda-0.1.2/PKG-INFO` & `pyproject2conda-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pyproject2conda
-Version: 0.1.2
-Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
-Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST-PD
-Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
-Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
-Keywords: pyproject2conda
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: Public Domain
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
@@ -121,89 +97,125 @@
 -p --pip     Pip install pyproject package on this line.
 -s --skip    Skip pyproject package on this line.
 -c --channel Add channel to pyproject package on this line
 ```
 
 So, if we run the following, we get:
 
+<!-- [[[cog
+import subprocess
+import shlex
+
+def run_command(cmd, wrapper="bash"):
+    args = shlex.split(cmd)
+    output = subprocess.check_output(args)
+    total = f"$ {cmd}\n{output.decode()}"
+
+    if wrapper:
+        total = f"\n```{wrapper}\n"  + total + "```\n"
+
+    print(total)
+]]] -->
+<!-- [[[end]]] -->
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml")]]] -->
+
 ```bash
-$ pyproject2conda create -f test/test-pyproject.toml
+$ pyproject2conda yaml -f tests/test-pyproject.toml
 channels:
   - conda-forge
 dependencies:
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
+<!-- [[[end]]] -->
+
 Note that other comments can be mixed in. This also works with extras. For
 example, with the following:
 
 Also, by default, the python version is not included in the resulting conda
 output. To include the specification from pyproject.toml, use `-p/--python`
 option:
 
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p")]]] -->
+
 ```bash
- ➜ pyproject2conda create -f tests/test-pyproject.toml -p
+$ pyproject2conda yaml -f tests/test-pyproject.toml -p
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
+<!-- [[[end]]] -->
+
 To specify a value of python, pass a value with:
 
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9")]]] -->
+
 ```bash
- ➜ pyproject2conda create -f tests/test-pyproject.toml -p python=3.9
+$ pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9
 channels:
   - conda-forge
 dependencies:
   - python=3.9
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
+<!-- [[[end]]] -->
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
   "pandas",
   "pytest", # p2c: -c conda-forge
 
 ]
 # ...
 
 ```
 
 and running the the following gives:
 
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e test")]]] -->
+
 ```bash
-$ pyproject2conda create -f tests/test-pyproject.toml test
+$ pyproject2conda yaml -f tests/test-pyproject.toml -e test
 channels:
   - conda-forge
 dependencies:
   - bthing-conda
   - conda-forge::cthing
   - pandas
   - conda-forge::pytest
   - pip
   - pip:
       - athing
 ```
 
+<!-- [[[end]]] -->
+
 `pyproject2conda` also works with self referenced dependencies:
 
 ```toml
 # ...
 [project.optional-dependencies]
 # ...
 dev-extras = [
@@ -212,30 +224,35 @@
 
 ]
 dev = ["hello[test]", "hello[dev-extras]"]
 # ...
 
 ```
 
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e dev")]]] -->
+
 ```bash
-$ pyproject2conda create -f tests/test-pyproject.toml dev
+$ pyproject2conda yaml -f tests/test-pyproject.toml -e dev
 channels:
   - conda-forge
 dependencies:
   - bthing-conda
   - conda-forge::cthing
   - pandas
   - conda-forge::pytest
   - additional-thing
   - conda-matplotlib
   - pip
   - pip:
       - athing
 ```
 
+<!-- [[[end]]] -->
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
@@ -293,26 +310,30 @@
 
 ]
 
 ```
 
 These can be accessed using either of the following:
 
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi")]]] -->
+
 ```bash
-$ pyproject2conda isolated -f tests/test-pyproject.toml dist-pypi
+$ pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi
 channels:
   - conda-forge
 dependencies:
   - setuptools
   - pip
   - pip:
       - build
-
 ```
 
+<!-- [[[end]]] -->
+
 or
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
@@ -325,82 +346,158 @@
   - pip:
       - build
 
 ```
 
 ### CLI options
 
+<!-- [[[cog run_command("pyproject2conda --help")]]] -->
+
+```bash
+$ pyproject2conda --help
+Usage: pyproject2conda [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  conda-requirements  Create requirement files for conda and pip.
+  json                Create json representation.
+  list                List available extras/isolated
+  requirements        Create requirements.txt for pip depedencies.
+  yaml                Create yaml file from dependencies and...
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run_command("pyproject2conda list --help")]]] -->
+
 ```bash
- ➜ pyproject2conda --help
+$ pyproject2conda list --help
+Usage: pyproject2conda list [OPTIONS]
+
+  List available extras/isolated
+
+Options:
+  -f, --file PATH  input pyproject.toml file
+  -v, --verbose
+  --help           Show this message and exit.
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run_command("pyproject2conda yaml --help")]]] -->
+
+```bash
+$ pyproject2conda yaml --help
+Usage: pyproject2conda yaml [OPTIONS]
+
+  Create yaml file from dependencies and optional-dependencies.
+
+Options:
+  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
+                       multiple extras.
+  -i, --isolated TEXT  Isolated dependencies (under
+                       [tool.pyproject2conda.isolated-dependencies]).  Can
+                       specify multiple times.
+  -c, --channel TEXT   conda channel.  Can specify. Overrides
+                       [tool.pyproject2conda.channels]
+  -f, --file PATH      input pyproject.toml file
+  -n, --name TEXT      Name of conda env
+  -o, --output PATH    File to output results
+  -p, --python TEXT    if flag passed without options, include python spec
+                       from pyproject.toml in output.  If value passed, use
+                       this value of python in the output
+  --help               Show this message and exit.
+```
 
- Usage: pyproject2conda [OPTIONS] COMMAND [ARGS]...
+<!-- [[[end]]] -->
 
-╭─ Options ───────────────────────────────────────────────────────────────────╮
-│ --help      Show this message and exit.                                     │
-╰─────────────────────────────────────────────────────────────────────────────╯
-╭─ Commands ──────────────────────────────────────────────────────────────────╮
-│ create    Create yaml file from dependencies and optional-dependencies.     │
-│ isolated  Create yaml file from                                             │
-│           [tool.pyproject2conda.isolated-dependencies]                      │
-│ list      List available extras/isolated                                    │
-╰─────────────────────────────────────────────────────────────────────────────╯
+<!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
+```bash
+$ pyproject2conda requirements --help
+Usage: pyproject2conda requirements [OPTIONS]
 
- ➜ pyproject2conda list --help
+  Create requirements.txt for pip depedencies.
 
- Usage: pyproject2conda list [OPTIONS]
+Options:
+  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
+                       multiple extras.
+  -i, --isolated TEXT  Isolated dependencies (under
+                       [tool.pyproject2conda.isolated-dependencies]).  Can
+                       specify multiple times.
+  -f, --file PATH      input pyproject.toml file
+  -o, --output PATH    File to output results
+  --help               Show this message and exit.
+```
 
- List available extras/isolated
+<!-- [[[end]]] -->
 
-╭─ Options ───────────────────────────────────────────────────────────────────╮
-│ --file     -f  PATH  input pyproject.toml file                              │
-│ --verbose  -v                                                               │
-│ --help               Show this message and exit.                            │
-╰─────────────────────────────────────────────────────────────────────────────╯
+<!-- [[[cog run_command("pyproject2conda conda-requirements --help")]]] -->
 
+```bash
+$ pyproject2conda conda-requirements --help
+Usage: pyproject2conda conda-requirements [OPTIONS] [PATH_CONDA] [PATH_PIP]
 
- ➜ pyproject2conda create --help
+  Create requirement files for conda and pip.
 
- Usage: pyproject2conda create [OPTIONS] [EXTRAS]...
+  These can be install with, for example,
 
- Create yaml file from dependencies and optional-dependencies.
+  conda install --file {path_conda} pip install -r {path_pip}
 
-╭─ Options ───────────────────────────────────────────────────────────────────╮
-│ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
-│                      Overrides [tool.pyproject2conda.channels]              │
-│ --file     -f  PATH  input pyproject.toml file                              │
-│ --name     -n  TEXT  Name of conda env                                      │
-│ --output   -o  PATH  File to output results                                 │
-│ --python   -p  TEXT  if flag passed without options, include python spec    │
-│                      from pyproject.toml in output.  If value passed, use   │
-│                      this value of python in the output                     │
-│ --help               Show this message and exit.                            │
-╰─────────────────────────────────────────────────────────────────────────────╯
+Options:
+  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
+                       multiple extras.
+  -i, --isolated TEXT  Isolated dependencies (under
+                       [tool.pyproject2conda.isolated-dependencies]).  Can
+                       specify multiple times.
+  -p, --python TEXT    if flag passed without options, include python spec
+                       from pyproject.toml in output.  If value passed, use
+                       this value of python in the output
+  -c, --channel TEXT   conda channel.  Can specify. Overrides
+                       [tool.pyproject2conda.channels]
+  -f, --file PATH      input pyproject.toml file
+  --prefix TEXT        set conda-output=prefix + 'conda.txt', pip-
+                       output=prefix + 'pip.txt'
+  --prepend-channel
+  --help               Show this message and exit.
+```
 
+<!-- [[[end]]] -->
 
- ➜ pyproject2conda isolated --help
+<!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
- Usage: pyproject2conda isolated [OPTIONS] ISOLATED...
+```bash
+$ pyproject2conda json --help
+Usage: pyproject2conda json [OPTIONS]
 
- Create yaml file from [tool.pyproject2conda.isolated-dependencies]
+  Create json representation.
 
-╭─ Options ───────────────────────────────────────────────────────────────────╮
-│ --channel  -c  TEXT  conda channel.  Can be specified multiple times.       │
-│                      Overrides [tool.pyproject2conda.channels]              │
-│ --file     -f  PATH  input pyproject.toml file                              │
-│ --name     -n  TEXT  Name of conda env                                      │
-│ --output   -o  PATH  File to output results                                 │
-│ --python   -p  TEXT  if flag passed without options, include python spec    │
-│                      from pyproject.toml in output.  If value passed, use   │
-│                      this value of python in the output                     │
-│ --help               Show this message and exit.                            │
-╰─────────────────────────────────────────────────────────────────────────────╯
+  Keys are: "dependencies": conda dependencies. "pip": pip dependencies.
+  "channels": conda channels.
 
+Options:
+  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
+                       multiple extras.
+  -i, --isolated TEXT  Isolated dependencies (under
+                       [tool.pyproject2conda.isolated-dependencies]).  Can
+                       specify multiple times.
+  -p, --python TEXT    if flag passed without options, include python spec
+                       from pyproject.toml in output.  If value passed, use
+                       this value of python in the output
+  -c, --channel TEXT   conda channel.  Can specify. Overrides
+                       [tool.pyproject2conda.channels]
+  -f, --file PATH      input pyproject.toml file
+  -o, --output PATH    File to output results
+  --help               Show this message and exit.
 ```
 
+<!-- [[[end]]] -->
+
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!-- See the [documentation][docs-link] for a look at -->
 <!-- `pyproject2conda` in action. -->
 
@@ -419,43 +516,7 @@
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
-
-# Changelog
-
-Changelog for `pyproject2conda`
-
-## Unreleased
-
-See the fragment files in
-[changelog.d](https://github.com/wpk-nist-gov/pyproject2conda)
-
-<!-- scriv-insert-here -->
-
-This software was developed by employees of the National Institute of Standards
-and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
-United States Code Section 105, works of NIST employees are not subject to
-copyright protection in the United States and are considered to be in the public
-domain. Permission to freely use, copy, modify, and distribute this software and
-its documentation without fee is hereby granted, provided that this notice and
-disclaimer of warranty appears in all copies.
-
-THE SOFTWARE IS PROVIDED 'AS IS' WITHOUT ANY WARRANTY OF ANY KIND, EITHER
-EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY
-THAT THE SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND FREEDOM FROM
-INFRINGEMENT, AND ANY WARRANTY THAT THE DOCUMENTATION WILL CONFORM TO THE
-SOFTWARE, OR ANY WARRANTY THAT THE SOFTWARE WILL BE ERROR FREE. IN NO EVENT
-SHALL NIST BE LIABLE FOR ANY DAMAGES, INCLUDING, BUT NOT LIMITED TO, DIRECT,
-INDIRECT, SPECIAL OR CONSEQUENTIAL DAMAGES, ARISING OUT OF, RESULTING FROM, OR
-IN ANY WAY CONNECTED WITH THIS SOFTWARE, WHETHER OR NOT BASED UPON WARRANTY,
-CONTRACT, TORT, OR OTHERWISE, WHETHER OR NOT INJURY WAS SUSTAINED BY PERSONS OR
-PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED FROM, OR AROSE OUT
-OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES PROVIDED HEREUNDER.
-
-Distributions of NIST software should also include copyright and licensing
-statements of any third-party software that are legally bundled with the code in
-compliance with the conditions of those licenses.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyproject2conda-0.1.2/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/Makefile` & `pyproject2conda-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_static/css/nist-combined.css` & `pyproject2conda-0.2.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_static/js/leave_notice.js` & `pyproject2conda-0.2.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.2.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.2.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.2.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/class-single-page.rst` & `pyproject2conda-0.2.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.2.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.2.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/module-custom.rst` & `pyproject2conda-0.2.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/module-single.rst` & `pyproject2conda-0.2.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/_templates/module-template.rst` & `pyproject2conda-0.2.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/conf.py` & `pyproject2conda-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/examples/example-usage.md` & `pyproject2conda-0.2.0/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.2.0/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/installation.md` & `pyproject2conda-0.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/docs/make.bat` & `pyproject2conda-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/environment/dev-extras.yaml` & `pyproject2conda-0.2.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/environment/docs-extras.yaml` & `pyproject2conda-0.2.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/examples/usage/demo.ipynb` & `pyproject2conda-0.2.0/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/pyproject.toml` & `pyproject2conda-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/scripts/dist-conda.mk` & `pyproject2conda-0.2.0/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.2.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/scripts/recipe-append.sh` & `pyproject2conda-0.2.0/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/src/pyproject2conda/__init__.py` & `pyproject2conda-0.2.0/src/pyproject2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/src/pyproject2conda/parser.py` & `pyproject2conda-0.2.0/src/pyproject2conda/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,14 +72,37 @@
 
     try:
         return reduce(operator.getitem, keys, nested_dict)
     except (KeyError, IndexError, TypeError):
         return default
 
 
+def _unique_list(values):
+    """
+    Return only unique values in list.
+    Unlike using set(values), this preserves order.
+    """
+    output = []
+    for v in values:
+        if v not in output:
+            output.append(v)
+    return output
+
+
+def _list_to_str(values, eol=True):
+    if values:
+        output = "\n".join(values)
+        if eol:
+            output += "\n"
+    else:
+        output = ""
+
+    return output
+
+
 def _iter_value_comment_pairs(
     array: tomlkit.items.Array,
 ) -> list[tuple(Tstr_opt, Tstr_opt)]:
     """Extract value and comments from array"""
     for v in array._value:
         if v.value is not None and not isinstance(v.value, tomlkit.items.Null):
             value = str(v.value)  # .as_string()
@@ -212,14 +235,15 @@
     return {"dependencies": conda_deps, "pip": pip_deps}
 
 
 def _pyproject_to_value_comment_pairs(
     data: tomlkit.toml_document.TOMLDocument,
     extras: Tstr_seq_opt = None,
     isolated: Tstr_seq_opt = None,
+    unique: bool = True,
 ):
     project = data["project"]
     package_name = project["name"]
 
     deps = project["dependencies"]
 
     if isolated:
@@ -234,14 +258,17 @@
         value_comment_list = get_value_comment_pairs(
             package_name=package_name,
             extras=extras,
             deps=deps,
             opts=get_in(["project", "optional-dependencies"], data),
         )
 
+    if unique:
+        value_comment_list = _unique_list(value_comment_list)
+
     return value_comment_list
 
 
 def pyproject_to_conda_lists(
     data: str | Path | tomlkit.toml_document.TOMLDocument,
     extras: Tstr_seq_opt = None,
     isolated: Tstr_seq_opt = None,
@@ -407,18 +434,81 @@
         isolated: Tstr_seq_opt = None,
     ) -> list[str]:
         self._check_extras_isolated(extras, isolated)
 
         values = _pyproject_to_value_comment_pairs(
             data=self.data, extras=extras, isolated=isolated
         )
-
         return [x for x, y in values if x is not None]
 
+    def to_requirements(
+        self,
+        extras: Tstr_opt = None,
+        isolated: Tstr_seq_opt = None,
+        stream: str | Path | None = None,
+    ):
+        """Create requirements.txt like file with pip dependencies."""
+
+        self._check_extras_isolated(extras, isolated)
+
+        reqs = self.to_requirement_list(extras=extras, isolated=isolated)
+
+        s = _list_to_str(reqs)
+
+        if stream:
+            with open(stream, "w") as f:
+                f.write(s)
+        else:
+            return s
+
+    def to_conda_requirements(
+        self,
+        extras: Tstr_opt = None,
+        isolated: Tstr_seq_opt = None,
+        channels: Tstr_seq_opt = None,
+        python: Tstr_opt = None,
+        prepend_channel: bool = False,
+        stream_conda: str | Path | None = None,
+        stream_pip: str | Path | None = None,
+    ):
+        output = self.to_conda_lists(
+            extras=extras,
+            isolated=isolated,
+            channels=channels,
+            python=python,
+        )
+
+        deps = output.get("dependencies", None)
+        reqs = output.get("pip", None)
+
+        channels = output.get("channels", None)
+        if channels and prepend_channel:
+            assert len(channels) == 1
+            channel = channels[0]
+            # add in channel if none exists
+            if deps:
+                deps = [dep if "::" in dep else f"{channel}::{dep}" for dep in deps]
+
+        deps_str = _list_to_str(deps)
+        reqs_str = _list_to_str(reqs)
+
+        if stream_conda and deps_str:
+            with open(stream_conda, "w") as f:
+                f.write(deps_str)
+
+        if stream_pip and reqs_str:
+            with open(stream_pip, "w") as f:
+                f.write(reqs_str)
+
+        return deps_str, reqs_str
+
     def _check_extras_isolated(self, extras, isolated):
+        if extras and isolated:
+            raise ValueError("can only specify extras or isolated, not both.")
+
         def _do_test(sent, available):
             if isinstance(sent, str):
                 sent = [sent]
             for s in sent:
                 if s not in available:
                     raise ValueError(f"{s} not in {available}")
```

### Comparing `pyproject2conda-0.1.2/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.2.0/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/tests/test-pyproject.toml` & `pyproject2conda-0.2.0/tests/test-pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/tests/test_parser.py` & `pyproject2conda-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.1.2/tox.ini` & `pyproject2conda-0.2.0/tox.ini`

 * *Files identical despite different names*

