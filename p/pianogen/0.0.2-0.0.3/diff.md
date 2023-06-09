# Comparing `tmp/pianogen-0.0.2.tar.gz` & `tmp/pianogen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pianogen-0.0.2.tar", last modified: Wed May 24 12:35:36 2023, max compression
+gzip compressed data, was "pianogen-0.0.3.tar", last modified: Fri Jun  9 13:23:01 2023, max compression
```

## Comparing `pianogen-0.0.2.tar` & `pianogen-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:35:36.329844 pianogen-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-24 11:02:52.000000 pianogen-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2759 2023-05-24 12:35:36.329844 pianogen-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2055 2023-05-24 12:21:29.000000 pianogen-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 12:35:36.303112 pianogen-0.0.2/pianogen/
-drwxrwxrwx   0        0        0        0 2023-05-24 12:35:36.316076 pianogen-0.0.2/pianogen/pianogen/
--rw-rw-rw-   0        0        0      150 2023-05-24 11:15:01.000000 pianogen-0.0.2/pianogen/pianogen/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-05-24 11:15:01.000000 pianogen-0.0.2/pianogen/pianogen/commonTracks.py
--rw-rw-rw-   0        0        0     3133 2023-05-24 11:15:01.000000 pianogen-0.0.2/pianogen/pianogen/parse_to_npy.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:35:36.328844 pianogen-0.0.2/pianogen/pianogen.egg-info/
--rw-rw-rw-   0        0        0     2759 2023-05-24 12:35:36.000000 pianogen-0.0.2/pianogen/pianogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-24 12:35:36.000000 pianogen-0.0.2/pianogen/pianogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:35:36.000000 pianogen-0.0.2/pianogen/pianogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-24 12:35:36.000000 pianogen-0.0.2/pianogen/pianogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 12:35:36.000000 pianogen-0.0.2/pianogen/pianogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 07:26:14.000000 pianogen-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      876 2023-05-24 12:35:36.330845 pianogen-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.355190 pianogen-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-24 11:02:52.000000 pianogen-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2759 2023-06-09 13:23:01.355190 pianogen-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2055 2023-05-24 12:21:29.000000 pianogen-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.323027 pianogen-0.0.3/pianogen/
+drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.343136 pianogen-0.0.3/pianogen/pianogen/
+-rw-rw-rw-   0        0        0      150 2023-05-24 11:15:01.000000 pianogen-0.0.3/pianogen/pianogen/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-09 13:10:11.000000 pianogen-0.0.3/pianogen/pianogen/commonTracks.py
+-rw-rw-rw-   0        0        0     3135 2023-06-09 13:20:37.000000 pianogen-0.0.3/pianogen/pianogen/parse_to_npy.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:23:01.355190 pianogen-0.0.3/pianogen/pianogen.egg-info/
+-rw-rw-rw-   0        0        0     2759 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 13:23:01.000000 pianogen-0.0.3/pianogen/pianogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 07:26:14.000000 pianogen-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      868 2023-06-09 13:23:01.355190 pianogen-0.0.3/setup.cfg
```

### Comparing `pianogen-0.0.2/LICENSE` & `pianogen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pianogen-0.0.2/PKG-INFO` & `pianogen-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianogen
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pianoroll-generator A package to generate pianoroll (NPZ) datasets
 Home-page: https://github.com/cliffordkleinsr/pianoroll-generator
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pianogen-0.0.2/README.md` & `pianogen-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pianogen-0.0.2/pianogen/pianogen/commonTracks.py` & `pianogen-0.0.3/pianogen/pianogen/commonTracks.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,35 +12,45 @@
         self.fldr = fldr # the folder where your midis are saved
         #self.savez = savez
 
     def get_items(
         self,
     ) -> None:
         files = glob.glob(join(self.fldr, '*mid'))
-        return files
+        str_files, clean_files = [], []
+        print("Cleaning Files ...............\ ")
+        for f in files:
+            try:
+                gud_f =Multitrack(f)
+                len(gud_f.tracks)
+                str_files +=[f]
+                clean_files += [gud_f]
+            except (RuntimeWarning, ValueError, IndexError, OSError) as e:
+                continue
+        return str_files, clean_files
         
     def most_common(
         self,
         lst,
     ) -> None:
         return max(set(lst), key=lst.count)
     
     def get_listItems(
         self,
     ) -> None:
         #os.makedirs(self.savez, exist_ok=True)
