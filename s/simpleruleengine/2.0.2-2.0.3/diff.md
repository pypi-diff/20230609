# Comparing `tmp/simpleruleengine-2.0.2.tar.gz` & `tmp/simpleruleengine-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jeyab\PycharmProjects\simple-rule-engine\dist\tmpqfi76tj6\simpleruleengine-2.0.2.tar", last modified: Tue Nov  1 15:17:43 2022, max compression
+gzip compressed data, was "C:\Users\jeyab\PycharmProjects\simple-rule-engine\dist\.tmp-7xliy4jt\simpleruleengine-2.0.3.tar", last modified: Fri Jun  9 06:13:30 2023, max compression
```

## Comparing `simpleruleengine-2.0.2.tar` & `simpleruleengine-2.0.3.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/
--rw-rw-rw-   0        0        0     1091 2022-09-25 05:01:13.000000 simpleruleengine-2.0.2/LICENSE
--rw-rw-rw-   0        0        0    26557 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    25931 2022-11-01 15:16:19.000000 simpleruleengine-2.0.2/README.md
--rw-rw-rw-   0        0        0     1070 2022-11-01 15:13:43.000000 simpleruleengine-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/
--rw-rw-rw-   0        0        0        0 2020-11-08 10:14:48.000000 simpleruleengine-2.0.2/simpleruleengine/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/conditional/
--rw-rw-rw-   0        0        0        0 2020-11-11 02:22:14.000000 simpleruleengine-2.0.2/simpleruleengine/conditional/__init__.py
--rw-rw-rw-   0        0        0     1107 2022-09-25 11:02:30.000000 simpleruleengine-2.0.2/simpleruleengine/conditional/conditional.py
--rw-rw-rw-   0        0        0      559 2022-09-25 11:02:50.000000 simpleruleengine-2.0.2/simpleruleengine/conditional/when_all.py
--rw-rw-rw-   0        0        0      559 2022-09-25 11:03:06.000000 simpleruleengine-2.0.2/simpleruleengine/conditional/when_any.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/exception/
--rw-rw-rw-   0        0        0        0 2022-09-15 04:29:03.000000 simpleruleengine-2.0.2/simpleruleengine/exception/__init__.py
--rw-rw-rw-   0        0        0       58 2022-09-15 04:32:41.000000 simpleruleengine-2.0.2/simpleruleengine/exception/rule_row_exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/expression/
--rw-rw-rw-   0        0        0        0 2022-09-23 04:54:08.000000 simpleruleengine-2.0.2/simpleruleengine/expression/__init__.py
--rw-rw-rw-   0        0        0      381 2022-09-25 07:35:39.000000 simpleruleengine-2.0.2/simpleruleengine/expression/expression.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/operator/
--rw-rw-rw-   0        0        0        0 2020-11-10 06:35:46.000000 simpleruleengine-2.0.2/simpleruleengine/operator/__init__.py
--rw-rw-rw-   0        0        0      448 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/between.py
--rw-rw-rw-   0        0        0      751 2022-11-01 15:12:15.000000 simpleruleengine-2.0.2/simpleruleengine/operator/boolean_operator.py
--rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/equal.py
--rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/greater_than.py
--rw-rw-rw-   0        0        0      309 2022-09-25 07:28:45.000000 simpleruleengine-2.0.2/simpleruleengine/operator/greater_than_equal.py
--rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/less_than.py
--rw-rw-rw-   0        0        0      309 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/less_than_equal.py
--rw-rw-rw-   0        0        0      772 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/numeric_operator.py
--rw-rw-rw-   0        0        0      144 2020-11-10 06:47:25.000000 simpleruleengine-2.0.2/simpleruleengine/operator/operator.py
--rw-rw-rw-   0        0        0      276 2022-09-25 07:28:44.000000 simpleruleengine-2.0.2/simpleruleengine/operator/string_in.py
--rw-rw-rw-   0        0        0      283 2022-09-25 11:06:08.000000 simpleruleengine-2.0.2/simpleruleengine/operator/string_not_in.py
--rw-rw-rw-   0        0        0      834 2022-09-25 07:41:56.000000 simpleruleengine-2.0.2/simpleruleengine/operator/string_operator.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/rule/
--rw-rw-rw-   0        0        0        0 2020-11-19 06:36:31.000000 simpleruleengine-2.0.2/simpleruleengine/rule/__init__.py
--rw-rw-rw-   0        0        0      479 2022-09-25 11:14:45.000000 simpleruleengine-2.0.2/simpleruleengine/rule/rule.py
--rw-rw-rw-   0        0        0      677 2022-09-25 11:26:08.000000 simpleruleengine-2.0.2/simpleruleengine/rule/rule_decision.py
--rw-rw-rw-   0        0        0      675 2022-09-25 11:14:31.000000 simpleruleengine-2.0.2/simpleruleengine/rule/rule_score.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/rulerow/
--rw-rw-rw-   0        0        0        0 2020-12-07 01:01:25.000000 simpleruleengine-2.0.2/simpleruleengine/rulerow/__init__.py
--rw-rw-rw-   0        0        0      768 2022-09-22 05:04:07.000000 simpleruleengine-2.0.2/simpleruleengine/rulerow/rule_row_decision.py
--rw-rw-rw-   0        0        0     1052 2022-09-22 05:04:07.000000 simpleruleengine-2.0.2/simpleruleengine/rulerow/rule_row_score.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/ruleset/
--rw-rw-rw-   0        0        0        0 2020-12-07 01:02:04.000000 simpleruleengine-2.0.2/simpleruleengine/ruleset/__init__.py
--rw-rw-rw-   0        0        0      956 2022-09-25 11:13:37.000000 simpleruleengine-2.0.2/simpleruleengine/ruleset/rule_set_decision.py
--rw-rw-rw-   0        0        0     1303 2022-09-25 11:17:59.000000 simpleruleengine-2.0.2/simpleruleengine/ruleset/rule_set_score.py
--rw-rw-rw-   0        0        0     1931 2022-11-01 15:11:57.000000 simpleruleengine-2.0.2/simpleruleengine/test_expression.py
--rw-rw-rw-   0        0        0     1022 2022-11-01 15:10:52.000000 simpleruleengine-2.0.2/simpleruleengine/test_operator.py
--rw-rw-rw-   0        0        0     2012 2022-09-25 11:24:19.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_decision.py
--rw-rw-rw-   0        0        0      897 2022-09-25 10:49:40.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_row_decision.py
--rw-rw-rw-   0        0        0     1318 2022-09-25 10:59:19.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_row_score.py
--rw-rw-rw-   0        0        0     3669 2022-09-25 11:21:13.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_score.py
--rw-rw-rw-   0        0        0     4401 2022-09-25 11:15:46.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_set_decision.py
--rw-rw-rw-   0        0        0     5670 2022-09-25 11:20:00.000000 simpleruleengine-2.0.2/simpleruleengine/test_rule_set_score.py
--rw-rw-rw-   0        0        0     2130 2022-09-25 11:10:49.000000 simpleruleengine-2.0.2/simpleruleengine/test_when_all.py
--rw-rw-rw-   0        0        0     2481 2022-09-25 11:11:53.000000 simpleruleengine-2.0.2/simpleruleengine/test_when_any.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/token/
--rw-rw-rw-   0        0        0        0 2020-11-10 06:31:36.000000 simpleruleengine-2.0.2/simpleruleengine/token/__init__.py
--rw-rw-rw-   0        0        0      390 2022-10-29 14:09:57.000000 simpleruleengine-2.0.2/simpleruleengine/token/boolean_token.py
--rw-rw-rw-   0        0        0      390 2022-09-25 07:35:39.000000 simpleruleengine-2.0.2/simpleruleengine/token/numeric_token.py
--rw-rw-rw-   0        0        0      430 2022-09-25 07:35:39.000000 simpleruleengine-2.0.2/simpleruleengine/token/rule_token.py
--rw-rw-rw-   0        0        0      387 2022-09-25 07:35:39.000000 simpleruleengine-2.0.2/simpleruleengine/token/string_token.py
--rw-rw-rw-   0        0        0      485 2022-09-23 05:32:06.000000 simpleruleengine-2.0.2/simpleruleengine/token/token.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine/utils/
--rw-rw-rw-   0        0        0        0 2020-11-10 04:40:48.000000 simpleruleengine-2.0.2/simpleruleengine/utils/__init__.py
--rw-rw-rw-   0        0        0      874 2022-09-25 07:43:32.000000 simpleruleengine-2.0.2/simpleruleengine/utils/type_util.py
-drwxrwxrwx   0        0        0        0 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine.egg-info/
--rw-rw-rw-   0        0        0    26557 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-11-01 15:17:43.000000 simpleruleengine-2.0.2/simpleruleengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/
+-rw-rw-rw-   0        0        0     1091 2022-09-25 05:01:13.000000 simpleruleengine-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4026 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3400 2023-06-01 04:25:29.000000 simpleruleengine-2.0.3/README.md
+-rw-rw-rw-   0        0        0     1070 2023-06-09 05:56:58.000000 simpleruleengine-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/
+-rw-rw-rw-   0        0        0        0 2020-11-08 10:14:48.000000 simpleruleengine-2.0.3/simpleruleengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/conditional/
+-rw-rw-rw-   0        0        0        0 2020-11-11 02:22:14.000000 simpleruleengine-2.0.3/simpleruleengine/conditional/__init__.py
+-rw-rw-rw-   0        0        0     1107 2022-09-25 11:02:30.000000 simpleruleengine-2.0.3/simpleruleengine/conditional/conditional.py
+-rw-rw-rw-   0        0        0      559 2022-09-25 11:02:50.000000 simpleruleengine-2.0.3/simpleruleengine/conditional/when_all.py
+-rw-rw-rw-   0        0        0      559 2022-09-25 11:03:06.000000 simpleruleengine-2.0.3/simpleruleengine/conditional/when_any.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/exception/
+-rw-rw-rw-   0        0        0        0 2022-09-15 04:29:03.000000 simpleruleengine-2.0.3/simpleruleengine/exception/__init__.py
+-rw-rw-rw-   0        0        0       58 2022-09-15 04:32:41.000000 simpleruleengine-2.0.3/simpleruleengine/exception/rule_row_exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/expression/
+-rw-rw-rw-   0        0        0        0 2022-09-23 04:54:08.000000 simpleruleengine-2.0.3/simpleruleengine/expression/__init__.py
+-rw-rw-rw-   0        0        0      381 2022-09-25 07:35:39.000000 simpleruleengine-2.0.3/simpleruleengine/expression/expression.py
+-rw-rw-rw-   0        0        0     1633 2023-06-01 05:18:15.000000 simpleruleengine-2.0.3/simpleruleengine/expression/expression_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/operator/
+-rw-rw-rw-   0        0        0        0 2020-11-10 06:35:46.000000 simpleruleengine-2.0.3/simpleruleengine/operator/__init__.py
+-rw-rw-rw-   0        0        0      448 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/between.py
+-rw-rw-rw-   0        0        0      751 2022-11-01 15:12:15.000000 simpleruleengine-2.0.3/simpleruleengine/operator/boolean_operator.py
+-rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/equal.py
+-rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/greater_than.py
+-rw-rw-rw-   0        0        0      309 2022-09-25 07:28:45.000000 simpleruleengine-2.0.3/simpleruleengine/operator/greater_than_equal.py
+-rw-rw-rw-   0        0        0      308 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/less_than.py
+-rw-rw-rw-   0        0        0      309 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/less_than_equal.py
+-rw-rw-rw-   0        0        0      330 2023-06-09 05:49:45.000000 simpleruleengine-2.0.3/simpleruleengine/operator/not_equal.py
+-rw-rw-rw-   0        0        0      772 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/numeric_operator.py
+-rw-rw-rw-   0        0        0      144 2020-11-10 06:47:25.000000 simpleruleengine-2.0.3/simpleruleengine/operator/operator.py
+-rw-rw-rw-   0        0        0      276 2022-09-25 07:28:44.000000 simpleruleengine-2.0.3/simpleruleengine/operator/string_in.py
+-rw-rw-rw-   0        0        0      283 2022-09-25 11:06:08.000000 simpleruleengine-2.0.3/simpleruleengine/operator/string_not_in.py
+-rw-rw-rw-   0        0        0      834 2022-09-25 07:41:56.000000 simpleruleengine-2.0.3/simpleruleengine/operator/string_operator.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/rule/
+-rw-rw-rw-   0        0        0        0 2020-11-19 06:36:31.000000 simpleruleengine-2.0.3/simpleruleengine/rule/__init__.py
+-rw-rw-rw-   0        0        0      479 2022-09-25 11:14:45.000000 simpleruleengine-2.0.3/simpleruleengine/rule/rule.py
+-rw-rw-rw-   0        0        0      677 2022-09-25 11:26:08.000000 simpleruleengine-2.0.3/simpleruleengine/rule/rule_decision.py
+-rw-rw-rw-   0        0        0      675 2022-09-25 11:14:31.000000 simpleruleengine-2.0.3/simpleruleengine/rule/rule_score.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/rulerow/
+-rw-rw-rw-   0        0        0        0 2020-12-07 01:01:25.000000 simpleruleengine-2.0.3/simpleruleengine/rulerow/__init__.py
+-rw-rw-rw-   0        0        0      768 2022-09-22 05:04:07.000000 simpleruleengine-2.0.3/simpleruleengine/rulerow/rule_row_decision.py
+-rw-rw-rw-   0        0        0     1052 2022-09-22 05:04:07.000000 simpleruleengine-2.0.3/simpleruleengine/rulerow/rule_row_score.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/ruleset/
+-rw-rw-rw-   0        0        0        0 2020-12-07 01:02:04.000000 simpleruleengine-2.0.3/simpleruleengine/ruleset/__init__.py
+-rw-rw-rw-   0        0        0      956 2022-09-25 11:13:37.000000 simpleruleengine-2.0.3/simpleruleengine/ruleset/rule_set_decision.py
+-rw-rw-rw-   0        0        0     1303 2022-09-25 11:17:59.000000 simpleruleengine-2.0.3/simpleruleengine/ruleset/rule_set_score.py
+-rw-rw-rw-   0        0        0     2193 2023-06-09 06:00:16.000000 simpleruleengine-2.0.3/simpleruleengine/test_expression.py
+-rw-rw-rw-   0        0        0      737 2023-06-01 05:14:14.000000 simpleruleengine-2.0.3/simpleruleengine/test_expression_builder.py
+-rw-rw-rw-   0        0        0     1354 2023-06-09 05:55:06.000000 simpleruleengine-2.0.3/simpleruleengine/test_operator.py
+-rw-rw-rw-   0        0        0     2012 2022-09-25 11:24:19.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_decision.py
+-rw-rw-rw-   0        0        0      897 2022-09-25 10:49:40.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_row_decision.py
+-rw-rw-rw-   0        0        0     1318 2022-09-25 10:59:19.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_row_score.py
+-rw-rw-rw-   0        0        0     3669 2022-09-25 11:21:13.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_score.py
+-rw-rw-rw-   0        0        0     4401 2022-09-25 11:15:46.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_set_decision.py
+-rw-rw-rw-   0        0        0     5670 2022-09-25 11:20:00.000000 simpleruleengine-2.0.3/simpleruleengine/test_rule_set_score.py
+-rw-rw-rw-   0        0        0     2130 2022-09-25 11:10:49.000000 simpleruleengine-2.0.3/simpleruleengine/test_when_all.py
+-rw-rw-rw-   0        0        0     2481 2022-09-25 11:11:53.000000 simpleruleengine-2.0.3/simpleruleengine/test_when_any.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/token/
+-rw-rw-rw-   0        0        0        0 2020-11-10 06:31:36.000000 simpleruleengine-2.0.3/simpleruleengine/token/__init__.py
+-rw-rw-rw-   0        0        0      390 2022-10-29 14:09:57.000000 simpleruleengine-2.0.3/simpleruleengine/token/boolean_token.py
+-rw-rw-rw-   0        0        0      390 2022-09-25 07:35:39.000000 simpleruleengine-2.0.3/simpleruleengine/token/numeric_token.py
+-rw-rw-rw-   0        0        0      430 2022-09-25 07:35:39.000000 simpleruleengine-2.0.3/simpleruleengine/token/rule_token.py
+-rw-rw-rw-   0        0        0      387 2022-09-25 07:35:39.000000 simpleruleengine-2.0.3/simpleruleengine/token/string_token.py
+-rw-rw-rw-   0        0        0      485 2022-09-23 05:32:06.000000 simpleruleengine-2.0.3/simpleruleengine/token/token.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine/utils/
+-rw-rw-rw-   0        0        0        0 2020-11-10 04:40:48.000000 simpleruleengine-2.0.3/simpleruleengine/utils/__init__.py
+-rw-rw-rw-   0        0        0      874 2022-09-25 07:43:32.000000 simpleruleengine-2.0.3/simpleruleengine/utils/type_util.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine.egg-info/
+-rw-rw-rw-   0        0        0     4026 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2297 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 06:13:30.000000 simpleruleengine-2.0.3/simpleruleengine.egg-info/top_level.txt
```

### Comparing `simpleruleengine-2.0.2/LICENSE` & `simpleruleengine-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/pyproject.toml` & `simpleruleengine-2.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simpleruleengine"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Jeyabalaji Subramanian", email="jeyabalaji.subramanian@gmail.com" },
 ]
 description = "A lightweight rule engine that allows declarative specification of business rules."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simpleruleengine-2.0.2/simpleruleengine/conditional/conditional.py` & `simpleruleengine-2.0.3/simpleruleengine/conditional/conditional.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/conditional/when_all.py` & `simpleruleengine-2.0.3/simpleruleengine/conditional/when_all.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/conditional/when_any.py` & `simpleruleengine-2.0.3/simpleruleengine/conditional/when_any.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/operator/boolean_operator.py` & `simpleruleengine-2.0.3/simpleruleengine/operator/boolean_operator.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/operator/numeric_operator.py` & `simpleruleengine-2.0.3/simpleruleengine/operator/numeric_operator.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/operator/string_operator.py` & `simpleruleengine-2.0.3/simpleruleengine/operator/string_operator.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/rule/rule_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/rule/rule_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/rule/rule_score.py` & `simpleruleengine-2.0.3/simpleruleengine/rule/rule_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/rulerow/rule_row_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/rulerow/rule_row_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/rulerow/rule_row_score.py` & `simpleruleengine-2.0.3/simpleruleengine/rulerow/rule_row_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/ruleset/rule_set_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/ruleset/rule_set_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/ruleset/rule_set_score.py` & `simpleruleengine-2.0.3/simpleruleengine/ruleset/rule_set_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_expression.py` & `simpleruleengine-2.0.3/simpleruleengine/test_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 from simpleruleengine.expression.expression import Expression
 from simpleruleengine.operator.greater_than_equal import Gte
 from simpleruleengine.operator.boolean_operator import BooleanOperator
 from simpleruleengine.operator.string_in import In
 from simpleruleengine.token.boolean_token import BooleanToken
 from simpleruleengine.token.numeric_token import NumericToken
 from simpleruleengine.token.string_token import StringToken
