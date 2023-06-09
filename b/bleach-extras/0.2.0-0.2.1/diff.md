# Comparing `tmp/bleach_extras-0.2.0.tar.gz` & `tmp/bleach_extras-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bleach_extras-0.2.0.tar", last modified: Thu Jun  8 18:51:49 2023, max compression
+gzip compressed data, was "dist/bleach_extras-0.2.1.tar", last modified: Fri Jun  9 21:19:23 2023, max compression
```

## Comparing `bleach_extras-0.2.0.tar` & `bleach_extras-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.413172 bleach_extras-0.2.0/
--rw-r--r--   0 jvanasco   (501) admin       (80)      739 2023-06-07 22:27:27.000000 bleach_extras-0.2.0/CHANGELOG.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1487 2018-10-17 03:28:21.000000 bleach_extras-0.2.0/LICENSE
--rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 20:58:45.000000 bleach_extras-0.2.0/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     5477 2023-06-08 18:51:49.413510 bleach_extras-0.2.0/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     4642 2022-05-19 16:34:08.000000 bleach_extras-0.2.0/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-07 22:24:46.000000 bleach_extras-0.2.0/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      365 2023-06-08 18:51:49.415276 bleach_extras-0.2.0/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2082 2023-06-08 18:50:47.000000 bleach_extras-0.2.0/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.389130 bleach_extras-0.2.0/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.401618 bleach_extras-0.2.0/src/bleach_extras/
--rw-r--r--   0 jvanasco   (501) admin       (80)      522 2023-06-07 22:27:32.000000 bleach_extras-0.2.0/src/bleach_extras/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     7338 2023-06-08 18:11:06.000000 bleach_extras-0.2.0/src/bleach_extras/tag_tree_filter.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.410063 bleach_extras-0.2.0/src/bleach_extras.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)     5477 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      416 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:00:56.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)      109 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       14 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.411479 bleach_extras-0.2.0/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)    17453 2021-12-02 19:32:39.000000 bleach_extras-0.2.0/tests/test_clean.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      175 2023-06-08 18:16:02.000000 bleach_extras-0.2.0/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-07 22:24:46.000000 bleach_extras-0.2.1/pyproject.toml
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    17453 2021-12-02 19:32:39.000000 bleach_extras-0.2.1/tests/test_clean.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6310 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1487 2018-10-17 03:28:21.000000 bleach_extras-0.2.1/LICENSE
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2132 2023-06-09 21:19:16.000000 bleach_extras-0.2.1/setup.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4642 2022-05-19 16:34:08.000000 bleach_extras-0.2.1/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)      175 2023-06-08 18:16:02.000000 bleach_extras-0.2.1/tox.ini
+-rw-r--r--   0 jvanasco   (501) admin       (80)      473 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 20:58:45.000000 bleach_extras-0.2.1/MANIFEST.in
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      522 2023-06-09 21:19:16.000000 bleach_extras-0.2.1/src/bleach_extras/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7338 2023-06-08 18:11:06.000000 bleach_extras-0.2.1/src/bleach_extras/tag_tree_filter.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:16.000000 bleach_extras-0.2.1/src/bleach_extras/py.typed
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:00:56.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6310 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      109 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       14 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/top_level.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      443 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-09 21:19:23.000000 bleach_extras-0.2.1/src/bleach_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      778 2023-06-09 21:19:16.000000 bleach_extras-0.2.1/CHANGELOG.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bleach_extras-0.2.0/CHANGELOG.txt` & `bleach_extras-0.2.1/CHANGELOG.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.2.1 | 20230609
+    - added py.typed
+
 0.2.0 | 20230608
     - drop python 2.6
     - mpy
 
 0.1.3 | 20220519
 	- version pinning against bleach <5 because of incompatibilities
 	- adjusted github test matrix
```

### Comparing `bleach_extras-0.2.0/LICENSE` & `bleach_extras-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bleach_extras-0.2.0/PKG-INFO` & `bleach_extras-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: bleach_extras
-Version: 0.2.0
-Summary: some extensions for bleach
-Home-page: http://github.com/jvanasco/bleach_extras
-Author: Jonathan Vanasco
-Author-email: jonathan@findmeon.com
-License: MIT License
-Keywords: bleach html-sanitizing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
 
 `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
 use with the `bleach` library.
 
 The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
 and `cleaner_factory__strip_content`.
```

