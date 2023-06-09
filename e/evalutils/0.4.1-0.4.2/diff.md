# Comparing `tmp/evalutils-0.4.1.tar.gz` & `tmp/evalutils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalutils-0.4.1.tar", max compression
+gzip compressed data, was "evalutils-0.4.2.tar", max compression
```

## Comparing `evalutils-0.4.1.tar` & `evalutils-0.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1086 2023-05-11 08:32:51.617926 evalutils-0.4.1/LICENSE
--rw-r--r--   0        0        0     1512 2023-05-11 08:32:51.617926 evalutils-0.4.1/README.md
--rw-r--r--   0        0        0      356 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/__init__.py
--rw-r--r--   0        0        0       82 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/__main__.py
--rw-r--r--   0        0        0     3938 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/annotations.py
--rw-r--r--   0        0        0     6632 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/cli.py
--rw-r--r--   0        0        0    23270 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/evalutils.py
--rw-r--r--   0        0        0      195 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/exceptions.py
--rw-r--r--   0        0        0     4094 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/io.py
--rw-r--r--   0        0        0    10237 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/roc.py
--rw-r--r--   0        0        0     3827 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/scorers.py
--rw-r--r--   0        0        0    29369 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/stats.py
--rw-r--r--   0        0        0        0 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/__init__.py
--rw-r--r--   0        0        0      414 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/__init__.py
--rw-r--r--   0        0        0     2124 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/post_gen_project.py
--rw-r--r--   0        0        0      340 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/hooks/pre_gen_project.py
--rw-r--r--   0        0        0       21 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.dockerignore
--rw-r--r--   0        0        0       94 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitattributes.j2
--rw-r--r--   0        0        0      555 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1190 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore
--rw-r--r--   0        0        0      965 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile
--rw-r--r--   0        0        0      354 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/README.md
--rw-r--r--   0        0        0      466 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0   372164 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      336 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_classification.json
--rw-r--r--   0        0        0     1849 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json
--rw-r--r--   0        0        0      418 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_segmentation.json
--rwxr-xr-x   0        0        0      137 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/build.sh
--rw-r--r--   0        0        0     4438 2023-05-11 08:32:51.617926 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2
--rw-r--r--   0        0        0      408 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0   529641 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      397 2023-05-11 08:32:51.621927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
--rw-r--r--   0        0        0   414098 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
--rw-r--r--   0        0        0      358 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/detection-submission.csv
--rw-r--r--   0        0        0       52 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/submission.csv
--rwxr-xr-x   0        0        0      134 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/export.sh
--rw-r--r--   0        0        0      415 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
--rw-r--r--   0        0        0  1014889 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
--rw-r--r--   0        0        0      403 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
--rw-r--r--   0        0        0   806220 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
--rw-r--r--   0        0        0      154 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/detection-reference.csv
--rw-r--r--   0        0        0       52 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/reference.csv
--rw-r--r--   0        0        0     2691 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2
--rw-r--r--   0        0        0      106 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/requirements.in
--rwxr-xr-x   0        0        0     2122 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh
--rw-r--r--   0        0        0     1240 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/utils.py
--rw-r--r--   0        0        0     4408 2023-05-11 08:32:51.625927 evalutils-0.4.1/evalutils/validators.py
--rw-r--r--   0        0        0     2115 2023-05-11 08:32:51.625927 evalutils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 evalutils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-09 10:13:06.782487 evalutils-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1512 2023-06-09 10:13:06.782487 evalutils-0.4.2/README.md
+-rw-r--r--   0        0        0      356 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/__main__.py
+-rw-r--r--   0        0        0     3938 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/annotations.py
+-rw-r--r--   0        0        0     6632 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/cli.py
+-rw-r--r--   0        0        0    23715 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/evalutils.py
+-rw-r--r--   0        0        0      195 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/exceptions.py
+-rw-r--r--   0        0        0     4107 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/io.py
+-rw-r--r--   0        0        0    10237 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/roc.py
+-rw-r--r--   0        0        0     3827 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/scorers.py
+-rw-r--r--   0        0        0    29369 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/stats.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/hooks/__init__.py
+-rw-r--r--   0        0        0     2124 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      340 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0       21 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.dockerignore
+-rw-r--r--   0        0        0       94 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitattributes.j2
+-rw-r--r--   0        0        0      555 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1190 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore
+-rw-r--r--   0        0        0      965 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile
+-rw-r--r--   0        0        0      354 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/README.md
+-rw-r--r--   0        0        0      466 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0   372164 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      336 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_classification.json
+-rw-r--r--   0        0        0     1849 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json
+-rw-r--r--   0        0        0      418 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_segmentation.json
+-rwxr-xr-x   0        0        0      137 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/build.sh
+-rw-r--r--   0        0        0     4438 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2
+-rw-r--r--   0        0        0      408 2023-06-09 10:13:06.786487 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0   529641 2023-06-09 10:13:06.790488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      397 2023-06-09 10:13:06.790488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
+-rw-r--r--   0        0        0   414098 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
+-rw-r--r--   0        0        0      358 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/detection-submission.csv
+-rw-r--r--   0        0        0       52 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/submission.csv
+-rwxr-xr-x   0        0        0      134 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/export.sh
+-rw-r--r--   0        0        0      415 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.mhd
+-rw-r--r--   0        0        0  1014889 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw
+-rw-r--r--   0        0        0      403 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.mhd
+-rw-r--r--   0        0        0   806220 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw
+-rw-r--r--   0        0        0      154 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/detection-reference.csv
+-rw-r--r--   0        0        0       52 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/reference.csv
+-rw-r--r--   0        0        0     2691 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2
+-rw-r--r--   0        0        0      106 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/requirements.in
+-rwxr-xr-x   0        0        0     2122 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh
+-rw-r--r--   0        0        0     1240 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/utils.py
+-rw-r--r--   0        0        0     4408 2023-06-09 10:13:06.794488 evalutils-0.4.2/evalutils/validators.py
+-rw-r--r--   0        0        0     2115 2023-06-09 10:13:06.794488 evalutils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 evalutils-0.4.2/PKG-INFO
```

### Comparing `evalutils-0.4.1/LICENSE` & `evalutils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/README.md` & `evalutils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/annotations.py` & `evalutils-0.4.2/evalutils/annotations.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/cli.py` & `evalutils-0.4.2/evalutils/cli.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/evalutils.py` & `evalutils-0.4.2/evalutils/evalutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,16 +582,22 @@
             if self._join_key:
                 extra = [p[self._join_key] for p in extra]
             self._raise_extra_predictions_error(extra=extra)
 
     def score(self):
         self._case_results = DataFrame()
         for idx, case in self._cases.iterrows():
