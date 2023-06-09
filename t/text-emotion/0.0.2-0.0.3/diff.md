# Comparing `tmp/text_emotion-0.0.2.tar.gz` & `tmp/text_emotion-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_emotion-0.0.2.tar", max compression
+gzip compressed data, was "text_emotion-0.0.3.tar", max compression
```

## Comparing `text_emotion-0.0.2.tar` & `text_emotion-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-27 19:48:12.166350 text_emotion-0.0.2/LICENSE
--rw-r--r--   0        0        0      288 2023-06-06 01:35:51.881314 text_emotion-0.0.2/README.md
--rw-r--r--   0        0        0      703 2023-06-06 01:55:24.543745 text_emotion-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-06 01:28:21.574005 text_emotion-0.0.2/src/text_emotion/__init__.py
--rw-r--r--   0        0        0     3297 2023-06-06 01:43:03.292148 text_emotion-0.0.2/src/text_emotion/emotion.py
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 text_emotion-0.0.2/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 text_emotion-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-27 19:48:12.166350 text_emotion-0.0.3/LICENSE
+-rw-r--r--   0        0        0      836 2023-06-09 20:13:36.160154 text_emotion-0.0.3/README.md
+-rw-r--r--   0        0        0      866 2023-06-09 20:16:33.165531 text_emotion-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-06 01:28:21.574005 text_emotion-0.0.3/src/text_emotion/__init__.py
+-rw-r--r--   0        0        0     4967 2023-06-09 20:13:11.354208 text_emotion-0.0.3/src/text_emotion/emotion.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 text_emotion-0.0.3/setup.py
+-rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 text_emotion-0.0.3/PKG-INFO
```

### Comparing `text_emotion-0.0.2/LICENSE` & `text_emotion-0.0.3/LICENSE`

 * *Files identical despite different names*