-        files = self.get_items()
-        tracks = [len(Multitrack(f).tracks) for f in files]
+        str_files, clean_files = self.get_items()
+              
+        tracks = [len(f.tracks) for f in clean_files]
         mc = self.most_common(tracks)
 
         '''loop'''
         common = []
-        for f in files:
-            m = Multitrack(f)
-            if len(m.tracks) == mc:
+        for f, c in zip(str_files, clean_files):
+            if len(c.tracks) == mc:
                 common +=[f]
                 #print('moving:', f, 'with no. of tracks ', len(m.tracks))
                 #shutil.move(f, self.savez)
         with open('common_files.json', 'w') as outfile:
             json.dump(common, outfile)
```

### Comparing `pianogen-0.0.2/pianogen/pianogen/parse_to_npy.py` & `pianogen-0.0.3/pianogen/pianogen/parse_to_npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,19 +70,19 @@
             # Reshape and get the phrase pianorolls
             pianoroll = pianoroll.reshape(-1, 4 * self.BEAT_RESOLUTION, 84, N_TRACKS)
             self.results.append(np.concatenate(
                 [pianoroll[:-3], pianoroll[1:-2], pianoroll[2:-1], pianoroll[3:]], 1))
 
             result = np.concatenate(self.results, 0)
             
-            print('Original shape: ', result.shape)
+            #print('Original shape: ', result.shape)
             
             result = result.reshape(-1, RESHAPE_PARAMS['num_bar'], RESHAPE_PARAMS['num_timestep'],
                         RESHAPE_PARAMS['num_pitch'], RESHAPE_PARAMS['num_track'])
 
-            print('New shape: ', result.shape)
+            #print('New shape: ', result.shape)
             
         # NOTE: You might want to shuffle the training data here
         np.savez_compressed(
             self.resulting_fname, nonzero=np.array(result.nonzero()),
             shape=result.shape
             )
```

### Comparing `pianogen-0.0.2/pianogen/pianogen.egg-info/PKG-INFO` & `pianogen-0.0.3/pianogen/pianogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianogen
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pianoroll-generator A package to generate pianoroll (NPZ) datasets
 Home-page: https://github.com/cliffordkleinsr/pianoroll-generator
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pianogen-0.0.2/setup.cfg` & `pianogen-0.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6961 6e6f 6765 6e0d 0a76 6572   = pianogen..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
 00000030: 7468 6f72 203d 2043 6c69 6666 6f72 6420  thor = Clifford 
 00000040: 4e6a 6f72 6f67 650d 0a61 7574 686f 725f  Njoroge..author_
 00000050: 656d 6169 6c20 3d20 636e 6a6f 726f 6765  email = cnjoroge
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000070: 7269 7074 696f 6e20 3d20 5069 616e 6f72  ription = Pianor
 00000080: 6f6c 6c2d 6765 6e65 7261 746f 7220 4120  oll-generator A 
 00000090: 7061 636b 6167 6520 746f 2067 656e 6572  package to gener
@@ -42,14 +42,14 @@
 00000290: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
 000002a0: 2070 6961 6e6f 6765 6e0d 0a70 6163 6b61   pianogen..packa
 000002b0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
 000002c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 000002d0: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
 000002e0: 6571 7569 7265 7320 3d20 0d0a 0970 7970  equires = ...pyp
 000002f0: 6961 6e6f 726f 6c6c 203d 3d20 302e 352e  ianoroll == 0.5.
-00000300: 330d 0a09 6e75 6d70 793e 3d31 2e32 342e  3...numpy>=1.24.
-00000310: 330d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  3....[options.pa
-00000320: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000330: 6572 6520 3d20 7069 616e 6f67 656e 0d0a  ere = pianogen..
-00000340: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000350: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000360: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000300: 330d 0a09 6e75 6d70 790d 0a0d 0a5b 6f70  3...numpy....[op
+00000310: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000320: 696e 645d 0d0a 7768 6572 6520 3d20 7069  ind]..where = pi
+00000330: 616e 6f67 656e 0d0a 0d0a 5b65 6767 5f69  anogen....[egg_i
+00000340: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000350: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000360: 0d0a 0d0a                                ....
```

