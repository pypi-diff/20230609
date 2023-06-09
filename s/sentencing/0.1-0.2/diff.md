# Comparing `tmp/sentencing-0.1-py3-none-any.whl.zip` & `tmp/sentencing-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1359 bytes, number of entries: 6
+Zip file size: 1416 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 09:14 sentencing/__init__.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-09 09:15 sentencing/example.py
--rw-r--r--  2.0 unx       73 b- defN 23-Jun-09 09:21 sentencing-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 09:21 sentencing-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-09 09:21 sentencing-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      452 b- defN 23-Jun-09 09:21 sentencing-0.1.dist-info/RECORD
-6 files, 691 bytes uncompressed, 531 bytes compressed:  23.2%
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-09 09:38 sentencing/example.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-09 09:39 sentencing-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 09:39 sentencing-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-09 09:39 sentencing-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      453 b- defN 23-Jun-09 09:39 sentencing-0.2.dist-info/RECORD
+6 files, 788 bytes uncompressed, 588 bytes compressed:  25.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sentencing/__init__.py
 Comment: 
 
 Filename: sentencing/example.py
 Comment: 
 
-Filename: sentencing-0.1.dist-info/METADATA
+Filename: sentencing-0.2.dist-info/METADATA
 Comment: 
 
-Filename: sentencing-0.1.dist-info/WHEEL
+Filename: sentencing-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sentencing-0.1.dist-info/top_level.txt
+Filename: sentencing-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sentencing-0.1.dist-info/RECORD
+Filename: sentencing-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sentencing/example.py

```diff
@@ -1,2 +1,7 @@
-def sentence_to_words(s: str) -> list:
-    return s.split(" ")
+class SentenceModel:
+    def __init__(self) -> None:
+        pass
+
+    @staticmethod   
+    def sentence_to_words(s: str) -> list:
+        return s.split(" ")
```

