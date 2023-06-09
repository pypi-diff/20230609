# Comparing `tmp/libpymcr-0.1.1-cp39-cp39-win_amd64.whl.zip` & `tmp/libpymcr-0.1.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 192759 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     5007 b- defN 23-Mar-24 10:19 libpymcr/Matlab.py
--rw-rw-rw-  2.0 fat     9690 b- defN 23-Mar-24 10:19 libpymcr/MatlabProxyObject.py
--rw-rw-rw-  2.0 fat      175 b- defN 23-Mar-24 10:19 libpymcr/__init__.py
--rw-rw-rw-  2.0 fat   447488 b- defN 23-Mar-24 10:28 libpymcr/_libpymcr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      518 b- defN 23-Mar-24 10:28 libpymcr/_version.py
--rw-rw-rw-  2.0 fat     8322 b- defN 23-Mar-24 10:19 libpymcr/utils.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Mar-24 10:29 libpymcr-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Mar-24 10:29 libpymcr-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-24 10:29 libpymcr-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-24 10:29 libpymcr-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      875 b- defN 23-Mar-24 10:29 libpymcr-0.1.1.dist-info/RECORD
-11 files, 510593 bytes uncompressed, 191291 bytes compressed:  62.5%
+Zip file size: 194113 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     5010 b- defN 23-Jun-09 01:03 libpymcr/Matlab.py
+-rw-rw-rw-  2.0 fat     9690 b- defN 23-Jun-09 01:03 libpymcr/MatlabProxyObject.py
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Jun-09 01:03 libpymcr/__init__.py
+-rw-rw-rw-  2.0 fat   450048 b- defN 23-Jun-09 01:11 libpymcr/_libpymcr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-09 01:11 libpymcr/_version.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 23-Jun-09 01:03 libpymcr/utils.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      875 b- defN 23-Jun-09 01:12 libpymcr-0.1.2.dist-info/RECORD
+11 files, 513216 bytes uncompressed, 192645 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: libpymcr/_version.py
 Comment: 
 
 Filename: libpymcr/utils.py
 Comment: 
 
-Filename: libpymcr-0.1.1.dist-info/LICENSE
+Filename: libpymcr-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: libpymcr-0.1.1.dist-info/METADATA
+Filename: libpymcr-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: libpymcr-0.1.1.dist-info/WHEEL
+Filename: libpymcr-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: libpymcr-0.1.1.dist-info/top_level.txt
+Filename: libpymcr-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: libpymcr-0.1.1.dist-info/RECORD
+Filename: libpymcr-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libpymcr/Matlab.py

```diff
@@ -38,15 +38,15 @@
 
 class NamespaceWrapper(object):
     def __init__(self, interface, name):
         self._interface = interface
         self._name = name
 
     def __getattr__(self, name):
-        return NamespaceWrapper(self._matlab, f'{self._name}.{name}')
+        return NamespaceWrapper(self._interface, f'{self._name}.{name}')
 
     def __call__(self, *args, **kwargs):
         nargout = kwargs.pop('nargout') if 'nargout' in kwargs.keys() else None
         nreturn = get_nlhs()
         if nargout is None:
             mnargout, undetermined = self._interface.call('getArgOut', self._name, nargout=2)
             if not undetermined:
```

## libpymcr/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-03-24T03:09:25+0000",
+ "date": "2023-06-09T01:51:35+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "12e90de8e5ccd2f87cc53672e79ec72651f9d862",
- "version": "0.1.1"
+ "full-revisionid": "9b713dbc40b12ecbe097335aa1b319c17d186046",
+ "version": "0.1.2"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## libpymcr/utils.py

```diff
@@ -6,15 +6,15 @@
 import traceback
 from pathlib import Path
 
 
 def get_nlhs():
     caller = traceback.extract_stack()[-3].line
     retvals = (0, '')
-    if '=' in caller:
+    if '=' in caller and '(' in caller and caller.index('=') < caller.index('('):
         return len(caller.split('=')[0].split(','))
     else:
         return 1
 
 
 def get_version_from_ctf(ctffile):
     with zipfile.ZipFile(ctffile, 'r') as ctf:
```

## Comparing `libpymcr-0.1.1.dist-info/LICENSE` & `libpymcr-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libpymcr-0.1.1.dist-info/METADATA` & `libpymcr-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpymcr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module to allow Python to call functions from a compiled Matlab archive
 Home-page: https://github.com/pace-neutrons/libpymcr
 Author: Duc Le
 Author-email: duc.le@stfc.ac.uk
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

## Comparing `libpymcr-0.1.1.dist-info/RECORD` & `libpymcr-0.1.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-libpymcr/Matlab.py,sha256=GFvKIRDzffgN6mqNJWyLX7auuCYTR98R5qI0ndKwJ8o,5007
+libpymcr/Matlab.py,sha256=l2cesZ372H3Zo_przYnwgzQF3AHCK6Meg6mxQPcth2Y,5010
 libpymcr/MatlabProxyObject.py,sha256=5A93jipCzHhPwOAly8E0wXkzKMQE3PbapWmylv4S5X8,9690
 libpymcr/__init__.py,sha256=sQKTM1zicjP6fj_l3S3MBGEnqp_H0TYtm0iIlejgs-I,175
-libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=jnUAKjag08n_u0chaMaw9cOJvVBY6ldDc2IZrl67F0k,447488
-libpymcr/_version.py,sha256=Yp_YLe_zfXHjz76bXSQUz9dC480_Auvkft3Q0i5Cec0,518
-libpymcr/utils.py,sha256=IFTcuBaNjnYY0wuCGuOe19lm8okgfHRCa8DdcE2H9cY,8322
-libpymcr-0.1.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-libpymcr-0.1.1.dist-info/METADATA,sha256=3KJZQKDwwL3Y6QaPk6diMD4ljTdWe9cYZwfCQK0bDDw,2586
-libpymcr-0.1.1.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-libpymcr-0.1.1.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
-libpymcr-0.1.1.dist-info/RECORD,,
+libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=xG6IH7mDmw5NP_Hl_y93DEcAYXWpO-v6211JV5jKGFo,450048
+libpymcr/_version.py,sha256=bmRryh7vRc3D2wU1ddY30NFCkfEmVzhQAmpO0G20ycg,518
+libpymcr/utils.py,sha256=ZQIZfG0uSFKJBpwE4w8Jveh3C0873z4ak2XTh1S-Z9k,8382
+libpymcr-0.1.2.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+libpymcr-0.1.2.dist-info/METADATA,sha256=xZRNSmNEziSOlbpy31o0ASWcxtTeyItEjdH1hgymqiQ,2586
+libpymcr-0.1.2.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
+libpymcr-0.1.2.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
+libpymcr-0.1.2.dist-info/RECORD,,
```

