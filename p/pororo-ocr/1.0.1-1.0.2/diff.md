# Comparing `tmp/pororo_ocr-1.0.1-py3-none-any.whl.zip` & `tmp/pororo_ocr-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 62336 bytes, number of entries: 37
+Zip file size: 59907 bytes, number of entries: 37
 -rw-r--r--  2.0 unx      111 b- defN 23-Jun-08 13:23 prrocr/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-08 13:25 prrocr/__version__.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-09 13:52 prrocr/__version__.py
 -rw-r--r--  2.0 unx     2900 b- defN 23-Jun-08 09:24 prrocr/pororo.py
--rw-r--r--  2.0 unx     6952 b- defN 23-Jun-08 13:08 prrocr/prrocr.py
+-rw-r--r--  2.0 unx     6694 b- defN 23-Jun-09 10:31 prrocr/prrocr.py
 -rw-r--r--  2.0 unx      238 b- defN 23-Jun-08 10:07 prrocr/test.py
 -rw-r--r--  2.0 unx     2222 b- defN 23-May-31 02:46 prrocr/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 02:46 prrocr/models/__init__.py
 -rw-r--r--  2.0 unx       37 b- defN 23-May-31 02:46 prrocr/models/brainOCR/__init__.py
 -rw-r--r--  2.0 unx     1022 b- defN 23-May-31 02:46 prrocr/models/brainOCR/_dataset.py
 -rw-r--r--  2.0 unx    20996 b- defN 23-May-31 02:46 prrocr/models/brainOCR/_modules.py
 -rw-r--r--  2.0 unx     8365 b- defN 23-Jun-08 08:49 prrocr/models/brainOCR/brainocr.py
@@ -25,15 +25,15 @@
 -rw-r--r--  2.0 unx     8768 b- defN 23-May-31 02:46 prrocr/models/brainOCR/modules/transformation.py
 -rw-r--r--  2.0 unx      388 b- defN 23-Jun-08 09:24 prrocr/tasks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 02:46 prrocr/tasks/utils/__init__.py
 -rw-r--r--  2.0 unx     5011 b- defN 23-May-31 02:46 prrocr/tasks/utils/base.py
 -rw-r--r--  2.0 unx     3386 b- defN 23-May-31 02:46 prrocr/tasks/utils/config.py
 -rw-r--r--  2.0 unx     8101 b- defN 23-Jun-08 09:24 prrocr/tasks/utils/download_utils.py
 -rw-r--r--  2.0 unx     2804 b- defN 23-May-31 02:46 prrocr/tasks/utils/tokenizer.py
--rw-r--r--  2.0 unx    11360 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    26965 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_library
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_model
--rw-r--r--  2.0 unx     8749 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3263 b- defN 23-Jun-08 13:25 pororo_ocr-1.0.1.dist-info/RECORD
-37 files, 198220 bytes uncompressed, 57052 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx    11360 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26965 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_library
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_model
+-rw-r--r--  2.0 unx     2828 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3263 b- defN 23-Jun-09 13:52 pororo_ocr-1.0.2.dist-info/RECORD
+37 files, 192041 bytes uncompressed, 54623 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -84,29 +84,29 @@
 
 Filename: prrocr/tasks/utils/download_utils.py
 Comment: 
 
 Filename: prrocr/tasks/utils/tokenizer.py
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/LICENSE
+Filename: pororo_ocr-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_library
+Filename: pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_library
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_model
+Filename: pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_model
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/METADATA
+Filename: pororo_ocr-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/WHEEL
+Filename: pororo_ocr-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/top_level.txt
+Filename: pororo_ocr-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pororo_ocr-1.0.1.dist-info/RECORD
+Filename: pororo_ocr-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prrocr/__version__.py

```diff
@@ -1 +1 @@
-version = "1.0.1"
+version = "1.0.2"
```

## prrocr/prrocr.py

```diff
@@ -217,13 +217,7 @@
                 image_path,
                 skip_details=False,
                 batch_size=1,
                 paragraph=True,
             ),
             detail,
         )
-
-if __name__ == "__main__":
-    ocr = PororoOCR(lang="ko")
-    result = ocr(
-        "https://lh3.googleusercontent.com/proxy/u0cVmJsmGQ9QF5pTuHaf1cnA2_XUmy4YL6lzzF_9177TBe2qXwjGugdly42dec5oI46Ks8sAFEtDU8bSTI4o4y7kWcQkXvLUGwpN00Ym7Eiendcj")
-    print(result)
```

## Comparing `pororo_ocr-1.0.1.dist-info/LICENSE` & `pororo_ocr-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_library` & `pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_library`

 * *Files identical despite different names*

## Comparing `pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_model` & `pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_model`

 * *Files identical despite different names*

