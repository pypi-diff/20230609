# Comparing `tmp/pyrgo-0.3.0.tar.gz` & `tmp/pyrgo-0.4.0.tar.gz`

## Comparing `pyrgo-0.3.0.tar` & `pyrgo-0.4.0.tar`

### file list

```diff
@@ -1,76 +1,74 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.tool-versions
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyrgo-0.3.0/Makefile
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.3.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/constants.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/__main__.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/add.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/audit.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/build.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/check.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/clean.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/fmt.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/lock.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/remove.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/sync.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/test.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/venv.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/build.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/new.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/root.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/__main__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/constants.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/command.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/config.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/__init__.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/audit.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/build.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/check.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/clean.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/fmt.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/lock.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/sync.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/test.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/venv.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/build.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/new.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/serve.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/README.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/__init__.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/starter-project.zip
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/command.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/io.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/text.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 pyrgo-0.3.0/requirements/core.txt
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyrgo-0.3.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.3.0/scripts/new_release.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/test_errors.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/models/test_command.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/utilities/test_command.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/utilities/test_text.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.3.0/LICENSE
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyrgo-0.3.0/README.md
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pyrgo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.tool-versions
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyrgo-0.4.0/Makefile
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.4.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/constants.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/__main__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/audit.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/build.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/check.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/clean.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/fmt.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/lock.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/sync.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/test.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/venv.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/build.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/new.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/root.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_new/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_new/__main__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/cli/pyrgo_new/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/constants.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/models/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/models/command.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/models/config.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/__init__.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/audit.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/build.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/check.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/clean.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/fmt.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/lock.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/sync.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/test.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/venv.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/docs/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/docs/build.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/docs/new.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/ops/docs/serve.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/resources/README.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/resources/__init__.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/resources/starter-project.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/utilities/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/utilities/command.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/utilities/io.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyrgo/core/utilities/text.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 pyrgo-0.4.0/requirements/core.txt
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 pyrgo-0.4.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.4.0/scripts/new_release.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pyrgo-0.4.0/tests/test_errors.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyrgo-0.4.0/tests/models/test_command.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pyrgo-0.4.0/tests/utilities/test_command.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyrgo-0.4.0/tests/utilities/test_text.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pyrgo-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrgo-0.4.0/README.md
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pyrgo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyrgo-0.4.0/PKG-INFO
```

### Comparing `pyrgo-0.3.0/Makefile` & `pyrgo-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/.github/workflows/release.yml` & `pyrgo-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/.github/workflows/test.yml` & `pyrgo-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/.vscode/settings.json` & `pyrgo-0.4.0/.vscode/settings.json`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     "editor.rulers": [
         88,
         100
     ],
     "python.testing.pytestArgs": [
         "tests",
         // https://github.com/microsoft/vscode-python/issues/693#issuecomment-367856613
-        "--no-cov",
+        "--no-cov"
     ],
     "python.testing.pytestEnabled": true,
     "python.analysis.autoImportCompletions": true,
     "python.analysis.completeFunctionParens": true,
     "python.analysis.inlayHints.callArgumentNames": true,
     "python.analysis.inlayHints.variableTypes": true,
     "python.analysis.typeCheckingMode": "basic",
     "python.analysis.userFileIndexingLimit": -1,
     "[python]": {
         "editor.defaultFormatter": "ms-python.black-formatter"
-    },
+    }
 }
```

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/cli.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Root core CLI."""
 from __future__ import annotations
 
 import click
 
 from pyrgo.cli.constants import PACKAGE_NAME
-from pyrgo.cli.pyrgo_core.commands.add import add
 from pyrgo.cli.pyrgo_core.commands.audit import audit
 from pyrgo.cli.pyrgo_core.commands.build import build
 from pyrgo.cli.pyrgo_core.commands.check import check
 from pyrgo.cli.pyrgo_core.commands.clean import clean
 from pyrgo.cli.pyrgo_core.commands.docs import docs
 from pyrgo.cli.pyrgo_core.commands.fmt import fmt
 from pyrgo.cli.pyrgo_core.commands.lock import lock
-from pyrgo.cli.pyrgo_core.commands.remove import remove
 from pyrgo.cli.pyrgo_core.commands.sync import sync
 from pyrgo.cli.pyrgo_core.commands.test import test
 from pyrgo.cli.pyrgo_core.commands.venv import venv
 from pyrgo.cli.utils import add_commands
 
 
 @click.group(
@@ -43,16 +41,14 @@
     cli=root,
     commands=[
         check,
         clean,
         fmt,
         lock,
         venv,
-        add,
         test,
         docs,
-        remove,
         build,
         sync,
         audit,
     ],
 )
```

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/audit.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/audit.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/check.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/check.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,18 +31,27 @@
     "--ignore-noqa",
     "ignore_noqa",
     is_flag=True,
     default=False,
     type=bool,
     help="Ignore any `# noqa` comments",
 )
