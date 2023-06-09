# Comparing `tmp/FoxitPDFConversionSDKPython3-1.2.0-cp39-cp39-win_amd64.whl.zip` & `tmp/FoxitPDFConversionSDKPython3-1.3.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9585477 bytes, number of entries: 8
+Zip file size: 10070429 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      187 b- defN 22-Dec-30 03:55 FoxitPDFConversionSDKPython3/__init__.py
--rw-rw-rw-  2.0 fat 22322176 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3/_fpdfconversionsdk.pyd
--rw-rw-rw-  2.0 fat    22935 b- defN 23-Apr-06 09:47 FoxitPDFConversionSDKPython3/fpdfconversionsdk.py
--rw-rw-rw-  2.0 fat     2872 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat    21548 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3-1.2.0.dist-info/legal.txt
--rw-rw-rw-  2.0 fat       48 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      810 b- defN 23-Apr-06 09:53 FoxitPDFConversionSDKPython3-1.2.0.dist-info/RECORD
-8 files, 22370676 bytes uncompressed, 9584035 bytes compressed:  57.2%
+-rw-rw-rw-  2.0 fat 23531520 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3/_fpdfconversionsdk.pyd
+-rw-rw-rw-  2.0 fat    23314 b- defN 23-Jun-06 08:20 FoxitPDFConversionSDKPython3/fpdfconversionsdk.py
+-rw-rw-rw-  2.0 fat     4318 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat    21548 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3-1.3.0.dist-info/legal.txt
+-rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-06 08:26 FoxitPDFConversionSDKPython3-1.3.0.dist-info/RECORD
+8 files, 23581845 bytes uncompressed, 10068987 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: FoxitPDFConversionSDKPython3/_fpdfconversionsdk.pyd
 Comment: 
 
 Filename: FoxitPDFConversionSDKPython3/fpdfconversionsdk.py
 Comment: 
 
-Filename: FoxitPDFConversionSDKPython3-1.2.0.dist-info/METADATA
+Filename: FoxitPDFConversionSDKPython3-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: FoxitPDFConversionSDKPython3-1.2.0.dist-info/WHEEL
+Filename: FoxitPDFConversionSDKPython3-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: FoxitPDFConversionSDKPython3-1.2.0.dist-info/legal.txt
+Filename: FoxitPDFConversionSDKPython3-1.3.0.dist-info/legal.txt
 Comment: 
 
-Filename: FoxitPDFConversionSDKPython3-1.2.0.dist-info/top_level.txt
+Filename: FoxitPDFConversionSDKPython3-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: FoxitPDFConversionSDKPython3-1.2.0.dist-info/RECORD
+Filename: FoxitPDFConversionSDKPython3-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## FoxitPDFConversionSDKPython3/fpdfconversionsdk.py

```diff
@@ -400,14 +400,18 @@
         Release = staticmethod(_fpdfconversionsdk.Library_Release)
     else:
         Release = _fpdfconversionsdk.Library_Release
     if _newclass:
         GetVersion = staticmethod(_fpdfconversionsdk.Library_GetVersion)
     else:
         GetVersion = _fpdfconversionsdk.Library_GetVersion
+    if _newclass:
+        EnableThreadSafety = staticmethod(_fpdfconversionsdk.Library_EnableThreadSafety)
+    else:
+        EnableThreadSafety = _fpdfconversionsdk.Library_EnableThreadSafety
     __swig_destroy__ = _fpdfconversionsdk.delete_Library
     __del__ = lambda self: None
 Library_swigregister = _fpdfconversionsdk.Library_swigregister
 Library_swigregister(Library)
 
 def Library_Initialize(*args):
     return _fpdfconversionsdk.Library_Initialize(*args)
@@ -421,14 +425,18 @@
     return _fpdfconversionsdk.Library_Release(*args)
 Library_Release = _fpdfconversionsdk.Library_Release
 
 def Library_GetVersion(*args):
     return _fpdfconversionsdk.Library_GetVersion(*args)
 Library_GetVersion = _fpdfconversionsdk.Library_GetVersion
 
+def Library_EnableThreadSafety(*args):
+    return _fpdfconversionsdk.Library_EnableThreadSafety(*args)
+Library_EnableThreadSafety = _fpdfconversionsdk.Library_EnableThreadSafety
+
 class Progressive(Base):
     __swig_setmethods__ = {}
     for _s in [Base]:
         __swig_setmethods__.update(getattr(_s, '__swig_setmethods__', {}))
     __setattr__ = lambda self, name, value: _swig_setattr(self, Progressive, name, value)
     __swig_getmethods__ = {}
     for _s in [Base]:
```

