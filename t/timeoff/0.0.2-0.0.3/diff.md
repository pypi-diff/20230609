# Comparing `tmp/timeoff-0.0.2.tar.gz` & `tmp/timeoff-0.0.3.tar.gz`

## Comparing `timeoff-0.0.2.tar` & `timeoff-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 timeoff-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 timeoff-0.0.2/Make.defs
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 timeoff-0.0.2/Makefile
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 timeoff-0.0.2/requirements.txt
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 timeoff-0.0.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/__init__.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/cli.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/config.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/exceptions.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/models.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/prompts.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/schedules.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/update.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 timeoff-0.0.2/src/timeoff/util.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 timeoff-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 timeoff-0.0.2/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 timeoff-0.0.2/README.md
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 timeoff-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 timeoff-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 timeoff-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 timeoff-0.0.3/Make.defs
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 timeoff-0.0.3/Makefile
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 timeoff-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 timeoff-0.0.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/__init__.py
+-rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/commands.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/config.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/exceptions.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/prompt.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/update.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/base.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/entry.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/policy.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/schedule.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 timeoff-0.0.3/src/timeoff/model/setting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 timeoff-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 timeoff-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 timeoff-0.0.3/README.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 timeoff-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 timeoff-0.0.3/PKG-INFO
```

### Comparing `timeoff-0.0.2/CHANGELOG.md` & `timeoff-0.0.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.0.3] - 2023-06-08
+
+## Changed
+
+- Use PyInquirer for prompts
+- Refactor and restructuring
+
 ## [0.0.2] - 2023-05-22
 
 ### Added
 
 - GitHub Actions workflow to publish to PyPI.
 
-[unreleased]: https://github.com/tifa/timeoff/compare/v0.0.2...HEAD
+[unreleased]: https://github.com/tifa/timeoff/compare/v0.0.3...HEAD
+[0.0.3]: https://github.com/tifa/timeoff/releases/tag/v0.0.2...v0.0.3
 [0.0.2]: https://github.com/tifa/timeoff/releases/tag/v0.0.1...v0.0.2
 [0.0.1]: https://github.com/tifa/timeoff/releases/tag/v0.0.1
```

### Comparing `timeoff-0.0.2/.github/workflows/pypi-publish.yml` & `timeoff-0.0.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `timeoff-0.0.2/src/timeoff/schedules.py` & `timeoff-0.0.3/src/timeoff/model/schedule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from abc import abstractmethod
 from dataclasses import dataclass
 from datetime import timedelta
 
+from timeoff.prompt import int_validator, prompt
 from timeoff.util import print_ordinal
 
-"""
-Schedules
-=========
-
-This module contains classes that represent different accrual schedules.
-"""
 
 @dataclass
 class Schedule:
     """Base class for all schedules."""
 
 @dataclass
 class PayPeriod(Schedule):
@@ -102,40 +97,33 @@
                 return last_day_of_month
 
         # Next date is on the first paydate of next month.
         return self._next_month(date).replace(day=self.first)
 
     @staticmethod
     def setup_prompt():
-        while True:
-            first = input("First pay date of the month (1-28) [1]: ") or 1
-            try:
-                first = int(first)
-            except ValueError:
-                print("Please enter a valid number")
-                continue
-
-            if first < 1 or first > SemiMonthly.MAX_COMMON_DAY:
-                print("Please enter a number between 1 and 28")
-            else:
-                break
-
-        while True:
-            second = (
-                input(
-                    "Second pay date of the month (2-28 or -1 for last day of the"
-                    " month) [15]: ",
-                )
-                or 15
-            )
-            try:
-                second = int(second)
-            except ValueError:
-                print("Please enter a valid number")
-                continue
-
-            if (second <= 1 or second > SemiMonthly.MAX_COMMON_DAY) and second != -1:
-                print("Please enter a number between 2 and 28")
-            else:
-                break
-
-        return [first, second]
+        """Prompt to set up the schedule and return a list of arguments for this class."""
+        questions = [
+            {
+                "type": "input",
+                "name": "first",
+                "message": "First pay date of the month (1-28)",
+                "default": "1",
+                "validate": int_validator(lambda val: val >= 1 and val <= SemiMonthly.MAX_COMMON_DAY
+                                          or "Please enter a number between 1 and 28"),
+                "filter": lambda val: int(val),
+            },
+        ]
+        answers = prompt(questions)
+        questions = [
+            {
+                "type": "input",
+                "name": "second",
+                "message": "Second pay date of the month (2-28 or -1 for last day of the month)",
+                "default": str(answers["first"] + 1),
+                "validate": int_validator(lambda val: val >= answers["first"] + 1 and val <= SemiMonthly.MAX_COMMON_DAY
+                                          or val == -1 or "Please enter a number between 2 and 28 or -1"), 
+                "filter": lambda val: int(val),
+            },
+        ]
+        answers.update(prompt(questions))
+        return [answers["first"], answers["second"]]
```

