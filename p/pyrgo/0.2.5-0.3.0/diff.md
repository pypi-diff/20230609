# Comparing `tmp/pyrgo-0.2.5.tar.gz` & `tmp/pyrgo-0.3.0.tar.gz`

## Comparing `pyrgo-0.2.5.tar` & `pyrgo-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.tool-versions
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrgo-0.2.5/Makefile
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.2.5/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.2.5/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/constants.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/__main__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/add.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/audit.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/build.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/check.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/clean.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/fmt.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/lock.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/remove.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/sync.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/test.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/venv.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/build.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/new.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/root.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/__main__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/cli/pyrgo_new/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/constants.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/command.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/models/config.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/__init__.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/audit.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/build.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/check.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/clean.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/fmt.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/lock.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/sync.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/test.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/venv.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/build.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/new.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/ops/docs/serve.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/README.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/__init__.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/resources/starter-project.zip
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/command.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/io.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyrgo/core/utilities/text.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 pyrgo-0.2.5/requirements/core.txt
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyrgo-0.2.5/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.2.5/scripts/new_release.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/test_errors.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/models/test_command.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/utilities/test_command.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyrgo-0.2.5/tests/utilities/test_text.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyrgo-0.2.5/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.2.5/LICENSE
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyrgo-0.2.5/README.md
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pyrgo-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pyrgo-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.tool-versions
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyrgo-0.3.0/Makefile
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.3.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/constants.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/__main__.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/add.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/audit.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/build.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/check.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/clean.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/fmt.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/lock.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/remove.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/sync.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/test.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/venv.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/build.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/new.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/root.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/__main__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/cli/pyrgo_new/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/constants.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/command.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/models/config.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/__init__.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/audit.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/build.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/check.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/clean.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/fmt.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/lock.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/sync.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/test.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/venv.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/build.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/new.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/ops/docs/serve.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/README.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/__init__.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/resources/starter-project.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/command.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/io.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyrgo/core/utilities/text.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 pyrgo-0.3.0/requirements/core.txt
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 pyrgo-0.3.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.3.0/scripts/new_release.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/test_errors.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/models/test_command.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/utilities/test_command.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pyrgo-0.3.0/tests/utilities/test_text.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyrgo-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyrgo-0.3.0/README.md
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pyrgo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pyrgo-0.3.0/PKG-INFO
```

### Comparing `pyrgo-0.2.5/Makefile` & `pyrgo-0.3.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 .PHONY: build-docs
 build-docs:
 	@mkdocs build
 
 .PHONY: lock-dependencies
 lock-dependencies: ## Lock dependencies specified in pyproject.toml
 	@mkdir -p requirements
-	@pip-compile --resolver=backtracking -o requirements/core.lock pyproject.toml
-	@pip-compile --extra dev --resolver=backtracking -o requirements/dev.lock pyproject.toml
+	@pip-compile --resolver=backtracking -o requirements/core.txt pyproject.toml
+	@pip-compile --extra dev --resolver=backtracking -o requirements/dev.txt pyproject.toml
 
 .PHONY: reload-settings
 reload-settings: ## Reload settings from pyproject.toml
 	@touch pyproject.toml
 
 .PHONY: help
 help:
```

### Comparing `pyrgo-0.2.5/.github/workflows/release.yml` & `pyrgo-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/.github/workflows/test.yml` & `pyrgo-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/cli.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 @click.group(
     context_settings={
         "help_option_names": [
             "-h",
             "--help",
         ],
+        "show_default": True,
     },
 )
 @click.version_option(
     None,
     "-v",
     "--version",
     package_name=PACKAGE_NAME,
```

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/audit.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/audit.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/check.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 from pyrgo.core import ops
 from pyrgo.core.constants import app_config
 
 
 @click.command()
 @click.option(
+    "-t",
+    "--timeout",
+    "timeout",
+    default=360,
+    type=click.IntRange(min=0, max=None, min_open=True),
+    help="To automatically shutdown mypy deamon after n seconds of inactivity",
+)
+@click.option(
     "--add-noqa",
     "add_noqa",
     is_flag=True,
     default=False,
     type=bool,
     help="Enable automatic additions of `noqa` directives to failing lines",
 )
@@ -23,17 +31,18 @@
     "--ignore-noqa",
     "ignore_noqa",
     is_flag=True,
     default=False,
     type=bool,
     help="Ignore any `# noqa` comments",
 )
-def check(*, add_noqa: bool, ignore_noqa: bool) -> None:
+def check(*, timeout: int, add_noqa: bool, ignore_noqa: bool) -> None:
     """Analyze the current package with `ruff` and `mypy`."""
     executed = ops.check.execute(
         add_noqa=add_noqa,
         ignore_noqa=ignore_noqa,
+        deamon_time_out=timeout,
         app_config=app_config,
     )
     if not isinstance(executed, Ok):
         sys.exit(1)
     sys.exit(0)
