# Comparing `tmp/AoiPy-0.9.17-py3-none-any.whl.zip` & `tmp/AoiPy-0.9.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,20 @@
-Zip file size: 4444 bytes, number of entries: 12
+Zip file size: 6638 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat       62 b- defN 23-May-28 17:44 Aoipy/__init__.py
--rw-rw-rw-  2.0 fat     2023 b- defN 23-May-28 17:23 Aoipy/tools.py
+-rw-rw-rw-  2.0 fat     2037 b- defN 23-May-28 19:28 Aoipy/tools.py
 -rw-rw-rw-  2.0 fat     3891 b- defN 23-May-28 17:51 Aoipy/Function/AoiCore.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:14 Aoipy/Function/__init__.py
 -rw-rw-rw-  2.0 fat       83 b- defN 23-May-28 07:25 Aoipy/Function/Guilds/Channels.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:15 Aoipy/Function/Guilds/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:17 Aoipy/Function/Users/__init__.py
 -rw-rw-rw-  2.0 fat      781 b- defN 23-May-28 17:23 Aoipy/Function/Users/funcs.py
--rw-rw-rw-  2.0 fat      396 b- defN 23-May-28 19:18 AoiPy-0.9.17.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 19:18 AoiPy-0.9.17.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-28 19:18 AoiPy-0.9.17.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      943 b- defN 23-May-28 19:18 AoiPy-0.9.17.dist-info/RECORD
-12 files, 8277 bytes uncompressed, 2844 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     3891 b- defN 23-May-28 17:51 Aoipy/Functions/AoiCore.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:14 Aoipy/Functions/__init__.py
+-rw-rw-rw-  2.0 fat       83 b- defN 23-May-28 07:25 Aoipy/Functions/Guilds/Channels.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:15 Aoipy/Functions/Guilds/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 19:17 Aoipy/Functions/Users/__init__.py
+-rw-rw-rw-  2.0 fat      781 b- defN 23-May-28 17:23 Aoipy/Functions/Users/funcs.py
+-rw-rw-rw-  2.0 fat      396 b- defN 23-May-28 19:32 AoiPy-0.9.18.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 19:32 AoiPy-0.9.18.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-28 19:32 AoiPy-0.9.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1457 b- defN 23-May-28 19:32 AoiPy-0.9.18.dist-info/RECORD
+18 files, 13560 bytes uncompressed, 4214 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -18,20 +18,38 @@
 
 Filename: Aoipy/Function/Users/__init__.py
 Comment: 
 
 Filename: Aoipy/Function/Users/funcs.py
 Comment: 
 
-Filename: AoiPy-0.9.17.dist-info/METADATA
+Filename: Aoipy/Functions/AoiCore.py
 Comment: 
 
-Filename: AoiPy-0.9.17.dist-info/WHEEL
+Filename: Aoipy/Functions/__init__.py
 Comment: 
 
-Filename: AoiPy-0.9.17.dist-info/top_level.txt
+Filename: Aoipy/Functions/Guilds/Channels.py
 Comment: 
 
-Filename: AoiPy-0.9.17.dist-info/RECORD
+Filename: Aoipy/Functions/Guilds/__init__.py
+Comment: 
+
+Filename: Aoipy/Functions/Users/__init__.py
+Comment: 
+
+Filename: Aoipy/Functions/Users/funcs.py
+Comment: 
+
+Filename: AoiPy-0.9.18.dist-info/METADATA
+Comment: 
+
+Filename: AoiPy-0.9.18.dist-info/WHEEL
+Comment: 
+
+Filename: AoiPy-0.9.18.dist-info/top_level.txt
+Comment: 
+
+Filename: AoiPy-0.9.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Aoipy/tools.py

```diff
@@ -52,9 +52,9 @@
             else:
                 argument = await findBracketPairs(argument)
             find = [first, last, keyword, argument]
         if find[2].lower() in funcs:
             name = await funcs[find[2].lower()](find[3])
     try:
         return name
-    except ReferenceError:
-        return "Error"
+    except:
+        raise SyntaxError(f"Missing '$' in {code}")
```

## Comparing `AoiPy-0.9.17.dist-info/RECORD` & `AoiPy-0.9.18.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 Aoipy/__init__.py,sha256=nMiUPuIkNRiQgcDSVrk4cmg1lRy2e1CLf15OzqNMFUc,62
-Aoipy/tools.py,sha256=VyE2QlN6HWT7l2JO-lNcqhGKUtY2mL9HN08N9VArgG8,2023
+Aoipy/tools.py,sha256=6syyO2RSjD8UoT9ZA5hE0VCXCDCEg9H3JvPqw73Xp0E,2037
 Aoipy/Function/AoiCore.py,sha256=h0A8ep9SAy4NArIl0gxhJksRC-QWMMzXxONWXrxK1bI,3891
 Aoipy/Function/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Aoipy/Function/Guilds/Channels.py,sha256=ZEkBK5_XcMoH3TN-BohAnAEGP-1pMOFDOKjaMGd44EQ,83
 Aoipy/Function/Guilds/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Aoipy/Function/Users/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Aoipy/Function/Users/funcs.py,sha256=SQk2U2DQqNapXSB11nzqhJfEuhgiwOZTEFl7iQxDzqw,781
-AoiPy-0.9.17.dist-info/METADATA,sha256=qU1z9khBIe6YgVPCBZhL5schOzgllDlTbJYPaF12PJA,396
-AoiPy-0.9.17.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-AoiPy-0.9.17.dist-info/top_level.txt,sha256=SA7Pn09kz2QD1ED-0qO8ZZBUgKZHmUnWp3UbzaDh6-A,6
-AoiPy-0.9.17.dist-info/RECORD,,
+Aoipy/Functions/AoiCore.py,sha256=h0A8ep9SAy4NArIl0gxhJksRC-QWMMzXxONWXrxK1bI,3891
+Aoipy/Functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+Aoipy/Functions/Guilds/Channels.py,sha256=ZEkBK5_XcMoH3TN-BohAnAEGP-1pMOFDOKjaMGd44EQ,83
+Aoipy/Functions/Guilds/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+Aoipy/Functions/Users/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+Aoipy/Functions/Users/funcs.py,sha256=SQk2U2DQqNapXSB11nzqhJfEuhgiwOZTEFl7iQxDzqw,781
+AoiPy-0.9.18.dist-info/METADATA,sha256=U7-EyEuUJMEAc2svtWWMxJCWT2sbNVXTYFKH3gnpEZs,396
+AoiPy-0.9.18.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+AoiPy-0.9.18.dist-info/top_level.txt,sha256=SA7Pn09kz2QD1ED-0qO8ZZBUgKZHmUnWp3UbzaDh6-A,6
+AoiPy-0.9.18.dist-info/RECORD,,
```