## Comparing `pororo_ocr-1.0.1.dist-info/RECORD` & `pororo_ocr-1.0.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 prrocr/__init__.py,sha256=dqsUwavjOW-ggrFIp7A1hL16gOWX_28Hi2lzXZjnQts,111
-prrocr/__version__.py,sha256=_ZEXZ9OcLtIJ-gPvOkMv1OKAzml7W1MzZe1jHAUZeBE,18
+prrocr/__version__.py,sha256=tTF5v0pCQ3wj3WtOg6KXgEGkOMgBeRFQACKUYV29zxo,18
 prrocr/pororo.py,sha256=sKBnwVS_D4UaphAHZPtcfCtzGyjgCCyUMzhFgO4FUno,2900
-prrocr/prrocr.py,sha256=DzoMpO2vqIuvNuHuM86eBbZ7rNPDx7O0mYbhzIyuf80,6952
+prrocr/prrocr.py,sha256=pHfJQIxnBl2Bh-eZXfyMgYWf6t_X9C57VUu2dp4Y9_I,6694
 prrocr/test.py,sha256=yggeDcdLMFgs37QxrlUt-mugp2Do53_M_FtGk-lEqB8,238
 prrocr/utils.py,sha256=jsF8Un5cUDUoN1rt4vxnSi8hUPlriW2OAfo9pRrkFGs,2222
 prrocr/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 prrocr/models/brainOCR/__init__.py,sha256=NJjH7zI5cSQU-u4yAIi-J3gC2DIpo-Yvn6EtDD_Zyfo,37
 prrocr/models/brainOCR/_dataset.py,sha256=2_GyQpc1rgbsPI3H06_QHW4x6NgZElVRaNmwKISMaa0,1022
 prrocr/models/brainOCR/_modules.py,sha256=i2ls_LZmS9BVxttpIBKtJuavddfa1AiVqv91Hf2F_1w,20996
 prrocr/models/brainOCR/brainocr.py,sha256=o7Ukk86fCWqm7BQesjw91AczC6IjmiCiGuOVxEhfvro,8365
@@ -24,14 +24,14 @@
 prrocr/models/brainOCR/modules/transformation.py,sha256=XT3JJH4Xedmkd6jx2daWn00ofNxSTKqk5CDa7xV5Z-s,8768
 prrocr/tasks/__init__.py,sha256=36HpriUdBsUSqv2U7m9AekbGLmnIupqbKEuTdUilB8I,388
 prrocr/tasks/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 prrocr/tasks/utils/base.py,sha256=Kb3tF01RBGfpIbebzyc2LAoesBNW6o2Tr0Wc3U0LA38,5011
 prrocr/tasks/utils/config.py,sha256=VL4jz_Oz6XWsNXZ10OcrM-niBvcnI1CyWKQWCQynlI4,3386
 prrocr/tasks/utils/download_utils.py,sha256=vSFUpIwgvf5_-urStMwIkMzzA3btaDaIKE_dIkoMUpA,8101
 prrocr/tasks/utils/tokenizer.py,sha256=XR-_VH3A2YEJ_IoXoWLSE8C5Cebl8u3yfHwQOWLq4U8,2804
-pororo_ocr-1.0.1.dist-info/LICENSE,sha256=MUQMax-oXcGRIfQm7KUyMvagMVACVmtSCThi_KM5uJM,11360
-pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_library,sha256=vzTLs7Ez8WDngBP5YaPgj-43EUU_3oZ0-QnscuiUj-A,26965
-pororo_ocr-1.0.1.dist-info/LICENSE.3rd_party_model,sha256=xs2P3XJWWcOV3uShs6-b1otvxxqX4d17yIQQEuEa5_4,966
-pororo_ocr-1.0.1.dist-info/METADATA,sha256=zkLxV_0JLx0spCoBtV1rbf8vwAmnf4rkc0DFY_AliCw,8749
-pororo_ocr-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pororo_ocr-1.0.1.dist-info/top_level.txt,sha256=fzB2InJjGHzJwA9-GTgkNWslDAsnZv9DLYj2YvotPbA,7
-pororo_ocr-1.0.1.dist-info/RECORD,,
+pororo_ocr-1.0.2.dist-info/LICENSE,sha256=MUQMax-oXcGRIfQm7KUyMvagMVACVmtSCThi_KM5uJM,11360
+pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_library,sha256=vzTLs7Ez8WDngBP5YaPgj-43EUU_3oZ0-QnscuiUj-A,26965
+pororo_ocr-1.0.2.dist-info/LICENSE.3rd_party_model,sha256=xs2P3XJWWcOV3uShs6-b1otvxxqX4d17yIQQEuEa5_4,966
+pororo_ocr-1.0.2.dist-info/METADATA,sha256=FKLveKkTOmRB2FGT44RFiE3xquPo0A7b2WP6EV6qxdo,2828
+pororo_ocr-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pororo_ocr-1.0.2.dist-info/top_level.txt,sha256=fzB2InJjGHzJwA9-GTgkNWslDAsnZv9DLYj2YvotPbA,7
+pororo_ocr-1.0.2.dist-info/RECORD,,
```

