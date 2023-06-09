# Comparing `tmp/easylsb-1.0.7.tar.gz` & `tmp/easylsb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.7.tar", last modified: Tue Jun  6 07:05:58 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.8.tar", last modified: Fri Jun  9 06:49:06 2023, max compression
```

## Comparing `easylsb-1.0.7.tar` & `easylsb-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:05:58.000000 easylsb-1.0.7/
--rw-rw-rw-   0        0        0     1745 2023-06-06 07:05:58.000000 easylsb-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-06-06 07:05:31.000000 easylsb-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 07:05:58.000000 easylsb-1.0.7/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15819 2023-06-06 06:56:54.000000 easylsb-1.0.7/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-06 07:05:58.000000 easylsb-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-06-06 06:57:12.000000 easylsb-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 06:49:06.000000 easylsb-1.0.8/
+-rw-rw-rw-   0        0        0     1745 2023-06-09 06:49:06.000000 easylsb-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-06-06 07:05:31.000000 easylsb-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16093 2023-06-09 06:48:03.000000 easylsb-1.0.8/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 06:49:06.000000 easylsb-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-06-09 06:48:53.000000 easylsb-1.0.8/setup.py
```

### Comparing `easylsb-1.0.7/PKG-INFO` & `easylsb-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
```

### Comparing `easylsb-1.0.7/README.md` & `easylsb-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `easylsb-1.0.7/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.8/easylsb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
```

### Comparing `easylsb-1.0.7/lsb.py` & `easylsb-1.0.8/lsb.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,18 @@
                 with open(args.rsa + '.pem', 'rb') as f:
                     privkey = _rsa.PrivateKey.load_pkcs1(f.read())
             else:
                 privkey = None
             img = _i.open(args.image)
             dec = lsbdec(_a(img), mode=mode, key=args.key.encode(args.encoding),rsakey=privkey)
             if args.auto:
-                encoding=detect(dec)
+                encoding=detect(dec)['encoding']
+                if encoding is None:
+                    print('It seems that the encoding is unknown')
+                    return -1
             else:
                 encoding=args.encoding
             print(dec.decode(encoding))
     else:
         print("unkown operation: ", args.operation)
         return -1
 
@@ -421,14 +424,17 @@
                 privkey=_rsa.PrivateKey.load_pkcs1(f.read())
         else:
             privkey=None
         wav = wave.open(args.audio)
         dec = lsbdec_audio(wav, mode, key=args.key.encode(args.encoding),rsakey=privkey)
         if args.auto:
             encoding=detect(dec)['encoding']
+            if encoding is None:
+                print('It seems that the encoding is unknown')
+                return -1
         else:
             encoding=args.encoding
         print(dec.decode(encoding))
     else:
         print("Unknown operation: ", args.operation)
         return -1
```

### Comparing `easylsb-1.0.7/setup.py` & `easylsb-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     req.append('pillow')
 def readme():
     with open('README.md','r') as file:
         return file.read()
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 setup(
     name="easylsb",
-    version="1.0.7",
+    version="1.0.8",
     description="Simple Python package for steganography",
     long_description=readme(),
     long_description_content_type='text/markdown',
     py_modules=["lsb"],
     install_requires=req,
     entry_points={
         "console_scripts": [
```