+from simpleruleengine.operator.equal import Eq
+from simpleruleengine.operator.not_equal import NotEq
 
 
 class TestExpression(TestCase):
     def test_evaluate_numeric_token(self):
         numeric_token_age = NumericToken(name="age")
         age_gte_35 = Expression(numeric_token_age, Gte(35))
 
         fact = dict(age=40)
 
         assert age_gte_35.evaluate(token_dict=fact) is True
 
+        assert Expression(numeric_token_age, Eq(35)).evaluate(dict(age=35))
+        assert Expression(numeric_token_age, NotEq(35)).evaluate(dict(age=40))
+
     def test_evaluate_string_token(self):
         string_token_pet = StringToken(name="pet")
         pet_in_dog_cat = Expression(string_token_pet, In("dog", "cat"))
 
         fact = dict(pet="cat")
         assert pet_in_dog_cat.evaluate(token_dict=fact) is True
```

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_operator.py` & `simpleruleengine-2.0.3/simpleruleengine/test_operator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from unittest import TestCase
 from simpleruleengine.operator.between import Between
 from simpleruleengine.operator.greater_than_equal import Gte
 from simpleruleengine.operator.string_in import In
 from simpleruleengine.operator.boolean_operator import BooleanOperator
+from simpleruleengine.operator.equal import Eq
+from simpleruleengine.operator.not_equal import NotEq
 
 
 class TestOperator(TestCase):
     def test_evaluate_between_true(self):
         assert Between(floor=650, ceiling=800).evaluate(675)
 
     def test_evaluate_between_false(self):
@@ -22,7 +24,14 @@
         assert In("dog", "cat").evaluate("dog") is True
 
     def test_evaluate_boolean_true(self):
         assert BooleanOperator(True).evaluate(True) is True
 
     def test_evaluate_boolean_false(self):
         assert BooleanOperator(False).evaluate(False) is True
+
+    def test_evaluate_equal_true(self):
+        assert Eq(2).evaluate(3) is False
+
+    def test_evaluate_not_equal_true(self):
+        assert NotEq(2).evaluate(3) is True
+        assert NotEq(2.25).evaluate(2.26) is True
```

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_row_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_row_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_row_score.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_row_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_score.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_set_decision.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_set_decision.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_rule_set_score.py` & `simpleruleengine-2.0.3/simpleruleengine/test_rule_set_score.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_when_all.py` & `simpleruleengine-2.0.3/simpleruleengine/test_when_all.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/test_when_any.py` & `simpleruleengine-2.0.3/simpleruleengine/test_when_any.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine/utils/type_util.py` & `simpleruleengine-2.0.3/simpleruleengine/utils/type_util.py`

 * *Files identical despite different names*

### Comparing `simpleruleengine-2.0.2/simpleruleengine.egg-info/SOURCES.txt` & `simpleruleengine-2.0.3/simpleruleengine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 simpleruleengine/__init__.py
 simpleruleengine/test_expression.py
