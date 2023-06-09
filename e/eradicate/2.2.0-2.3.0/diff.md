# Comparing `tmp/eradicate-2.2.0.tar.gz` & `tmp/eradicate-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradicate-2.2.0.tar", last modified: Wed Mar  1 08:36:23 2023, max compression
+gzip compressed data, was "eradicate-2.3.0.tar", last modified: Fri Jun  9 06:30:42 2023, max compression
```

## Comparing `eradicate-2.2.0.tar` & `eradicate-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-03-01 08:36:23.662622 eradicate-2.2.0/
--rw-r--r--   0 sobolev    (501) staff       (20)       56 2023-03-01 08:32:23.000000 eradicate-2.2.0/MANIFEST.in
--rw-r--r--   0 sobolev    (501) staff       (20)     2547 2023-03-01 08:36:23.661794 eradicate-2.2.0/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)     1987 2023-03-01 08:32:23.000000 eradicate-2.2.0/README.rst
--rwxr-xr-x   0 sobolev    (501) staff       (20)     1659 2023-03-01 08:32:23.000000 eradicate-2.2.0/eradicate
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-03-01 08:36:23.659972 eradicate-2.2.0/eradicate.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)     2547 2023-03-01 08:36:23.000000 eradicate-2.2.0/eradicate.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      186 2023-03-01 08:36:23.000000 eradicate-2.2.0/eradicate.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-03-01 08:36:23.000000 eradicate-2.2.0/eradicate.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-03-01 08:36:23.000000 eradicate-2.2.0/eradicate.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)    11563 2023-03-01 08:35:41.000000 eradicate-2.2.0/eradicate.py
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-03-01 08:36:23.663413 eradicate-2.2.0/setup.cfg
--rwxr-xr-x   0 sobolev    (501) staff       (20)     1206 2023-03-01 08:35:41.000000 eradicate-2.2.0/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-09 06:30:42.625721 eradicate-2.3.0/
+-rw-r--r--   0 sobolev    (501) staff       (20)       82 2023-06-08 16:50:05.000000 eradicate-2.3.0/MANIFEST.in
+-rw-r--r--   0 sobolev    (501) staff       (20)     2547 2023-06-09 06:30:42.625560 eradicate-2.3.0/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)     1987 2023-06-08 16:50:05.000000 eradicate-2.3.0/README.rst
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-09 06:30:42.625341 eradicate-2.3.0/eradicate.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)     2547 2023-06-09 06:30:42.000000 eradicate-2.3.0/eradicate.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      230 2023-06-09 06:30:42.000000 eradicate-2.3.0/eradicate.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-06-09 06:30:42.000000 eradicate-2.3.0/eradicate.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       45 2023-06-09 06:30:42.000000 eradicate-2.3.0/eradicate.egg-info/entry_points.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-06-09 06:30:42.000000 eradicate-2.3.0/eradicate.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)    11748 2023-06-09 06:24:48.000000 eradicate-2.3.0/eradicate.py
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-06-09 06:30:42.625765 eradicate-2.3.0/setup.cfg
+-rwxr-xr-x   0 sobolev    (501) staff       (20)     1309 2023-06-08 16:50:05.000000 eradicate-2.3.0/setup.py
+-rwxr-xr-x   0 sobolev    (501) staff       (20)    19826 2023-06-09 06:24:34.000000 eradicate-2.3.0/test_eradicate.py
```

### Comparing `eradicate-2.2.0/PKG-INFO` & `eradicate-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradicate
-Version: 2.2.0
+Version: 2.3.0
 Summary: Removes commented-out code.
 Home-page: https://github.com/myint/eradicate
 Author: Steven Myint
 Maintainer: Nikita Sobolev <mail@sobolevn.me>
 License: Expat License
 Keywords: clean,format,commented-out code
 Classifier: Environment :: Console
```

### Comparing `eradicate-2.2.0/README.rst` & `eradicate-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `eradicate-2.2.0/eradicate.egg-info/PKG-INFO` & `eradicate-2.3.0/eradicate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradicate
-Version: 2.2.0
+Version: 2.3.0
 Summary: Removes commented-out code.
 Home-page: https://github.com/myint/eradicate
 Author: Steven Myint
 Maintainer: Nikita Sobolev <mail@sobolevn.me>
 License: Expat License
 Keywords: clean,format,commented-out code
 Classifier: Environment :: Console
```

### Comparing `eradicate-2.2.0/eradicate.py` & `eradicate-2.3.0/eradicate.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,25 @@
 
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import difflib
 import io
 import os
+import sys
 import re
 import tokenize
 
-__version__ = '2.2.0'
+try:
+    detect_encoding = tokenize.detect_encoding
+except AttributeError:
+    from lib2to3.pgen2 import tokenize as lib2to3_tokenize
+    detect_encoding = lib2to3_tokenize.detect_encoding
+
+__version__ = '2.3.0'
 
 
 class Eradicator(object):
     """Eradicate comments."""
     BRACKET_REGEX = re.compile(r'^[()\[\]{}\s]+$')
     CODING_COMMENT_REGEX = re.compile(r'.*?coding[:=][ \t]*([-_.a-zA-Z0-9]+)')
     DEF_STATEMENT_REGEX = re.compile(r"def .+\)[\s]+->[\s]+[a-zA-Z_][a-zA-Z0-9_]*:$")
@@ -209,16 +216,15 @@
                        newline='')  # Preserve line endings
 
 
     def detect_encoding(self, filename):
         """Return file encoding."""
         try:
             with open(filename, 'rb') as input_file:
-                from lib2to3.pgen2 import tokenize as lib2to3_tokenize
-                encoding = lib2to3_tokenize.detect_encoding(input_file.readline)[0]
+                encoding = detect_encoding(input_file.readline)[0]
 
                 # Check for correctness of encoding.
                 with self.open_with_encoding(filename, encoding) as input_file:
                     input_file.read()
 
             return encoding
         except (SyntaxError, LookupError, UnicodeDecodeError):
@@ -232,15 +238,15 @@
                 flags=re.IGNORECASE)
         else:
             self.WHITELIST_REGEX = re.compile(
                 r'|'.join(new_whitelist),
                 flags=re.IGNORECASE)
 
 
-def main(argv, standard_out, standard_error):
+def main(argv=sys.argv, standard_out=sys.stdout, standard_error=sys.stderr):
     """Main entry point."""
     import argparse
     parser = argparse.ArgumentParser(description=__doc__, prog='eradicate')
     parser.add_argument('-i', '--in-place', action='store_true',
                         help='make changes to files instead of printing diffs')
     parser.add_argument('-r', '--recursive', action='store_true',
                         help='drill down directories recursively')
@@ -288,9 +294,14 @@
                                   if not d.startswith('.')]
         else:
             try:
                 change_or_error = eradicator.fix_file(name, args=args, standard_out=standard_out) or change_or_error
             except IOError as exception:
                 print('{}'.format(exception), file=standard_error)
                 change_or_error = True
+
     if change_or_error and args.error:
         return 1
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `eradicate-2.2.0/setup.py` & `eradicate-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,13 @@
                      'Intended Audience :: Developers',
                      'License :: OSI Approved :: MIT License',
                      'Programming Language :: Python :: 2.7',
                      'Programming Language :: Python :: 3',
                      'Topic :: Software Development :: Quality Assurance'],
         keywords='clean, format, commented-out code',
         py_modules=['eradicate'],
-        scripts=['eradicate'])
+        entry_points={
+            'console_scripts': [
+                'eradicate = eradicate:main',
+            ],
+        },
+    )
```