### Comparing `timeoff-0.0.2/src/timeoff/update.py` & `timeoff-0.0.3/src/timeoff/update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime
 
 from timeoff.exceptions import PolicyNotFoundError
-from timeoff.models import AccruedPTO, Policy, Settings
+from timeoff.model.entry import Accrued
+from timeoff.model.policy import Policy
+from timeoff.model.setting import Setting
 
 
 def effective_policy(policies, date):
     """Return the policy in effect on the given date."""
     all_policy_dates = sorted(policies.keys())
     last = None
     for policy_date in all_policy_dates:
@@ -18,20 +20,17 @@
     msg = "No policy found for date."
     raise PolicyNotFoundError(msg)
 
 
 def update_pto():
     all_policies = Policy.get()
 
-    all_accrued_pto = AccruedPTO.get()
-    if len(all_accrued_pto) == 0:
-        last_updated = Settings.get().starting_date
-    else:
-        last_updated = sorted(all_accrued_pto.keys())[-1]
+    all_accrued_pto = Accrued.get()
+    last_updated = Setting.get().starting_date if len(all_accrued_pto) == 0 else sorted(all_accrued_pto.keys())[-1]
 
     current_date = last_updated
     while current_date < datetime.today().date():
         policy = effective_policy(all_policies, current_date)
         current_date = policy.schedule.next_date(current_date)
         if current_date < datetime.today().date():
-            AccruedPTO(current_date, policy.rate).save()
+            Accrued(current_date, policy.rate).save()
```

### Comparing `timeoff-0.0.2/LICENSE` & `timeoff-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timeoff-0.0.2/README.md` & `timeoff-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 - View the remaining hours of PTO available to you.
 
 ## Installation
 
 To install ``timeoff``:
 
 ```console
-$ pip install git+https://github.com/tifa/timeoff
+$ pip install timeoff
 ```
 
 Documentation is in the works! Please run the `-h` help flag in the meantime. The interactive prompts will guide you through further instructions.
 
 ```console
 $ timeoff -h
 usage: timeoff [-h] {add,list,rm,settings} ...
```

### Comparing `timeoff-0.0.2/pyproject.toml` & `timeoff-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "timeoff"
 description = "Track vacation hours accrued."
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 license = { text = "MIT" }
 requires-python = ">=3.8"
 authors = [
   { name="Tiffany Huang", email="hello@tifa.io" },
 ]
 keywords = [
   "time off",
@@ -25,26 +25,26 @@
 dependencies = [
   "sphinx-rtd-theme==1.2.0",
   "sphinx-prompt==1.5.0",
   "tabulate==0.9.0",
 ]
 
 [project.scripts]
-timeoff = "timeoff.cli:main"
+timeoff = "timeoff.commands:main"
 
 [project.urls]
 Homepage = "https://github.com/tifa/timeoff"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.ruff]
 target-version = "py38"
-line-length = 88
+line-length = 120
 select = [
   "F",    # Pyflakes
   "E",    # pycodestyle
   "I",    # isort
   "N",    # pep8-naming
 #  "D",    # pydocstyle
   "YTT",  # flake8-2020
@@ -79,10 +79,10 @@
   "TRY",  # tryceratops
   "FLY",  # flynt
   "NPY",  # NumPy-specific rules
   "RUF",  # Ruff-specific rules
 ]
 
 [tool.ruff.per-file-ignores]
-"src/timeoff/cli.py" = ["T201"]
+"src/timeoff/commands.py" = ["T201"]
 "src/timeoff/prompts.py" = ["T201"]
 "src/timeoff/schedules.py" = ["T201"]
```

### Comparing `timeoff-0.0.2/PKG-INFO` & `timeoff-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeoff
-Version: 0.0.2
+Version: 0.0.3
 Summary: Track vacation hours accrued.
 Project-URL: Homepage, https://github.com/tifa/timeoff
 Author-email: Tiffany Huang <hello@tifa.io>
 License: MIT
 License-File: LICENSE
 Keywords: pto,time off,vacation
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -52,15 +52,15 @@
 - View the remaining hours of PTO available to you.
 
 ## Installation
 
 To install ``timeoff``:
 
 ```console
-$ pip install git+https://github.com/tifa/timeoff
+$ pip install timeoff
 ```
 
 Documentation is in the works! Please run the `-h` help flag in the meantime. The interactive prompts will guide you through further instructions.
 
 ```console
 $ timeoff -h
 usage: timeoff [-h] {add,list,rm,settings} ...
```