+simpleruleengine/test_expression_builder.py
 simpleruleengine/test_operator.py
 simpleruleengine/test_rule_decision.py
 simpleruleengine/test_rule_row_decision.py
 simpleruleengine/test_rule_row_score.py
 simpleruleengine/test_rule_score.py
 simpleruleengine/test_rule_set_decision.py
 simpleruleengine/test_rule_set_score.py
@@ -20,22 +21,24 @@
 simpleruleengine/conditional/conditional.py
 simpleruleengine/conditional/when_all.py
 simpleruleengine/conditional/when_any.py
 simpleruleengine/exception/__init__.py
 simpleruleengine/exception/rule_row_exceptions.py
 simpleruleengine/expression/__init__.py
 simpleruleengine/expression/expression.py
+simpleruleengine/expression/expression_builder.py
 simpleruleengine/operator/__init__.py
 simpleruleengine/operator/between.py
 simpleruleengine/operator/boolean_operator.py
 simpleruleengine/operator/equal.py
 simpleruleengine/operator/greater_than.py
 simpleruleengine/operator/greater_than_equal.py
 simpleruleengine/operator/less_than.py
 simpleruleengine/operator/less_than_equal.py
+simpleruleengine/operator/not_equal.py
 simpleruleengine/operator/numeric_operator.py
 simpleruleengine/operator/operator.py
 simpleruleengine/operator/string_in.py
 simpleruleengine/operator/string_not_in.py
 simpleruleengine/operator/string_operator.py
 simpleruleengine/rule/__init__.py
 simpleruleengine/rule/rule.py
```