#### html2text {}

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1 Name: bleach_extras Version: 0.2.0 Summary: some
-extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
-Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
-License Keywords: bleach html-sanitizing Classifier: License :: OSI Approved ::
-MIT License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown Provides-Extra: testing License-File:
-LICENSE ![Python package](https://github.com/jvanasco/bleach_extras/workflows/
+![Python package](https://github.com/jvanasco/bleach_extras/workflows/
 Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
 "extras" and utilities paired for use with the `bleach` library. The first
 utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
 `cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
 requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
 security concerns; latter versions are not compatible due to API changes
 (future support is planned). # `TagTreeFilter`, `clean_strip_content`,
```

### Comparing `bleach_extras-0.2.0/README.md` & `bleach_extras-0.2.1/src/bleach_extras.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,126 @@
-![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
-
-`bleach_extras` is a package of *unofficial* "extras" and utilities paired for
-use with the `bleach` library.
-
-The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
-and `cleaner_factory__strip_content`.
-
-# Compatability
-
-`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`.
-Earlier versions of `bleach` have security concerns; latter versions are not
-compatible due to API changes (future support is planned).
-
-
-# `TagTreeFilter`, `clean_strip_content`, `cleaner_factory__strip_content`
-
-`clean_strip_content` is paired to `bleach.clean`; the only intended difference
-is to support the concept of stripping the content tree of tags -- not just the
-tag node itself.  `cleaner_factory__strip_content` is a factory function used to
-create configured `bleach.Cleaner` instances.
-
-`bleach` has a `strip` flag that toggles the behavior of "unsafe" tags:
-
-`strip = False` will render the tags as escaped HTML encodings, such as this
-replacement:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
-	
-`strip = True` will strip the tags, but leave the HTML within as plaintext:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
-
-Many users of `bleach` want to remove both the tag and contents of unsafe tags
-for a variety of reasons, such as:
-
-* escaping the tags make the text safe, but unreadable
-* leaving the tags' content without the tags negatively affects readability and
-  comprehension
-* leaving the tags' content allows a malicious user to still have some sort of
-  fallback payload which is displayed
-
-`clean_strip_content` is a function that mimics `bleach.clean` with a key difference:
-
-* tags destined for content stripping are fed into a `Cleaner` instance as allowed
-* the tags are stripped during the filter process via `TagTreeFilter`
-
-An expected transformation is such:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.12.bar
-
-Look at that! all the evil payload is gone, including the bitcoin wallet address
-that f---- spammers tried to slip through.
-
-## Why do this filtering with `bleach` and not something else ?
-
-Parsing/Tokenzing HTML is not very efficient. Performing this outside of `bleach`
-would require performing these operations on the HTML fragments at least twice.
-
-`bleach`'s design implementation encodes/strips 'unsafe' tags during the
-parsing/tokening process - before the plugin filtering process starts. In order
-to filter the tags out correctly, they must be allowed during the generation of
-the DOM tree, then removed during the filter step. This trips a lot of people up;
-offering this in a public library with tests that can grow is ideal.
-
-
-Example:
-
-	dangerous = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar"""
-
-	print(bleach.clean(dangerous, tags=['div', ], strip=False))
-	# foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
-
-	print(bleach.clean(dangerous, tags=['div', ], strip=True))
-	# foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
-
-	print(bleach_extras.clean_strip_content(dangerous, tags=['div'], ))
-	# foo.<div>12</div>.bar
-
-	cleaner = bleach_extras.cleaner_factory__strip_content(tags=['div'],)
-	print(cleaner.clean(dangerous))
-	# foo.<div>12</div>.bar
-
-	print(bleach_extras.clean_strip_content(dangerous, tags=['div', ], strip=True, ))
-	# foo.<div>12</div>.bar
-
-## custom replacement of stripped nodes
-
-maybe you need to replace the evil content with a warning. this "extra" has you
-covered!
-
-	dangerous2 = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");<iframe>iiffrraammee</iframe></script>2</div>.bar"""
-
-	class IFrameFilter2(bleach_extras.TagTreeFilter):
-		tags_strip_content = ('script', 'style', 'iframe')
-		tag_replace_string = "&lt;unsafe garbage/&gt;"
-
-	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
-	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
-
+Metadata-Version: 2.1
+Name: bleach-extras
+Version: 0.2.1
+Summary: some extensions for bleach
+Home-page: http://github.com/jvanasco/bleach_extras
+Author: Jonathan Vanasco
+Author-email: jonathan@findmeon.com
+License: MIT License
+Description: ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
+        
+        `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
+        use with the `bleach` library.
+        
+        The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
+        and `cleaner_factory__strip_content`.
+        
+        # Compatability
+        
+        `bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`.
+        Earlier versions of `bleach` have security concerns; latter versions are not
+        compatible due to API changes (future support is planned).
+        
+        
+        # `TagTreeFilter`, `clean_strip_content`, `cleaner_factory__strip_content`
+        
+        `clean_strip_content` is paired to `bleach.clean`; the only intended difference
+        is to support the concept of stripping the content tree of tags -- not just the
+        tag node itself.  `cleaner_factory__strip_content` is a factory function used to
+        create configured `bleach.Cleaner` instances.
+        
+        `bleach` has a `strip` flag that toggles the behavior of "unsafe" tags:
+        
+        `strip = False` will render the tags as escaped HTML encodings, such as this
+        replacement:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
+        	
+        `strip = True` will strip the tags, but leave the HTML within as plaintext:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
+        
+        Many users of `bleach` want to remove both the tag and contents of unsafe tags
+        for a variety of reasons, such as:
+        
+        * escaping the tags make the text safe, but unreadable
+        * leaving the tags' content without the tags negatively affects readability and
+          comprehension
+        * leaving the tags' content allows a malicious user to still have some sort of
+          fallback payload which is displayed
+        
+        `clean_strip_content` is a function that mimics `bleach.clean` with a key difference:
+        
+        * tags destined for content stripping are fed into a `Cleaner` instance as allowed
+        * the tags are stripped during the filter process via `TagTreeFilter`
+        
+        An expected transformation is such:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.12.bar
+        
+        Look at that! all the evil payload is gone, including the bitcoin wallet address
+        that f---- spammers tried to slip through.
+        
+        ## Why do this filtering with `bleach` and not something else ?
+        
+        Parsing/Tokenzing HTML is not very efficient. Performing this outside of `bleach`
+        would require performing these operations on the HTML fragments at least twice.
+        
+        `bleach`'s design implementation encodes/strips 'unsafe' tags during the
+        parsing/tokening process - before the plugin filtering process starts. In order
+        to filter the tags out correctly, they must be allowed during the generation of
+        the DOM tree, then removed during the filter step. This trips a lot of people up;
+        offering this in a public library with tests that can grow is ideal.
+        
+        
+        Example:
+        
+        	dangerous = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar"""
+        
+        	print(bleach.clean(dangerous, tags=['div', ], strip=False))
+        	# foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
+        
+        	print(bleach.clean(dangerous, tags=['div', ], strip=True))
+        	# foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
+        
+        	print(bleach_extras.clean_strip_content(dangerous, tags=['div'], ))
+        	# foo.<div>12</div>.bar
+        
+        	cleaner = bleach_extras.cleaner_factory__strip_content(tags=['div'],)
+        	print(cleaner.clean(dangerous))
+        	# foo.<div>12</div>.bar
+        
+        	print(bleach_extras.clean_strip_content(dangerous, tags=['div', ], strip=True, ))
+        	# foo.<div>12</div>.bar
+        
+        ## custom replacement of stripped nodes
+        
+        maybe you need to replace the evil content with a warning. this "extra" has you
+        covered!
+        
+        	dangerous2 = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");<iframe>iiffrraammee</iframe></script>2</div>.bar"""
+        
+        	class IFrameFilter2(bleach_extras.TagTreeFilter):
+        		tags_strip_content = ('script', 'style', 'iframe')
+        		tag_replace_string = "&lt;unsafe garbage/&gt;"
+        
+        	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
+        	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
+        
+        
+Keywords: bleach html-sanitizing
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+Provides-Extra: testing
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-![Python package](https://github.com/jvanasco/bleach_extras/workflows/
-Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
-"extras" and utilities paired for use with the `bleach` library. The first
-utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
-`cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
-requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
-security concerns; latter versions are not compatible due to API changes
-(future support is planned). # `TagTreeFilter`, `clean_strip_content`,
-`cleaner_factory__strip_content` `clean_strip_content` is paired to
-`bleach.clean`; the only intended difference is to support the concept of
-stripping the content tree of tags -- not just the tagÂ node itself.
+Metadata-Version: 2.1 Name: bleach-extras Version: 0.2.1 Summary: some
+extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
+Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
+License Description: ![Python package](https://github.com/jvanasco/
+bleach_extras/workflows/Python%20package/badge.svg) `bleach_extras` is a
+package of *unofficial* "extras" and utilities paired for use with the `bleach`
+library. The first utility is `TagTreeFilter` which is utilized by
+`clean_strip_content` and `cleaner_factory__strip_content`. # Compatability
+`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`. Earlier
+versions of `bleach` have security concerns; latter versions are not compatible
+due to API changes (future support is planned). # `TagTreeFilter`,
+`clean_strip_content`, `cleaner_factory__strip_content` `clean_strip_content`
+is paired to `bleach.clean`; the only intended difference is to support the
+concept of stripping the content tree of tags -- not just the tagÂ node itself.
 `cleaner_factory__strip_content` is a factory function used to create
 configured `bleach.Cleaner` instances. `bleach` has a `strip` flag that toggles
 the behavior of "unsafe" tags: `strip = False` will render the tags as escaped
 HTML encodings, such as this replacement: - foo.
 1
 2
 .bar + foo.
@@ -68,8 +71,16 @@
 1
 2
 .bar""" class IFrameFilter2(bleach_extras.TagTreeFilter): tags_strip_content =
 ('script', 'style', 'iframe') tag_replace_string = "<unsafe garbage/>" print
 bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=
 [IFrameFilter2, ]) # foo.
 1&lt;unsafe garbage/&gt;2
-.bar
+.bar Keywords: bleach html-sanitizing Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Developers Description-Content-Type: text/markdown Provides-Extra:
+testing
```

### Comparing `bleach_extras-0.2.0/setup.py` & `bleach_extras-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     zip_safe=False,
     keywords="bleach html-sanitizing",
     test_suite="tests",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"bleach_extras": ["py.typed"]},
     include_package_data=True,
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
     classifiers=[
```

### Comparing `bleach_extras-0.2.0/src/bleach_extras/__init__.py` & `bleach_extras-0.2.1/src/bleach_extras/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 from .tag_tree_filter import TAG_TREE_TAGS  # noqa: F401
 from .tag_tree_filter import TagTreeFilter  # noqa: F401
 
 # ==============================================================================
 
 
 # yyyymmdd
-__releasedate__ = "20230608"
+__releasedate__ = "20230609"
 # x.y.z or x.y.z.dev0 -- semver
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 VERSION = parse_version(__version__)
```

### Comparing `bleach_extras-0.2.0/src/bleach_extras/tag_tree_filter.py` & `bleach_extras-0.2.1/src/bleach_extras/tag_tree_filter.py`

 * *Files identical despite different names*

### Comparing `bleach_extras-0.2.0/src/bleach_extras.egg-info/PKG-INFO` & `bleach_extras-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 Metadata-Version: 2.1
-Name: bleach-extras
-Version: 0.2.0
+Name: bleach_extras
+Version: 0.2.1
 Summary: some extensions for bleach
 Home-page: http://github.com/jvanasco/bleach_extras
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT License
+Description: ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
+        
+        `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
+        use with the `bleach` library.
+        
+        The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
+        and `cleaner_factory__strip_content`.
+        
+        # Compatability
+        
+        `bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`.
+        Earlier versions of `bleach` have security concerns; latter versions are not
+        compatible due to API changes (future support is planned).
+        
+        
+        # `TagTreeFilter`, `clean_strip_content`, `cleaner_factory__strip_content`
+        
+        `clean_strip_content` is paired to `bleach.clean`; the only intended difference
+        is to support the concept of stripping the content tree of tags -- not just the
+        tag node itself.  `cleaner_factory__strip_content` is a factory function used to
+        create configured `bleach.Cleaner` instances.
+        
+        `bleach` has a `strip` flag that toggles the behavior of "unsafe" tags:
+        
+        `strip = False` will render the tags as escaped HTML encodings, such as this
+        replacement:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
+        	
+        `strip = True` will strip the tags, but leave the HTML within as plaintext:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
+        
+        Many users of `bleach` want to remove both the tag and contents of unsafe tags
+        for a variety of reasons, such as:
+        
+        * escaping the tags make the text safe, but unreadable
+        * leaving the tags' content without the tags negatively affects readability and
+          comprehension
+        * leaving the tags' content allows a malicious user to still have some sort of
+          fallback payload which is displayed
+        
+        `clean_strip_content` is a function that mimics `bleach.clean` with a key difference:
+        
+        * tags destined for content stripping are fed into a `Cleaner` instance as allowed
+        * the tags are stripped during the filter process via `TagTreeFilter`
+        
+        An expected transformation is such:
+        
+        	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
+        	+ foo.12.bar
+        
+        Look at that! all the evil payload is gone, including the bitcoin wallet address
+        that f---- spammers tried to slip through.
+        
+        ## Why do this filtering with `bleach` and not something else ?
+        
+        Parsing/Tokenzing HTML is not very efficient. Performing this outside of `bleach`
+        would require performing these operations on the HTML fragments at least twice.
+        
+        `bleach`'s design implementation encodes/strips 'unsafe' tags during the
+        parsing/tokening process - before the plugin filtering process starts. In order
+        to filter the tags out correctly, they must be allowed during the generation of
+        the DOM tree, then removed during the filter step. This trips a lot of people up;
+        offering this in a public library with tests that can grow is ideal.
+        
+        
+        Example:
+        
+        	dangerous = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar"""
+        
+        	print(bleach.clean(dangerous, tags=['div', ], strip=False))
+        	# foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
+        
+        	print(bleach.clean(dangerous, tags=['div', ], strip=True))
+        	# foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
+        
+        	print(bleach_extras.clean_strip_content(dangerous, tags=['div'], ))
+        	# foo.<div>12</div>.bar
+        
+        	cleaner = bleach_extras.cleaner_factory__strip_content(tags=['div'],)
+        	print(cleaner.clean(dangerous))
+        	# foo.<div>12</div>.bar
+        
+        	print(bleach_extras.clean_strip_content(dangerous, tags=['div', ], strip=True, ))
+        	# foo.<div>12</div>.bar
+        
+        ## custom replacement of stripped nodes
+        
+        maybe you need to replace the evil content with a warning. this "extra" has you
+        covered!
+        
+        	dangerous2 = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");<iframe>iiffrraammee</iframe></script>2</div>.bar"""
+        
+        	class IFrameFilter2(bleach_extras.TagTreeFilter):
+        		tags_strip_content = ('script', 'style', 'iframe')
+        		tag_replace_string = "&lt;unsafe garbage/&gt;"
+        
+        	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
+        	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
+        
+        
 Keywords: bleach html-sanitizing
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 Provides-Extra: testing
-License-File: LICENSE
-
-![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
-
-`bleach_extras` is a package of *unofficial* "extras" and utilities paired for
-use with the `bleach` library.
-
-The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
-and `cleaner_factory__strip_content`.
-
-# Compatability
-
-`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`.
-Earlier versions of `bleach` have security concerns; latter versions are not
-compatible due to API changes (future support is planned).
-
-
-# `TagTreeFilter`, `clean_strip_content`, `cleaner_factory__strip_content`
-
-`clean_strip_content` is paired to `bleach.clean`; the only intended difference
-is to support the concept of stripping the content tree of tags -- not just the
-tag node itself.  `cleaner_factory__strip_content` is a factory function used to
-create configured `bleach.Cleaner` instances.
-
-`bleach` has a `strip` flag that toggles the behavior of "unsafe" tags:
-
-`strip = False` will render the tags as escaped HTML encodings, such as this
-replacement:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
-	
-`strip = True` will strip the tags, but leave the HTML within as plaintext:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
-
-Many users of `bleach` want to remove both the tag and contents of unsafe tags
-for a variety of reasons, such as:
-
-* escaping the tags make the text safe, but unreadable
-* leaving the tags' content without the tags negatively affects readability and
-  comprehension
-* leaving the tags' content allows a malicious user to still have some sort of
-  fallback payload which is displayed
-
-`clean_strip_content` is a function that mimics `bleach.clean` with a key difference:
-
-* tags destined for content stripping are fed into a `Cleaner` instance as allowed
-* the tags are stripped during the filter process via `TagTreeFilter`
-
-An expected transformation is such:
-
-	- foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar
-	+ foo.12.bar
-
-Look at that! all the evil payload is gone, including the bitcoin wallet address
-that f---- spammers tried to slip through.
-
-## Why do this filtering with `bleach` and not something else ?
-
-Parsing/Tokenzing HTML is not very efficient. Performing this outside of `bleach`
-would require performing these operations on the HTML fragments at least twice.
-
-`bleach`'s design implementation encodes/strips 'unsafe' tags during the
-parsing/tokening process - before the plugin filtering process starts. In order
-to filter the tags out correctly, they must be allowed during the generation of
-the DOM tree, then removed during the filter step. This trips a lot of people up;
-offering this in a public library with tests that can grow is ideal.
-
-
-Example:
-
-	dangerous = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");</script>2</div>.bar"""
-
-	print(bleach.clean(dangerous, tags=['div', ], strip=False))
-	# foo.<div>1&lt;script&gt;alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");&lt;/script&gt;2</div>.bar
-
-	print(bleach.clean(dangerous, tags=['div', ], strip=True))
-	# foo.<div>1alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");2</div>.bar
-
-	print(bleach_extras.clean_strip_content(dangerous, tags=['div'], ))
-	# foo.<div>12</div>.bar
-
-	cleaner = bleach_extras.cleaner_factory__strip_content(tags=['div'],)
-	print(cleaner.clean(dangerous))
-	# foo.<div>12</div>.bar
-
-	print(bleach_extras.clean_strip_content(dangerous, tags=['div', ], strip=True, ))
-	# foo.<div>12</div>.bar
-
-## custom replacement of stripped nodes
-
-maybe you need to replace the evil content with a warning. this "extra" has you
-covered!
-
-	dangerous2 = """foo.<div>1<script>alert("ur komputer hs VIRUS! Giv me ur BITCOIN in 24 hours! Wallet is: abdefg!");<iframe>iiffrraammee</iframe></script>2</div>.bar"""
-
-	class IFrameFilter2(bleach_extras.TagTreeFilter):
-		tags_strip_content = ('script', 'style', 'iframe')
-		tag_replace_string = "&lt;unsafe garbage/&gt;"
-
-	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
-	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
-
```

#### html2text {}

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1 Name: bleach-extras Version: 0.2.0 Summary: some
+Metadata-Version: 2.1 Name: bleach_extras Version: 0.2.1 Summary: some
 extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
 Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
-License Keywords: bleach html-sanitizing Classifier: License :: OSI Approved ::
-MIT License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown Provides-Extra: testing License-File:
-LICENSE ![Python package](https://github.com/jvanasco/bleach_extras/workflows/
-Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
-"extras" and utilities paired for use with the `bleach` library. The first
-utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
-`cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
-requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
-security concerns; latter versions are not compatible due to API changes
-(future support is planned). # `TagTreeFilter`, `clean_strip_content`,
-`cleaner_factory__strip_content` `clean_strip_content` is paired to
-`bleach.clean`; the only intended difference is to support the concept of
-stripping the content tree of tags -- not just the tagÂ node itself.
+License Description: ![Python package](https://github.com/jvanasco/
+bleach_extras/workflows/Python%20package/badge.svg) `bleach_extras` is a
+package of *unofficial* "extras" and utilities paired for use with the `bleach`
+library. The first utility is `TagTreeFilter` which is utilized by
+`clean_strip_content` and `cleaner_factory__strip_content`. # Compatability
+`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`. Earlier
+versions of `bleach` have security concerns; latter versions are not compatible
+due to API changes (future support is planned). # `TagTreeFilter`,
+`clean_strip_content`, `cleaner_factory__strip_content` `clean_strip_content`
+is paired to `bleach.clean`; the only intended difference is to support the
+concept of stripping the content tree of tags -- not just the tagÂ node itself.
 `cleaner_factory__strip_content` is a factory function used to create
 configured `bleach.Cleaner` instances. `bleach` has a `strip` flag that toggles
 the behavior of "unsafe" tags: `strip = False` will render the tags as escaped
 HTML encodings, such as this replacement: - foo.
 1
 2
 .bar + foo.
@@ -79,8 +71,16 @@
 1
 2
 .bar""" class IFrameFilter2(bleach_extras.TagTreeFilter): tags_strip_content =
 ('script', 'style', 'iframe') tag_replace_string = "<unsafe garbage/>" print
 bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=
 [IFrameFilter2, ]) # foo.
 1&lt;unsafe garbage/&gt;2
-.bar
+.bar Keywords: bleach html-sanitizing Platform: UNKNOWN Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Developers Description-Content-Type: text/markdown Provides-Extra:
+testing
```

### Comparing `bleach_extras-0.2.0/tests/test_clean.py` & `bleach_extras-0.2.1/tests/test_clean.py`

 * *Files identical despite different names*