-def check(*, timeout: int, add_noqa: bool, ignore_noqa: bool) -> None:
+@click.option(
+    "--typing/--no-typing",
+    "typing",
+    is_flag=True,
+    default=True,
+    type=bool,
+    help="Check typing with mypy.",
+)
+def check(*, timeout: int, add_noqa: bool, ignore_noqa: bool, typing: bool) -> None:
     """Analyze the current package with `ruff` and `mypy`."""
     executed = ops.check.execute(
         add_noqa=add_noqa,
         ignore_noqa=ignore_noqa,
         deamon_time_out=timeout,
         app_config=app_config,
+        typing=typing,
     )
     if not isinstance(executed, Ok):
         sys.exit(1)
     sys.exit(0)
```

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/lock.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/sync.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/test.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/test.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/build.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/cli/pyrgo_new/cli.py` & `pyrgo-0.4.0/pyrgo/cli/pyrgo_new/cli.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/models/command.py` & `pyrgo-0.4.0/pyrgo/core/models/command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/models/config.py` & `pyrgo-0.4.0/pyrgo/core/models/config.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/audit.py` & `pyrgo-0.4.0/pyrgo/core/ops/audit.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/build.py` & `pyrgo-0.4.0/pyrgo/core/ops/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/check.py` & `pyrgo-0.4.0/pyrgo/core/ops/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""check operation."""
+"""test operation."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pyrgo.core.models.command import (
     PythonExecCommand,
 )
@@ -14,36 +14,28 @@
     from result import Result
 
     from pyrgo.core.models.config import Config
 
 
 def execute(
     *,
-    add_noqa: bool,
-    ignore_noqa: bool,
-    deamon_time_out: int,
+    marker: str | None,
     app_config: Config,
 ) -> Result[None, list[subprocess.CalledProcessError]]:
-    """Execute check operation."""
-    ruff_command = PythonExecCommand(
-        program="ruff",
+    """Execute test operation."""
+    pytest_command = PythonExecCommand(
+        program="pytest",
     )
-    mypy_command = PythonExecCommand(
-        program="mypy.dmypy",
-    ).add_args(args=["run", "--timeout", str(deamon_time_out), "--"])
-
-    if add_noqa:
-        ruff_command.add_args(args=["--add-noqa"])
-    if ignore_noqa:
-        ruff_command.add_args(args=["--ignore-noqa"])
-
-    for command in [ruff_command, mypy_command]:
-        command.add_args(
-            args=app_config.relevant_paths,
+    if marker:
+        pytest_command.add_args(
+            args=[
+                "-m",
+                marker,
+            ],
         )
 
+    pytest_command.add_args(args=app_config.pytest_paths)
     return inform_and_run_program(
         commands=[
-            ruff_command,
-            mypy_command,
+            pytest_command,
         ],
     )
```

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/clean.py` & `pyrgo-0.4.0/pyrgo/core/ops/clean.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/fmt.py` & `pyrgo-0.4.0/pyrgo/core/ops/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/lock.py` & `pyrgo-0.4.0/pyrgo/core/ops/lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 def execute(
     *,
     groups: Iterable[str],
     app_config: Config,
     generate_hashes: bool,
 ) -> Result[None, list[subprocess.CalledProcessError]]:
     """Execute lock operation."""