## Comparing `FoxitPDFConversionSDKPython3-1.2.0.dist-info/legal.txt` & `FoxitPDFConversionSDKPython3-1.3.0.dist-info/legal.txt`

 * *Files identical despite different names*

## Comparing `FoxitPDFConversionSDKPython3-1.2.0.dist-info/RECORD` & `FoxitPDFConversionSDKPython3-1.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 FoxitPDFConversionSDKPython3/__init__.py,sha256=J8oxTN8mH1BsE3hpwxZiAos0oWIdrAD-0qBpCai6hTs,187
-FoxitPDFConversionSDKPython3/_fpdfconversionsdk.pyd,sha256=TFsb7dGPBV-h614Vz1USFNkqXffBa73_HQ9R17_91fY,22322176
-FoxitPDFConversionSDKPython3/fpdfconversionsdk.py,sha256=a27e_Mu8HD3FnQiLf9E-ZNMYrp40EfnVfQ0m0JRiBf0,22935
-FoxitPDFConversionSDKPython3-1.2.0.dist-info/METADATA,sha256=47Dn1k1hYMEWUidVGJErg-dXi_7khdRB2p9PEGHbh64,2872
-FoxitPDFConversionSDKPython3-1.2.0.dist-info/WHEEL,sha256=fVcVlLzi8CGi_Ul8vjMdn8gER25dn5GBg9E6k9z41-Y,100
-FoxitPDFConversionSDKPython3-1.2.0.dist-info/legal.txt,sha256=TxWCImLKj7FYcdeehPU5HivhzFTq_oYYEU1ZpVgzxuM,21548
-FoxitPDFConversionSDKPython3-1.2.0.dist-info/top_level.txt,sha256=S5ikbqXY_G-zFQOy80sbls20ss0Gqky04t0QJq5qPgo,48
-FoxitPDFConversionSDKPython3-1.2.0.dist-info/RECORD,,
+FoxitPDFConversionSDKPython3/_fpdfconversionsdk.pyd,sha256=V1ge1dAFCF51x4dMn-MCup-oEZ1VAoNGFgPHPKCy2qA,23531520
+FoxitPDFConversionSDKPython3/fpdfconversionsdk.py,sha256=CakVObsXLQAQXeKZvNhCB0k_AKFI0NX2y9NdBhQWISQ,23314
+FoxitPDFConversionSDKPython3-1.3.0.dist-info/METADATA,sha256=D4DR8dUIGeDvyVuDFE3oP9-IFxxVpvDal5Z2x1oV1fg,4318
+FoxitPDFConversionSDKPython3-1.3.0.dist-info/WHEEL,sha256=fVcVlLzi8CGi_Ul8vjMdn8gER25dn5GBg9E6k9z41-Y,100
+FoxitPDFConversionSDKPython3-1.3.0.dist-info/legal.txt,sha256=TxWCImLKj7FYcdeehPU5HivhzFTq_oYYEU1ZpVgzxuM,21548
+FoxitPDFConversionSDKPython3-1.3.0.dist-info/top_level.txt,sha256=S5ikbqXY_G-zFQOy80sbls20ss0Gqky04t0QJq5qPgo,48
+FoxitPDFConversionSDKPython3-1.3.0.dist-info/RECORD,,
```

