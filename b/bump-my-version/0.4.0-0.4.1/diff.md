# Comparing `tmp/bump-my-version-0.4.0.tar.gz` & `tmp/bump-my-version-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.4.0.tar", last modified: Thu Apr 20 19:42:48 2023, max compression
+gzip compressed data, was "bump-my-version-0.4.1.tar", last modified: Fri Jun  9 11:43:57 2023, max compression
```

## Comparing `bump-my-version-0.4.0.tar` & `bump-my-version-0.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.114294 bump-my-version-0.4.0/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 19:42:48.000000 bump-my-version-0.4.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.114294 bump-my-version-0.4.0/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/basic_cfg_expected.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:42:48.118294 bump-my-version-0.4.0/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-20 19:42:25.000000 bump-my-version-0.4.0/tests/test_version_part.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg_expected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_version_part.py
```

### Comparing `bump-my-version-0.4.0/CHANGELOG.md` & `bump-my-version-0.4.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## 0.4.1 (2023-06-09)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.4.0...0.4.1)
+
+### Fixes
+
+- Fixes release.yaml. [01870d5](https://github.com/callowayproject/bump-my-version/commit/01870d5878b5f0a6e601863c4b9c25572db6cbb0)
+    
+  Outputs the notes to a file instead of an environment variable.
+### Other
+
+- [pre-commit.ci] auto fixes from pre-commit.com hooks. [266002f](https://github.com/callowayproject/bump-my-version/commit/266002f4d60ed6fe3623ba5f713318dc6220ec00)
+    
+  for more information, see https://pre-commit.ci
+- [pre-commit.ci] pre-commit autoupdate. [edc444f](https://github.com/callowayproject/bump-my-version/commit/edc444f0328c27d905b35a5c970320a7171d738f)
+    
+  **updates:** - [github.com/charliermarsh/ruff-pre-commit: v0.0.261 → v0.0.270](https://github.com/charliermarsh/ruff-pre-commit/compare/v0.0.261...v0.0.270)
+
+
 ## 0.4.0 (2023-04-20)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.3.0...0.4.0)
 
 ### Fixes
 
 - Fixed pre-commit hook for dependency checking. [3d5c253](https://github.com/callowayproject/bump-my-version/commit/3d5c2533333112577c43cfe84d2091b1b60564b0)
```

### Comparing `bump-my-version-0.4.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/CONTRIBUTING.md` & `bump-my-version-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/LICENSE` & `bump-my-version-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/PKG-INFO` & `bump-my-version-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.4.0
+Version: 0.4.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.4.0/README.md` & `bump-my-version-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.4.1/bump_my_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.4.0
+Version: 0.4.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.4.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.4.1/bump_my_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/aliases.py` & `bump-my-version-0.4.1/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/autocast.py` & `bump-my-version-0.4.1/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/bump.py` & `bump-my-version-0.4.1/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/cli.py` & `bump-my-version-0.4.1/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/config.py` & `bump-my-version-0.4.1/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/exceptions.py` & `bump-my-version-0.4.1/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/files.py` & `bump-my-version-0.4.1/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/functions.py` & `bump-my-version-0.4.1/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/logging.py` & `bump-my-version-0.4.1/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/scm.py` & `bump-my-version-0.4.1/bumpversion/scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/utils.py` & `bump-my-version-0.4.1/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/bumpversion/version_part.py` & `bump-my-version-0.4.1/bumpversion/version_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         try:
             # test whether all parts required in the format have values
             serialized = serialize_format.format(**values)
 
         except KeyError as e:
             missing_key = getattr(e, "message", e.args[0])
             raise MissingValueError(
-                f"Did not find key {repr(missing_key)} in {repr(version)} when serializing version number"
+                f"Did not find key {missing_key!r} in {repr(version)} when serializing version number"
             ) from e
 
         keys_needing_representation = set()
 
         keys = list(self.order)
         for i, k in enumerate(keys):
             v = values[k]
```

### Comparing `bump-my-version-0.4.0/pyproject.toml` & `bump-my-version-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     "click",
     "pydantic",
     "rich-click",
     "rich",
     "tomlkit",
 ]
 
+[project.scripts]
+bump-my-version = "bumpversion.cli:cli"
+bumpversion = "bumpversion.cli:cli"
+
+
 [project.urls]
 homepage = "https://github.com/callowayproject/bump-my-version"
 repository = "https://github.com/callowayproject/bump-my-version.git"
 documentation = "https://callowayproject.github.io/bump-my-version/"
 
 [project.optional-dependencies]
 dev = [
@@ -201,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.4.1"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.4.0/tests/conftest.py` & `bump-my-version-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.4.1/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.4.1/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.4.1/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_autocast.py` & `bump-my-version-0.4.1/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_bump.py` & `bump-my-version-0.4.1/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_cli.py` & `bump-my-version-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_config.py` & `bump-my-version-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_files.py` & `bump-my-version-0.4.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_functions.py` & `bump-my-version-0.4.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_scm.py` & `bump-my-version-0.4.1/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.0/tests/test_version_part.py` & `bump-my-version-0.4.1/tests/test_version_part.py`

 * *Files identical despite different names*