-            self._case_results = self._case_results.append(
-                self.score_case(idx=idx, case=case), ignore_index=True
+            self._case_results = concat(
+                [
+                    self._case_results,
+                    DataFrame.from_records(
+                        [self.score_case(idx=idx, case=case)]
+                    ),
+                ],
+                ignore_index=True,
             )
         self._aggregate_results = self.score_aggregates()
 
 
 class Evaluation(ClassificationEvaluation):
     """
     Legacy class, you should use ClassificationEvaluation instead.
@@ -649,19 +655,28 @@
     def score(self):
         cases = set(self._ground_truth_cases[self._join_key])
         cases |= set(self._predictions_cases[self._join_key])
 
         self._case_results = DataFrame()
 
         for idx, case in enumerate(cases):
-            self._case_results = self._case_results.append(
-                self.score_case(
-                    idx=idx,
-                    case=self._cases.loc[self._cases[self._join_key] == case],
-                ),
+            self._case_results = concat(
+                [
+                    self._case_results,
+                    DataFrame.from_records(
+                        [
+                            self.score_case(
+                                idx=idx,
+                                case=self._cases.loc[
+                                    self._cases[self._join_key] == case
+                                ],
+                            )
+                        ]
+                    ),
+                ],
                 ignore_index=True,
             )
         self._aggregate_results = self.score_aggregates()
 
     def score_case(self, *, idx, case):
         score = score_detection(
             ground_truth=self.get_points(case=case, key="ground_truth"),
```

### Comparing `evalutils-0.4.1/evalutils/io.py` & `evalutils-0.4.2/evalutils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         raise NotImplementedError
 
 
 class ImageIOLoader(ImageLoader):
     @staticmethod
     def load_image(fname):
         with open(fname, "rb") as f:
-            with get_reader(f, mode="i") as r:
+            with get_reader(f, mode="i", pilmode="F") as r:
                 return r.get_data(0)
 
     @staticmethod
     def hash_image(image):
         return hash(image.tobytes())
```

### Comparing `evalutils-0.4.1/evalutils/roc.py` & `evalutils-0.4.2/evalutils/roc.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/scorers.py` & `evalutils-0.4.2/evalutils/scorers.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/stats.py` & `evalutils-0.4.2/evalutils/stats.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/hooks/post_gen_project.py` & `evalutils-0.4.2/evalutils/templates/container/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/Dockerfile`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/algorithm_test/results_detection.json`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation.py.j2`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/evaluation_test/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.0.000.000000.0.00.0.0000000000.0000.0000000000.000.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/ground-truth/1.2.276.0.28.3.0.14.4.0.20090213134050413.zraw`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/process.py.j2`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh` & `evalutils-0.4.2/evalutils/templates/container/{{ cookiecutter.package_name }}/test.sh`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/utils.py` & `evalutils-0.4.2/evalutils/utils.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/evalutils/validators.py` & `evalutils-0.4.2/evalutils/validators.py`

 * *Files identical despite different names*

### Comparing `evalutils-0.4.1/pyproject.toml` & `evalutils-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evalutils"
-version = "0.4.1"
+version = "0.4.2"
 description = "evalutils helps users create extensions for grand-challenge.org"
 authors = ["James Meakin <evalutils@jmsmkn.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/comic/evalutils"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -14,25 +14,25 @@
 ]
 
 [tool.poetry.scripts]
 evalutils = "evalutils.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-imageio = { version = "*", extras=["tifffile"] }
+imageio = { version = ">=2.31", extras=["tifffile"] }
 # Exclude 2.1.1.1 due to
 # https://github.com/SimpleITK/SimpleITK/issues/1627
 # and https://github.com/python-poetry/poetry/issues/2453
 SimpleITK = ">=2.0,!=2.1.1.1"
 cookiecutter = "*"
 click = "*"
 scipy = "*"
 scikit-learn = "*"
 numpy = ">=1.22"
-pandas = ">=1.3,<2.0"
+pandas = ">=1.3"
 pip-tools = ">=6"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-xdist = "*"
 pytest-randomly = "*"
 pytest-cov = "*"
```

### Comparing `evalutils-0.4.1/PKG-INFO` & `evalutils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: evalutils helps users create extensions for grand-challenge.org
 Home-page: https://github.com/comic/evalutils
 License: MIT
 Author: James Meakin
 Author-email: evalutils@jmsmkn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SimpleITK (>=2.0,!=2.1.1.1)
 Requires-Dist: click
 Requires-Dist: cookiecutter
-Requires-Dist: imageio[tifffile]
+Requires-Dist: imageio[tifffile] (>=2.31)
 Requires-Dist: numpy (>=1.22)
-Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pandas (>=1.3)
 Requires-Dist: pip-tools (>=6)
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Project-URL: Repository, https://github.com/comic/evalutils
 Description-Content-Type: text/markdown
 
 # evalutils
```