-    app_config.requirements_dir.relative_to(app_config.cwd)
+    app_config.requirements_dir.relative_to(app_config.cwd).mkdir(
+        exist_ok=True,
+        parents=False,
+    )
+
     commands: list[PythonExecCommand] = []
 
     if not groups:
         groups = app_config.dependency_groups
 
     for group in groups:
         piptools_command = PythonExecCommand(
```

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/sync.py` & `pyrgo-0.4.0/pyrgo/core/ops/sync.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/test.py` & `pyrgo-0.4.0/pyrgo/core/ops/docs/serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-"""test operation."""
+"""docs serve operation."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pyrgo.core.models.command import (
     PythonExecCommand,
 )
 from pyrgo.core.utilities.command import inform_and_run_program
 
 if TYPE_CHECKING:
     import subprocess
 
     from result import Result
 
-    from pyrgo.core.models.config import Config
-
 
 def execute(
     *,
-    marker: str | None,
-    app_config: Config,
+    dev_address: str,
+    theme: str,
+    strict: bool,
 ) -> Result[None, list[subprocess.CalledProcessError]]:
-    """Execute test operation."""
-    pytest_command = PythonExecCommand(
-        program="pytest",
+    """Execute docs serve operation."""
+    serve_command = PythonExecCommand(
+        program="mkdocs",
+    ).add_args(
+        args=[
+            "serve",
+        ],
     )
-    if marker:
-        pytest_command.add_args(
-            args=[
-                "-m",
-                marker,
-            ],
-        )
+    if strict:
+        serve_command.add_args(args=["--strict"])
 
-    pytest_command.add_args(args=app_config.pytest_paths)
-    return inform_and_run_program(
-        commands=[
-            pytest_command,
+    serve_command.add_args(
+        args=[
+            "--theme",
+            theme,
+            "--dev-addr",
+            dev_address,
         ],
     )
+
+    return inform_and_run_program(
+        commands=[serve_command],
+    )
```

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/venv.py` & `pyrgo-0.4.0/pyrgo/core/ops/venv.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/docs/build.py` & `pyrgo-0.4.0/pyrgo/core/ops/docs/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/ops/docs/new.py` & `pyrgo-0.4.0/pyrgo/core/ops/docs/new.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/resources/starter-project.zip` & `pyrgo-0.4.0/pyrgo/core/resources/starter-project.zip`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2177 bytes, number of entries: 7
+Zip file size: 2130 bytes, number of entries: 7
 drwxr-xr-x  3.0 unx        0 bx stor 23-May-19 15:54 starter-project/
 drwxr-xr-x  3.0 unx        0 bx stor 23-May-18 22:27 starter-project/project_name/
 -rw-r--r--  3.0 unx        0 bx stor 23-May-18 22:14 starter-project/project_name/__init__.py
--rw-r--r--  3.0 unx     1914 tx defN 23-May-19 16:48 starter-project/pyproject.toml
+-rw-r--r--  3.0 unx     1818 tx defN 23-Jun-09 16:26 starter-project/pyproject.toml
 drwxr-xr-x  3.0 unx        0 bx stor 23-May-18 22:14 starter-project/tests/
 -rw-r--r--  3.0 unx       16 tx stor 23-May-18 22:15 starter-project/tests/README.md
 -rw-r--r--  3.0 unx       19 tx stor 23-May-19 15:23 starter-project/README.md
-7 files, 1949 bytes uncompressed, 873 bytes compressed:  55.2%
+7 files, 1853 bytes uncompressed, 826 bytes compressed:  55.4%
```

#### starter-project/pyproject.toml

```diff
@@ -7,17 +7,14 @@
 version = "0.1.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
-authors = [
-    { name = "author", email = "author-email"}
-]
 dependencies = [
     
 ]
 
 [project.optional-dependencies]
 dev = [
     "pyrgo"
@@ -52,16 +49,15 @@
     "dist",
     "node_modules",
     "venv",
 ]
 
 [tool.ruff.per-file-ignores]
 "scripts/*.py" = ["INP001"]
-"__init__.py" = ["D104"]
-"tests/*.py" = ["INP001", "S101"]
+"tests/*.py" = ["S101"]
 
 [tool.ruff.isort]
 known-first-party = ["project_name"]
 force-wrap-aliases = true
 combine-as-imports = true
 
 [tool.ruff.flake8-tidy-imports]
```

### Comparing `pyrgo-0.3.0/pyrgo/core/utilities/command.py` & `pyrgo-0.4.0/pyrgo/core/utilities/command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/utilities/io.py` & `pyrgo-0.4.0/pyrgo/core/utilities/io.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/pyrgo/core/utilities/text.py` & `pyrgo-0.4.0/pyrgo/core/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/requirements/core.txt` & `pyrgo-0.4.0/requirements/dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/core.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=dev --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
 #
 --trusted-host pypi.python.org
 --trusted-host pypi.org
 --trusted-host files.pythonhosted.org
 
 black==23.3.0
     # via pyrgo (pyproject.toml)
 build==0.10.0
     # via
     #   pip-tools
     #   pyrgo (pyproject.toml)
-cachecontrol[filecache]==0.12.11
+cachecontrol[filecache]==0.13.1
     # via pip-audit
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   mkdocs
     #   pip-tools
     #   pyrgo (pyproject.toml)
 colorama==0.4.6
     # via mkdocs-material
+coverage[toml]==7.2.7
+    # via pytest-cov
 cyclonedx-python-lib==2.7.1
     # via pip-audit
 exceptiongroup==1.1.1
     # via pytest
+filelock==3.12.0
+    # via cachecontrol
 ghp-import==2.1.0
     # via mkdocs
 html5lib==1.1
     # via pip-audit
 idna==3.4
     # via requests
 importlib-metadata==6.6.0
@@ -49,34 +53,32 @@
     #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
-lockfile==0.12.2
-    # via cachecontrol
 loguru==0.7.0
     # via pyrgo (pyproject.toml)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markdown-it-py==2.2.0
     # via rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.3
     # via mkdocs-material
-mkdocs-material==9.1.13
+mkdocs-material==9.1.15
     # via pyrgo (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 msgpack==1.0.5
     # via cachecontrol
 mypy==1.3.0
     # via pyrgo (pyproject.toml)
@@ -94,15 +96,15 @@
     #   pip-audit
     #   pip-requirements-parser
     #   pytest
 pathspec==0.11.1
     # via black
 pip-api==0.0.30
     # via pip-audit
-pip-audit==2.5.5
+pip-audit==2.5.6
     # via pyrgo (pyproject.toml)
 pip-requirements-parser==32.0.1
     # via pip-audit
 pip-tools==6.13.0
     # via pyrgo (pyproject.toml)
 platformdirs==3.5.1
     # via black
@@ -115,36 +117,40 @@
 pymdown-extensions==10.0.1
     # via mkdocs-material
 pyparsing==3.0.9
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
+    # via
+    #   pyrgo (pyproject.toml)
+    #   pytest-cov
+pytest-cov==4.1.0
     # via pyrgo (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.5.5
+regex==2023.6.3
     # via mkdocs-material
-requests==2.29.0
+requests==2.31.0
     # via
     #   cachecontrol
     #   mkdocs-material
     #   pip-audit
 result==0.10.0
     # via pyrgo (pyproject.toml)
-rich==13.3.5
+rich==13.4.1
     # via pip-audit
-ruff==0.0.267
+ruff==0.0.272
     # via pyrgo (pyproject.toml)
 six==1.16.0
     # via
     #   html5lib
     #   python-dateutil
 sortedcontainers==2.4.0
     # via cyclonedx-python-lib
@@ -152,33 +158,36 @@
     # via
     #   cyclonedx-python-lib
     #   pip-audit
 tomli==2.0.1
     # via
     #   black
     #   build
+    #   coverage
     #   mypy
     #   pyproject-hooks
     #   pytest
 typed-ast==1.5.4
     # via
     #   black
     #   mypy
-typing-extensions==4.5.0
+typing-extensions==4.6.3
     # via
     #   black
     #   importlib-metadata
     #   markdown-it-py
     #   mkdocs
     #   mypy
     #   platformdirs
     #   result
     #   rich
-urllib3==1.26.15
-    # via requests
+urllib3==1.26.16
+    # via
+    #   pip-audit
+    #   requests
 watchdog==3.0.0
     # via mkdocs
 webencodings==0.5.1
     # via html5lib
 wheel==0.40.0
     # via pip-tools
 zipp==3.15.0
```

### Comparing `pyrgo-0.3.0/requirements/dev.txt` & `pyrgo-0.4.0/requirements/core.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=requirements/dev.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/core.txt --resolver=backtracking pyproject.toml
 #
 --trusted-host pypi.python.org
 --trusted-host pypi.org
 --trusted-host files.pythonhosted.org
 
 black==23.3.0
     # via pyrgo (pyproject.toml)
 build==0.10.0
     # via
     #   pip-tools
     #   pyrgo (pyproject.toml)
-cachecontrol[filecache]==0.12.11
+cachecontrol[filecache]==0.13.1
     # via pip-audit
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   mkdocs
     #   pip-tools
     #   pyrgo (pyproject.toml)
 colorama==0.4.6
     # via mkdocs-material
-coverage[toml]==7.2.5
-    # via pytest-cov
 cyclonedx-python-lib==2.7.1
     # via pip-audit
 exceptiongroup==1.1.1
     # via pytest
+filelock==3.12.0
+    # via cachecontrol
 ghp-import==2.1.0
     # via mkdocs
 html5lib==1.1
     # via pip-audit
 idna==3.4
     # via requests
 importlib-metadata==6.6.0
@@ -51,34 +51,32 @@
     #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
-lockfile==0.12.2
-    # via cachecontrol
 loguru==0.7.0
     # via pyrgo (pyproject.toml)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-material
     #   pymdown-extensions
 markdown-it-py==2.2.0
     # via rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mkdocs==1.4.3
     # via mkdocs-material
-mkdocs-material==9.1.13
+mkdocs-material==9.1.15
     # via pyrgo (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 msgpack==1.0.5
     # via cachecontrol
 mypy==1.3.0
     # via pyrgo (pyproject.toml)
@@ -96,15 +94,15 @@
     #   pip-audit
     #   pip-requirements-parser
     #   pytest
 pathspec==0.11.1
     # via black
 pip-api==0.0.30
     # via pip-audit
-pip-audit==2.5.5
+pip-audit==2.5.6
     # via pyrgo (pyproject.toml)
 pip-requirements-parser==32.0.1
     # via pip-audit
 pip-tools==6.13.0
     # via pyrgo (pyproject.toml)
 platformdirs==3.5.1
     # via black
@@ -117,40 +115,36 @@
 pymdown-extensions==10.0.1
     # via mkdocs-material
 pyparsing==3.0.9
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
-    # via
-    #   pyrgo (pyproject.toml)
-    #   pytest-cov
-pytest-cov==4.0.0
     # via pyrgo (pyproject.toml)
 python-dateutil==2.8.2
     # via ghp-import
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2023.5.5
+regex==2023.6.3
     # via mkdocs-material
-requests==2.29.0
+requests==2.31.0
     # via
     #   cachecontrol
     #   mkdocs-material
     #   pip-audit
 result==0.10.0
     # via pyrgo (pyproject.toml)
-rich==13.3.5
+rich==13.4.1
     # via pip-audit
-ruff==0.0.267
+ruff==0.0.272
     # via pyrgo (pyproject.toml)
 six==1.16.0
     # via
     #   html5lib
     #   python-dateutil
 sortedcontainers==2.4.0
     # via cyclonedx-python-lib
@@ -158,34 +152,35 @@
     # via
     #   cyclonedx-python-lib
     #   pip-audit
 tomli==2.0.1
     # via
     #   black
     #   build
-    #   coverage
     #   mypy
     #   pyproject-hooks
     #   pytest
 typed-ast==1.5.4
     # via
     #   black
     #   mypy
-typing-extensions==4.5.0
+typing-extensions==4.6.3
     # via
     #   black
     #   importlib-metadata
     #   markdown-it-py
     #   mkdocs
     #   mypy
     #   platformdirs
     #   result
     #   rich
-urllib3==1.26.15
-    # via requests
+urllib3==1.26.16
+    # via
+    #   pip-audit
+    #   requests
 watchdog==3.0.0
     # via mkdocs
 webencodings==0.5.1
     # via html5lib
 wheel==0.40.0
     # via pip-tools
 zipp==3.15.0
```

### Comparing `pyrgo-0.3.0/scripts/new_release.py` & `pyrgo-0.4.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/tests/test_errors.py` & `pyrgo-0.4.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/tests/models/test_command.py` & `pyrgo-0.4.0/tests/models/test_command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/tests/utilities/test_command.py` & `pyrgo-0.4.0/tests/utilities/test_command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/tests/utilities/test_text.py` & `pyrgo-0.4.0/tests/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/.gitignore` & `pyrgo-0.4.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 /target
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 .mypy_cache/
+.dmypy.json
 .ruff_cache/
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
```

### Comparing `pyrgo-0.3.0/LICENSE` & `pyrgo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgo-0.3.0/README.md` & `pyrgo-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -28,25 +28,24 @@
 pyrgo -h
 
 # Usage: pyrgo [OPTIONS] COMMAND [ARGS]...
 
 #   Pyrgo. Python package manager.
 
 # Options:
-#   --version   Show the version and exit.
-#   -h, --help  Show this message and exit.
+#   -v, --version  Show the version and exit.
+#   -h, --help     Show this message and exit.
 
 # Commands:
-#   add     Add dependencies to a pyproject.toml manifest file and install.
-#   build   Build project.
-#   check   Analyze the current package with `ruff` and `mypy`.
-#   clean   Remove artifacts that pyrgo has generated in the past.
-#   docs    Document you project with `mkdocs-material`.
-#   fmt     Format all files of the current project using `black` and `ruff`.
-#   init    Create a new pyrgo project in an existing directory.
-#   lock    Lock dependencies using `piptools`.
-#   new     Create a new pyrgo project.
-#   remove  Remove dependencies from the manifest file.
-#   sync    Synchronize virtual environment with requirements.txt.
-#   test    Execute tests using `pytest`.
-#   venv    Create project virtual environment.
+#   audit  Scan project requirements for packages with known vulnerabilities.
+#   build  Build project.
+#   check  Analyze the current package with `ruff` and `mypy`.
+#   clean  Remove artifacts that pyrgo has generated in the past.
+#   docs   Document you project with `mkdocs-material`.
+#   fmt    Format all files of the current project using `black` and `ruff`.
+#   lock   Lock dependencies using `piptools`.
+#   sync   Synchronize virtual environment with requirements.txt.
+#   test   Execute tests using `pytest`.
+#   venv   Create project virtual environment.
 ```
+
+Use `pyrgo-new -n <project-name> [path]` to initialize your new project
```

### Comparing `pyrgo-0.3.0/pyproject.toml` & `pyrgo-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyrgo"
-version = "0.3.0"
+version = "0.4.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `pyrgo-0.3.0/PKG-INFO` & `pyrgo-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrgo
-Version: 0.3.0
+Version: 0.4.0
 Project-URL: Documentation, https://github.com/Tomperez98/pyrgo#readme
 Project-URL: Issues, https://github.com/Tomperez98/pyrgo/issues
 Project-URL: Source, https://github.com/Tomperez98/pyrgo
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -55,25 +55,24 @@
 pyrgo -h
 
 # Usage: pyrgo [OPTIONS] COMMAND [ARGS]...
 
 #   Pyrgo. Python package manager.
 
 # Options:
-#   --version   Show the version and exit.
-#   -h, --help  Show this message and exit.
+#   -v, --version  Show the version and exit.
+#   -h, --help     Show this message and exit.
 
 # Commands:
-#   add     Add dependencies to a pyproject.toml manifest file and install.
-#   build   Build project.
-#   check   Analyze the current package with `ruff` and `mypy`.
-#   clean   Remove artifacts that pyrgo has generated in the past.
-#   docs    Document you project with `mkdocs-material`.
-#   fmt     Format all files of the current project using `black` and `ruff`.
-#   init    Create a new pyrgo project in an existing directory.
-#   lock    Lock dependencies using `piptools`.
-#   new     Create a new pyrgo project.
-#   remove  Remove dependencies from the manifest file.
-#   sync    Synchronize virtual environment with requirements.txt.
-#   test    Execute tests using `pytest`.
-#   venv    Create project virtual environment.
+#   audit  Scan project requirements for packages with known vulnerabilities.
+#   build  Build project.
+#   check  Analyze the current package with `ruff` and `mypy`.
+#   clean  Remove artifacts that pyrgo has generated in the past.
+#   docs   Document you project with `mkdocs-material`.
+#   fmt    Format all files of the current project using `black` and `ruff`.
+#   lock   Lock dependencies using `piptools`.
+#   sync   Synchronize virtual environment with requirements.txt.
+#   test   Execute tests using `pytest`.
+#   venv   Create project virtual environment.
 ```
+
+Use `pyrgo-new -n <project-name> [path]` to initialize your new project
```