```

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/lock.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/sync.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/test.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/test.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/build.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_core/commands/docs/serve.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_core/commands/docs/serve.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/cli/pyrgo_new/cli.py` & `pyrgo-0.3.0/pyrgo/cli/pyrgo_new/cli.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/models/command.py` & `pyrgo-0.3.0/pyrgo/core/models/command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/models/config.py` & `pyrgo-0.3.0/pyrgo/core/models/config.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/audit.py` & `pyrgo-0.3.0/pyrgo/core/ops/audit.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/build.py` & `pyrgo-0.3.0/pyrgo/core/ops/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/check.py` & `pyrgo-0.3.0/pyrgo/core/ops/check.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,24 @@
     from pyrgo.core.models.config import Config
 
 
 def execute(
     *,
     add_noqa: bool,
     ignore_noqa: bool,
+    deamon_time_out: int,
     app_config: Config,
 ) -> Result[None, list[subprocess.CalledProcessError]]:
     """Execute check operation."""
     ruff_command = PythonExecCommand(
         program="ruff",
     )
     mypy_command = PythonExecCommand(
-        program="mypy",
-    )
+        program="mypy.dmypy",
+    ).add_args(args=["run", "--timeout", str(deamon_time_out), "--"])
 
     if add_noqa:
         ruff_command.add_args(args=["--add-noqa"])
     if ignore_noqa:
         ruff_command.add_args(args=["--ignore-noqa"])
 
     for command in [ruff_command, mypy_command]:
```

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/clean.py` & `pyrgo-0.3.0/pyrgo/core/ops/clean.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 import itertools
 import shutil
 from typing import TYPE_CHECKING
 
 from result import Ok, Result
 
+from pyrgo.core.models.command import PythonExecCommand
+from pyrgo.core.utilities.command import inform_and_run_program
+
 if TYPE_CHECKING:
     from pyrgo.core.models.config import Config
 
 
 def execute(app_config: Config) -> Result[None, Exception]:
     """Execute clean operation."""
     for to_be_clean in itertools.chain(
@@ -29,8 +32,18 @@
     for env_not_as_opt_dep in set(app_config.available_envs).difference(
         set(app_config.dependency_groups),
     ):
         app_config.requirements_dir.joinpath(
             f"{env_not_as_opt_dep}.{app_config.lock_file_format}",
         ).unlink()
 
+    mypy_deamon_command = PythonExecCommand(
+        program="mypy.dmypy",
+    )
+    mypy_deamon_command.add_args(args=["stop"])
+    inform_and_run_program(
+        commands=[
+            mypy_deamon_command,
+        ],
+    )
+
     return Ok()
```

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/fmt.py` & `pyrgo-0.3.0/pyrgo/core/ops/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/lock.py` & `pyrgo-0.3.0/pyrgo/core/ops/lock.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/sync.py` & `pyrgo-0.3.0/pyrgo/core/ops/sync.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/test.py` & `pyrgo-0.3.0/pyrgo/core/ops/test.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/venv.py` & `pyrgo-0.3.0/pyrgo/core/ops/venv.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/docs/build.py` & `pyrgo-0.3.0/pyrgo/core/ops/docs/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/docs/new.py` & `pyrgo-0.3.0/pyrgo/core/ops/docs/new.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/ops/docs/serve.py` & `pyrgo-0.3.0/pyrgo/core/ops/docs/serve.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/resources/starter-project.zip` & `pyrgo-0.3.0/pyrgo/core/resources/starter-project.zip`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/utilities/command.py` & `pyrgo-0.3.0/pyrgo/core/utilities/command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/utilities/io.py` & `pyrgo-0.3.0/pyrgo/core/utilities/io.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyrgo/core/utilities/text.py` & `pyrgo-0.3.0/pyrgo/core/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/requirements/core.txt` & `pyrgo-0.3.0/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/requirements/dev.txt` & `pyrgo-0.3.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/scripts/new_release.py` & `pyrgo-0.3.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/tests/test_errors.py` & `pyrgo-0.3.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/tests/models/test_command.py` & `pyrgo-0.3.0/tests/models/test_command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/tests/utilities/test_command.py` & `pyrgo-0.3.0/tests/utilities/test_command.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/tests/utilities/test_text.py` & `pyrgo-0.3.0/tests/utilities/test_text.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/.gitignore` & `pyrgo-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/LICENSE` & `pyrgo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/README.md` & `pyrgo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.5/pyproject.toml` & `pyrgo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyrgo"
-version = "0.2.5"
+version = "0.3.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `pyrgo-0.2.5/PKG-INFO` & `pyrgo-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrgo
-Version: 0.2.5
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/Tomperez98/pyrgo#readme
 Project-URL: Issues, https://github.com/Tomperez98/pyrgo/issues
 Project-URL: Source, https://github.com/Tomperez98/pyrgo
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

