# Comparing `tmp/pyspk-1.3.tar.gz` & `tmp/pyspk-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.3.tar", last modified: Thu May 18 08:48:02 2023, max compression
+gzip compressed data, was "pyspk-1.4.tar", last modified: Fri Jun  9 16:28:32 2023, max compression
```

## Comparing `pyspk-1.3.tar` & `pyspk-1.4.tar`

### file list

```diff
@@ -1,27 +1,19 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.905345 pyspk-1.3/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2022-09-13 12:12:10.000000 pyspk-1.3/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2022-09-14 12:27:24.000000 pyspk-1.3/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9087 2023-05-18 08:48:02.905172 pyspk-1.3/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8566 2023-05-18 08:41:38.000000 pyspk-1.3/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.902318 pyspk-1.3/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     6148 2022-09-24 18:18:43.000000 pyspk-1.3/pyspk/.DS_Store
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2022-09-13 12:12:10.000000 pyspk-1.3/pyspk/__init__.py
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.904863 pyspk-1.3/pyspk/__pycache__/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-04-26 10:36:22.000000 pyspk-1.3/pyspk/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2022-09-25 14:31:25.000000 pyspk-1.3/pyspk/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-04-26 10:37:02.000000 pyspk-1.3/pyspk/__pycache__/fit_vals.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     2083 2022-09-25 14:31:25.000000 pyspk-1.3/pyspk/__pycache__/fit_vals.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    18870 2023-05-02 10:10:08.000000 pyspk-1.3/pyspk/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    14636 2022-11-04 10:54:05.000000 pyspk-1.3/pyspk/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-03-24 10:17:38.000000 pyspk-1.3/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-05-12 14:14:32.000000 pyspk-1.3/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180313 2022-09-24 07:34:27.000000 pyspk-1.3/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179350 2022-09-24 07:36:40.000000 pyspk-1.3/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-05-18 08:48:02.903538 pyspk-1.3/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9087 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      550 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-05-18 08:48:02.000000 pyspk-1.3/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-05-18 08:48:02.905382 pyspk-1.3/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-05-18 08:45:27.000000 pyspk-1.3/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.856931 pyspk-1.4/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.4/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.4/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 16:28:32.856725 pyspk-1.4/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.4/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.855882 pyspk-1.4/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/__init__.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.4/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 16:28:32.856549 pyspk-1.4/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      288 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-09 16:28:32.000000 pyspk-1.4/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-09 16:28:32.856965 pyspk-1.4/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-09 16:28:12.000000 pyspk-1.4/setup.py
```

### Comparing `pyspk-1.3/LICENSE.md` & `pyspk-1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.3/PKG-INFO` & `pyspk-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.3
+Version: 1.4
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
                           _____ ____   ____   _ 
         ____  __  __     / ___// __ \_/_/ /__| |
        / __ \/ / / /_____\__ \/ /_/ / // //_// /
       / /_/ / /_/ /_____/__/ / ____/ // ,<  / / 
      / .___/\__, /     /____/_/   / //_/|_|/_/  
     /_/    /____/                 |_|    /_/    
 
-py-SP(k) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
+py-SP(k) [(Salcido et al. 2023)](https://academic.oup.com/mnras/article/523/2/2247/7165765) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
 
 ## Requirements
 
 The module requires the following:
 
 - numpy
 - scipy
@@ -129,21 +129,23 @@
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
 @ARTICLE{SPK_Salcido_2023,
     author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
-    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    title = "{SP(k) – a hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
     journal = {Monthly Notices of the Royal Astronomical Society},
+    volume = {523},
+    number = {2},
+    pages = {2247-2262},
     year = {2023},
     month = {05},
     issn = {0035-8711},
     doi = {10.1093/mnras/stad1474},
     url = {https://doi.org/10.1093/mnras/stad1474},
-    note = {stad1474},
-    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
+    eprint = {https://academic.oup.com/mnras/article-pdf/523/2/2247/50512773/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.3/README.md` & `pyspk-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
                           _____ ____   ____   _ 
         ____  __  __     / ___// __ \_/_/ /__| |
        / __ \/ / / /_____\__ \/ /_/ / // //_// /
       / /_/ / /_/ /_____/__/ / ____/ // ,<  / / 
      / .___/\__, /     /____/_/   / //_/|_|/_/  
     /_/    /____/                 |_|    /_/    
 
-py-SP(k) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
+py-SP(k) [(Salcido et al. 2023)](https://academic.oup.com/mnras/article/523/2/2247/7165765) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
 
 ## Requirements
 
 The module requires the following:
 
 - numpy
 - scipy
@@ -116,21 +116,23 @@
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
 @ARTICLE{SPK_Salcido_2023,
     author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
-    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    title = "{SP(k) – a hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
     journal = {Monthly Notices of the Royal Astronomical Society},
+    volume = {523},
+    number = {2},
+    pages = {2247-2262},
     year = {2023},
     month = {05},
     issn = {0035-8711},
     doi = {10.1093/mnras/stad1474},
     url = {https://doi.org/10.1093/mnras/stad1474},
-    note = {stad1474},
-    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
+    eprint = {https://academic.oup.com/mnras/article-pdf/523/2/2247/50512773/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.3/pyspk/__pycache__/model.cpython-38.pyc` & `pyspk-1.4/pyspk/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1180 +1,1018 @@
-00000000: 550d 0d0a 0000 0000 6ce1 5064 5e58 0000  U.......l.Pd^X..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000f 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c02 6d05 5a06 0100 6404  ..d.d.l.m.Z...d.
-00000050: 6405 6c07 6d08 5a09 0100 6404 6406 6c07  d.l.m.Z...d.d.l.
-00000060: 6d0a 5a0b 0100 6400 6401 6c0c 5a0d 6400  m.Z...d.d.l.Z.d.
-00000070: 6401 6c0e 5a0f 650d 6a10 6407 6511 6408  d.l.Z.e.j.d.e.d.
-00000080: 8d02 0100 6427 6409 640a 8401 5a12 640b  ....d'd.d...Z.d.
-00000090: 640c 8400 5a13 640d 640e 8400 5a14 640f  d...Z.d.d...Z.d.
-000000a0: 6410 8400 5a15 6411 6412 8400 5a16 6413  d...Z.d.d...Z.d.
-000000b0: 6414 8400 5a17 6415 6416 8400 5a18 6417  d...Z.d.d...Z.d.
-000000c0: 6418 8400 5a19 6419 641a 8400 5a1a 641b  d...Z.d.d...Z.d.
-000000d0: 641c 8400 5a1b 641d 641e 8400 5a1c 6428  d...Z.d.d...Z.d(
-000000e0: 6423 6424 8401 5a1d 6429 6425 6426 8401  d#d$..Z.d)d%d&..
-000000f0: 5a1e 6401 5300 292a e900 0000 004e 2901  Z.d.S.)*.....N).
-00000100: da13 416b 696d 6131 4449 6e74 6572 706f  ..Akima1DInterpo
-00000110: 6c61 746f 7229 01da 144c 696e 6561 724e  lator)...LinearN
-00000120: 4449 6e74 6572 706f 6c61 746f 72e9 0100  DInterpolator...
-00000130: 0000 2901 da0d 6265 7374 5f66 6974 5f76  ..)...best_fit_v
-00000140: 616c 7329 01da 066c 696d 6974 73da 0661  als)...limits..a
-00000150: 6c77 6179 7329 01da 0863 6174 6567 6f72  lways)...categor
-00000160: 7963 0400 0000 0000 0000 0000 0000 0500  yc..............
-00000170: 0000 0500 0000 4300 0000 7318 0000 007c  ......C...s....|
-00000180: 0174 00a0 017c 007c 031b 007c 02a1 0214  .t...|.|...|....
-00000190: 007d 047c 0453 0029 0161 db01 0000 0a20  .}.|.S.).a..... 
-000001a0: 2020 2053 696d 706c 6520 706f 7765 722d     Simple power-
-000001b0: 6c61 7720 6675 6e63 7469 6f6e 2066 6974  law function fit
-000001c0: 2074 6f20 7468 6520 6261 7279 6f6e 2066   to the baryon f
-000001d0: 7261 6374 696f 6e20 2d20 6861 6c6f 206d  raction - halo m
-000001e0: 6173 7320 7265 6c61 7469 6f6e 0a0a 2020  ass relation..  
-000001f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000200: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000210: 6d5f 6861 6c6f 3a20 6172 7261 7920 6f66  m_halo: array of
-00000220: 2066 6c6f 6174 0a20 2020 2020 2020 2068   float.        h
-00000230: 616c 6f20 6d61 7373 2069 6e20 4d5f 7375  alo mass in M_su
-00000240: 6e20 756e 6974 730a 2020 2020 6662 5f61  n units.    fb_a
-00000250: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
-00000260: 2070 6f77 6572 206c 6177 2063 6f6e 7374   power law const
-00000270: 616e 740a 2020 2020 6662 5f70 6f77 203a  ant.    fb_pow :
-00000280: 2066 6c6f 6174 0a20 2020 2020 2020 2070   float.        p
-00000290: 6f77 6572 206c 6177 2065 7870 6f6e 656e  ower law exponen
-000002a0: 740a 2020 2020 6662 5f70 6976 6f74 203a  t.    fb_pivot :
-000002b0: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-000002c0: 310a 2020 2020 2020 2020 706f 7765 7220  1.        power 
-000002d0: 6c61 7720 7069 766f 7420 706f 696e 742e  law pivot point.
-000002e0: 200a 0a20 2020 2052 6574 7572 6e73 0a20   ..    Returns. 
-000002f0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 206f     -------.    o
-00000300: 7574 7075 743a 2061 7272 6179 206f 6620  utput: array of 
-00000310: 666c 6f61 740a 2020 2020 2020 2020 6261  float.        ba
-00000320: 7279 6f6e 2066 7261 6374 696f 6e20 6e6f  ryon fraction no
-00000330: 726d 616c 6973 6564 2062 7920 7468 6520  rmalised by the 
-00000340: 556e 6976 6572 7361 6c20 6261 7279 6f6e  Universal baryon
-00000350: 2066 7261 6374 696f 6e3a 2066 5f62 202f   fraction: f_b /
-00000360: 2028 4f6d 6567 615f 6220 2f20 4f6d 6567   (Omega_b / Omeg
-00000370: 615f 6d29 0a20 2020 20a9 02da 035f 6e70  a_m).    ...._np
-00000380: da05 706f 7765 7229 05da 066d 5f68 616c  ..power)...m_hal
-00000390: 6fda 0466 625f 61da 0666 625f 706f 77da  o..fb_a..fb_pow.
-000003a0: 0866 625f 7069 766f 74da 0266 62a9 0072  .fb_pivot..fb..r
-000003b0: 1100 0000 fa28 2f55 7365 7273 2f6a 6169  .....(/Users/jai
-000003c0: 6d65 7361 6c63 6964 6f2f 7079 7370 6b2f  mesalcido/pyspk/
-000003d0: 7079 7370 6b2f 6d6f 6465 6c2e 7079 da0a  pyspk/model.py..
-000003e0: 5f70 6f77 6572 5f6c 6177 0c00 0000 7304  _power_law....s.
-000003f0: 0000 0000 1414 0172 1300 0000 6302 0000  .......r....c...
-00000400: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00000410: 0043 0000 0073 2c00 0000 7c01 6401 1900  .C...s,...|.d...
-00000420: 7400 a001 7c00 6401 a102 1400 7c01 6402  t...|.d.....|.d.
-00000430: 1900 7c00 1400 1700 7c01 6403 1900 1700  ..|.....|.d.....
-00000440: 7d02 7c02 5300 2904 6116 0100 000a 2020  }.|.S.).a.....  
-00000450: 2020 5369 6d70 6c65 2070 6f6c 796e 6f6d    Simple polynom
-00000460: 6961 6c20 6f66 206f 7264 6572 2032 2e20  ial of order 2. 
-00000470: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000480: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00000490: 2020 2020 7820 3a20 6172 7261 7920 6f66      x : array of
-000004a0: 2066 6c6f 6174 0a20 2020 2020 2020 2069   float.        i
-000004b0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-000004c0: 626c 6520 0a20 2020 2076 616c 7320 3a20  ble .    vals : 
-000004d0: 6172 7261 7920 6f66 2066 6c6f 6174 0a20  array of float. 
-000004e0: 2020 2020 2020 2061 7272 6179 2063 6f6e         array con
-000004f0: 7461 696e 696e 6720 7468 6520 706f 6c79  taining the poly
-00000500: 6e6f 6d69 616c 2063 6f65 6666 6963 6965  nomial coefficie
-00000510: 6e74 730a 0a20 2020 2052 6574 7572 6e73  nts..    Returns
-00000520: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00000530: 2079 3a20 6172 7261 7920 6f66 2066 6c6f   y: array of flo
-00000540: 6174 0a20 2020 2020 2020 2064 6570 656e  at.        depen
-00000550: 6465 6e74 2076 6172 6961 626c 6520 0a20  dent variable . 
-00000560: 2020 20e9 0200 0000 7204 0000 0072 0100     .....r....r..
-00000570: 0000 7209 0000 0029 03da 0178 da04 7661  ..r....)...x..va
-00000580: 6c73 da01 7972 1100 0000 7211 0000 0072  ls..yr....r....r
-00000590: 1200 0000 da07 5f70 6f6c 795f 3224 0000  ......_poly_2$..
-000005a0: 0073 0400 0000 0010 2801 7218 0000 0063  .s......(.r....c
-000005b0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000005c0: 0700 0000 4300 0000 732c 0000 007c 0164  ....C...s,...|.d
-000005d0: 0119 007c 0164 0119 007c 0164 0219 0018  ...|.d...|.d....
-000005e0: 0074 00a0 017c 007c 0164 0319 00a1 0214  .t...|.|.d......
-000005f0: 0018 007d 027c 0253 0029 0461 8c01 0000  ...}.|.S.).a....
-00000600: 0a20 2020 204f 7074 696d 616c 206d 6173  .    Optimal mas
-00000610: 7320 6675 6e63 7469 6f6e 2064 6566 696e  s function defin
-00000620: 6564 2069 6e20 6571 2e28 3229 2069 6e20  ed in eq.(2) in 
-00000630: 5361 6c63 6964 6f20 6574 2061 6c2e 2028  Salcido et al. (
-00000640: 3230 3232 292e 0a0a 2020 2020 5061 7261  2022)...    Para
-00000650: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00000660: 2d2d 2d2d 2d0a 2020 2020 6b20 3a20 6172  -----.    k : ar
-00000670: 7261 7920 6f66 2066 6c6f 6174 0a20 2020  ray of float.   
-00000680: 2020 2020 2063 6f2d 6d6f 7669 6e67 2077       co-moving w
-00000690: 6176 656e 756d 6265 7220 696e 2075 6e69  avenumber in uni
-000006a0: 7473 205b 682f 4d70 635d 0a20 2020 2070  ts [h/Mpc].    p
-000006b0: 7261 6d73 203a 2064 6963 740a 2020 2020  rams : dict.    
-000006c0: 2020 2020 6469 6374 696f 6e61 7279 2063      dictionary c
-000006d0: 6f6e 7461 696e 696e 6720 7468 6520 6265  ontaining the be
-000006e0: 7374 2066 6974 7469 6e67 2070 6172 616d  st fitting param
-000006f0: 6574 6572 7320 6f66 2074 6865 2053 5028  eters of the SP(
-00000700: 6b29 206d 6f64 656c 2061 7420 6120 7370  k) model at a sp
-00000710: 6563 6966 6963 2072 6564 7368 6966 742e  ecific redshift.
-00000720: 200a 0a20 2020 2052 6574 7572 6e73 0a20   ..    Returns. 
-00000730: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 206f     -------.    o
-00000740: 7574 7075 743a 2061 7272 6179 206f 6620  utput: array of 
-00000750: 666c 6f61 740a 2020 2020 2020 2020 6c6f  float.        lo
-00000760: 675f 3130 206f 6620 7468 6520 6f70 7469  g_10 of the opti
-00000770: 6d61 6c20 6d61 7373 2069 6e20 4d5f 7375  mal mass in M_su
-00000780: 6e20 756e 6974 730a 2020 2020 da05 616c  n units.    ..al
-00000790: 7068 61da 0462 6574 61da 0567 616d 6d61  pha..beta..gamma
-000007a0: 7209 0000 0029 03da 016b da06 7061 7261  r....)...k..para
-000007b0: 6d73 da06 6f75 7470 7574 7211 0000 0072  ms..outputr....r
-000007c0: 1100 0000 7212 0000 00da 135f 6f70 7469  ....r......_opti
-000007d0: 6d61 6c5f 6d61 7373 5f66 756e 6374 3800  mal_mass_funct8.
-000007e0: 0000 7304 0000 0000 1028 0172 1f00 0000  ..s......(.r....
-000007f0: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
-00000800: 0007 0000 0043 0000 0073 6e00 0000 7400  .....C...sn...t.
-00000810: a001 7c02 a101 7d03 7c03 6401 6b04 721a  ..|...}.|.d.k.r.
-00000820: 7402 6402 8301 8201 7c03 6403 6b04 7230  t.d.....|.d.k.r0
-00000830: 7403 6a04 6404 6405 6406 8d02 0100 7405  t.j.d.d.d.....t.
-00000840: 7c00 7c01 8302 7d04 7c04 6407 1900 7c04  |.|...}.|.d...|.
-00000850: 6407 1900 7c04 6408 1900 1800 7400 a006  d...|.d.....t...
-00000860: 7c02 7c04 6409 1900 a102 1400 1800 7d05  |.|.d.........}.
-00000870: 7400 a006 640a 7c05 a102 5300 290b 61dc  t...d.|...S.).a.
-00000880: 0100 000a 2020 2020 4f70 7469 6d61 6c20  ....    Optimal 
-00000890: 6d61 7373 2066 756e 6374 696f 6e20 6173  mass function as
-000008a0: 2061 2066 756e 6374 696f 6e20 6f66 2073   a function of s
-000008b0: 6361 6c65 2061 6e64 2072 6564 7368 6966  cale and redshif
-000008c0: 7420 666f 7220 6120 7370 6563 6966 6963  t for a specific
-000008d0: 200a 2020 2020 7370 6865 7269 6361 6c20   .    spherical 
-000008e0: 6f76 6572 2d64 656e 7369 7479 2e20 4465  over-density. De
-000008f0: 6669 6e65 6420 696e 2065 712e 2832 2920  fined in eq.(2) 
-00000900: 696e 2053 616c 6369 646f 2065 7420 616c  in Salcido et al
-00000910: 2e20 2832 3032 3229 2e0a 0a20 2020 2050  . (2022)...    P
-00000920: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00000930: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2053 4f20  --------.    SO 
-00000940: 3a20 696e 740a 2020 2020 2020 2020 7370  : int.        sp
-00000950: 6865 7269 6361 6c20 6f76 6572 2d64 656e  herical over-den
-00000960: 7369 7479 2e20 4f6e 6c79 2061 6363 6570  sity. Only accep
-00000970: 7473 2032 3030 206f 7220 3530 300a 2020  ts 200 or 500.  
-00000980: 2020 7a20 3a20 666c 6f61 740a 2020 2020    z : float.    
-00000990: 2020 2020 7265 6473 6869 6674 207a 2e20      redshift z. 
-000009a0: 4f6e 6c79 2061 6363 6570 7473 2076 616c  Only accepts val
-000009b0: 7565 7320 6f66 207a 203c 3d20 330a 2020  ues of z <= 3.  
-000009c0: 2020 6b20 3a20 6172 7261 7920 6f66 2066    k : array of f
-000009d0: 6c6f 6174 0a20 2020 2020 2020 2063 6f2d  loat.        co-
-000009e0: 6d6f 7669 6e67 2077 6176 656e 756d 6265  moving wavenumbe
-000009f0: 7220 696e 2075 6e69 7473 205b 682f 4d70  r in units [h/Mp
-00000a00: 635d 0a0a 2020 2020 5265 7475 726e 730a  c]..    Returns.
-00000a10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00000a20: 6f75 7470 7574 3a20 6172 7261 7920 6f66  output: array of
-00000a30: 2066 6c6f 6174 0a20 2020 2020 2020 206f   float.        o
-00000a40: 7074 696d 616c 206d 6173 7320 696e 204d  ptimal mass in M
-00000a50: 5f73 756e 2075 6e69 7473 0a20 2020 20e9  _sun units.    .
-00000a60: 0c00 0000 7a61 1b5b 3931 6d70 792d 7370  ....za.[91mpy-sp
-00000a70: 6b20 7761 7320 6361 6c69 6272 6174 6564  k was calibrated
-00000a80: 2075 7020 746f 206b 5f6d 6178 203d 2031   up to k_max = 1
-00000a90: 3220 5b68 2f4d 7063 5d20 506c 6561 7365  2 [h/Mpc] Please
-00000aa0: 2073 7065 6369 6679 2076 616c 7565 7320   specify values 
-00000ab0: 6f66 206b 203c 3d20 3132 205b 682f 4d70  of k <= 12 [h/Mp
-00000ac0: 635d 201b 5b30 6de9 0800 0000 fa5d 1b5b  c] .[0m......].[
-00000ad0: 3333 6d53 6361 6c65 7320 7769 7468 206b  33mScales with k
-00000ae0: 5f6d 6178 203e 206b 5f6e 7920 3d20 3820  _max > k_ny = 8 
-00000af0: 5b68 2f4d 7063 5d20 6d61 7920 6e6f 7420  [h/Mpc] may not 
-00000b00: 6265 2061 6363 7572 6174 656c 7920 7265  be accurately re
-00000b10: 7072 6f64 7563 6564 2062 7920 7468 6520  produced by the 
-00000b20: 6d6f 6465 6c2e 201b 5b30 6d72 1400 0000  model. .[0mr....
-00000b30: a901 da0a 7374 6163 6b6c 6576 656c 7219  ....stacklevelr.
-00000b40: 0000 0072 1a00 0000 721b 0000 00e9 0a00  ...r....r.......
-00000b50: 0000 2907 720a 0000 00da 036d 6178 da09  ..).r......max..
-00000b60: 4578 6365 7074 696f 6eda 095f 7761 726e  Exception.._warn
-00000b70: 696e 6773 da04 7761 726e da0b 5f67 6574  ings..warn.._get
-00000b80: 5f70 6172 616d 7372 0b00 0000 2906 da02  _paramsr....)...
-00000b90: 534f da01 7a72 1c00 0000 da05 6b5f 6d61  SO..zr......k_ma
-00000ba0: 7872 1d00 0000 721e 0000 0072 1100 0000  xr....r....r....
-00000bb0: 7211 0000 0072 1200 0000 da0c 6f70 7469  r....r......opti
-00000bc0: 6d61 6c5f 6d61 7373 4c00 0000 7314 0000  mal_massL...s...
-00000bd0: 0000 130a 0108 0108 0208 0106 0102 ff06  ................
-00000be0: 030a 0128 0172 2e00 0000 6302 0000 0000  ...(.r....c.....
-00000bf0: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
-00000c00: 0000 0073 2200 0000 6401 7c01 6402 1900  ...s"...d.|.d...
-00000c10: 7400 a001 7c01 6403 1900 7c00 1400 a101  t...|.d...|.....
-00000c20: 1400 1700 7d02 7c02 5300 2904 617c 0100  ....}.|.S.).a|..
-00000c30: 000a 2020 2020 6c61 6d62 6461 2066 756e  ..    lambda fun
-00000c40: 6374 696f 6e20 666f 7220 6120 7370 6563  ction for a spec
-00000c50: 6966 6963 2072 6564 7368 6966 742e 2044  ific redshift. D
-00000c60: 6566 696e 6564 2069 6e20 6571 2e28 3629  efined in eq.(6)
-00000c70: 2069 6e20 5361 6c63 6964 6f20 6574 2061   in Salcido et a
-00000c80: 6c2e 2028 3230 3232 292e 0a0a 2020 2020  l. (2022)...    
-00000c90: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000ca0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6b20  ---------.    k 
-00000cb0: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
-00000cc0: 0a20 2020 2020 2020 2063 6f2d 6d6f 7669  .        co-movi
-00000cd0: 6e67 2077 6176 656e 756d 6265 7220 696e  ng wavenumber in
-00000ce0: 2075 6e69 7473 205b 682f 4d70 635d 0a20   units [h/Mpc]. 
-00000cf0: 2020 2070 7261 6d73 203a 2064 6963 740a     prams : dict.
-00000d00: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
-00000d10: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
-00000d20: 6520 6265 7374 2066 6974 7469 6e67 2070  e best fitting p
-00000d30: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
-00000d40: 2053 5028 6b29 206d 6f64 656c 2061 7420   SP(k) model at 
-00000d50: 6120 7370 6563 6966 6963 2072 6564 7368  a specific redsh
-00000d60: 6966 742e 200a 0a20 2020 2052 6574 7572  ift. ..    Retur
-00000d70: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00000d80: 2020 206f 7574 7075 743a 2061 7272 6179     output: array
-00000d90: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
-00000da0: 2020 6c61 6d62 6461 0a20 2020 2072 0400    lambda.    r..
-00000db0: 0000 5a08 6c61 6d62 6461 5f61 5a08 6c61  ..Z.lambda_aZ.la
-00000dc0: 6d62 6461 5f62 a902 720a 0000 00da 0365  mbda_b..r......e
-00000dd0: 7870 2903 7215 0000 0072 1d00 0000 721e  xp).r....r....r.
-00000de0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00000df0: 0000 da0d 5f6c 616d 6264 615f 6675 6e63  ...._lambda_func
-00000e00: 746c 0000 0073 0400 0000 0010 1e01 7231  tl...s........r1
-00000e10: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000e20: 0600 0000 0600 0000 4300 0000 7342 0000  ........C...sB..
-00000e30: 007c 0164 0119 007d 0264 027c 0164 0119  .|.d...}.d.|.d..
-00000e40: 0018 007d 0364 0274 00a0 017c 0164 0319  ...}.d.t...|.d..
-00000e50: 007c 0014 007c 0164 0419 0017 00a1 0117  .|...|.d........
-00000e60: 007d 047c 027c 037c 041b 0017 007d 057c  .}.|.|.|.....}.|
-00000e70: 0553 0029 0561 7401 0000 0a20 2020 206d  .S.).at....    m
-00000e80: 7520 6675 6e63 7469 6f6e 2066 6f72 2061  u function for a
-00000e90: 2073 7065 6369 6669 6320 7265 6473 6869   specific redshi
-00000ea0: 6674 2e20 4465 6669 6e65 6420 696e 2065  ft. Defined in e
-00000eb0: 712e 2837 2920 696e 2053 616c 6369 646f  q.(7) in Salcido
-00000ec0: 2065 7420 616c 2e20 2832 3032 3229 2e0a   et al. (2022)..
-00000ed0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00000ee0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00000ef0: 2020 206b 203a 2061 7272 6179 206f 6620     k : array of 
-00000f00: 666c 6f61 740a 2020 2020 2020 2020 636f  float.        co
-00000f10: 2d6d 6f76 696e 6720 7761 7665 6e75 6d62  -moving wavenumb
-00000f20: 6572 2069 6e20 756e 6974 7320 5b68 2f4d  er in units [h/M
-00000f30: 7063 5d0a 2020 2020 7072 616d 7320 3a20  pc].    prams : 
-00000f40: 6469 6374 0a20 2020 2020 2020 2064 6963  dict.        dic
-00000f50: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-00000f60: 6e67 2074 6865 2062 6573 7420 6669 7474  ng the best fitt
-00000f70: 696e 6720 7061 7261 6d65 7465 7273 206f  ing parameters o
-00000f80: 6620 7468 6520 5350 286b 2920 6d6f 6465  f the SP(k) mode
-00000f90: 6c20 6174 2061 2073 7065 6369 6669 6320  l at a specific 
-00000fa0: 7265 6473 6869 6674 2e20 0a0a 2020 2020  redshift. ..    
-00000fb0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00000fc0: 2d2d 2d0a 2020 2020 6f75 7470 7574 3a20  ---.    output: 
-00000fd0: 6172 7261 7920 6f66 2066 6c6f 6174 0a20  array of float. 
-00000fe0: 2020 2020 2020 206d 750a 2020 2020 5a04         mu.    Z.
-00000ff0: 6d75 5f61 7204 0000 005a 046d 755f 625a  mu_ar....Z.mu_bZ
-00001000: 046d 755f 6372 2f00 0000 2906 7215 0000  .mu_cr/...).r...
-00001010: 0072 1d00 0000 da01 41da 0142 da01 4372  .r......A..B..Cr
-00001020: 1e00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00001030: 0000 00da 095f 6d75 5f66 756e 6374 8000  ....._mu_funct..
-00001040: 0000 730a 0000 0000 1008 010c 011e 010c  ..s.............
-00001050: 0172 3500 0000 6302 0000 0000 0000 0000  .r5...c.........
-00001060: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-00001070: 3600 0000 7c01 6401 1900 7d02 7400 a001  6...|.d...}.t...
-00001080: 6402 7c00 7c01 6403 1900 1800 7c01 6404  d.|.|.d.....|.d.
-00001090: 1900 1b00 6405 1300 1400 a101 7d03 7c02  ....d.......}.|.
-000010a0: 7c03 1400 7d04 7c04 5300 2906 6174 0100  |...}.|.S.).at..
-000010b0: 000a 2020 2020 6e75 2066 756e 6374 696f  ..    nu functio
-000010c0: 6e20 666f 7220 6120 7370 6563 6966 6963  n for a specific
-000010d0: 2072 6564 7368 6966 742e 2044 6566 696e   redshift. Defin
-000010e0: 6564 2069 6e20 6571 2e28 3829 2069 6e20  ed in eq.(8) in 
-000010f0: 5361 6c63 6964 6f20 6574 2061 6c2e 2028  Salcido et al. (
-00001100: 3230 3232 292e 0a0a 2020 2020 5061 7261  2022)...    Para
-00001110: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00001120: 2d2d 2d2d 2d0a 2020 2020 6b20 3a20 6172  -----.    k : ar
-00001130: 7261 7920 6f66 2066 6c6f 6174 0a20 2020  ray of float.   
-00001140: 2020 2020 2063 6f2d 6d6f 7669 6e67 2077       co-moving w
-00001150: 6176 656e 756d 6265 7220 696e 2075 6e69  avenumber in uni
-00001160: 7473 205b 682f 4d70 635d 0a20 2020 2070  ts [h/Mpc].    p
-00001170: 7261 6d73 203a 2064 6963 740a 2020 2020  rams : dict.    
-00001180: 2020 2020 6469 6374 696f 6e61 7279 2063      dictionary c
-00001190: 6f6e 7461 696e 696e 6720 7468 6520 6265  ontaining the be
-000011a0: 7374 2066 6974 7469 6e67 2070 6172 616d  st fitting param
-000011b0: 6574 6572 7320 6f66 2074 6865 2053 5028  eters of the SP(
-000011c0: 6b29 206d 6f64 656c 2061 7420 6120 7370  k) model at a sp
-000011d0: 6563 6966 6963 2072 6564 7368 6966 742e  ecific redshift.
-000011e0: 200a 0a20 2020 2052 6574 7572 6e73 0a20   ..    Returns. 
-000011f0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 206f     -------.    o
-00001200: 7574 7075 743a 2061 7272 6179 206f 6620  utput: array of 
-00001210: 666c 6f61 740a 2020 2020 2020 2020 6e75  float.        nu
-00001220: 0a20 2020 205a 046e 755f 6167 0000 0000  .    Z.nu_ag....
-00001230: 0000 e0bf 5a04 6e75 5f62 5a04 6e75 5f63  ....Z.nu_bZ.nu_c
-00001240: 7214 0000 0072 2f00 0000 2905 7215 0000  r....r/...).r...
-00001250: 0072 1d00 0000 7232 0000 0072 3300 0000  .r....r2...r3...
-00001260: 721e 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00001270: 1200 0000 da08 5f6e 755f 6675 6e63 9700  ......_nu_func..
-00001280: 0000 7308 0000 0000 1008 0122 0108 0172  ..s........"...r
-00001290: 3600 0000 6303 0000 0000 0000 0000 0000  6...c...........
-000012a0: 000b 0000 0006 0000 0043 0000 0073 3c01  .........C...s<.
-000012b0: 0000 7400 7401 7402 7c00 8301 1900 6401  ..t.t.t.|.....d.
-000012c0: 1900 7401 7402 7c00 8301 1900 6402 1900  ..t.t.|.....d...
-000012d0: 8302 7d03 7400 7401 7402 7c00 8301 1900  ..}.t.t.t.|.....
-000012e0: 6401 1900 7401 7402 7c00 8301 1900 6403  d...t.t.|.....d.
-000012f0: 1900 8302 7d04 7400 7401 7402 7c00 8301  ....}.t.t.t.|...
-00001300: 1900 6401 1900 7401 7402 7c00 8301 1900  ..d...t.t.|.....
-00001310: 6404 1900 8302 7d05 7400 7401 7402 7c00  d.....}.t.t.t.|.
-00001320: 8301 1900 6401 1900 7401 7402 7c00 8301  ....d...t.t.|...
-00001330: 1900 6405 1900 8302 7d06 7400 7401 7402  ..d.....}.t.t.t.
-00001340: 7c00 8301 1900 6401 1900 7401 7402 7c00  |.....d...t.t.|.
-00001350: 8301 1900 6406 1900 8302 7d07 7400 7401  ....d.....}.t.t.
-00001360: 7402 7c00 8301 1900 6401 1900 7401 7402  t.|.....d...t.t.
-00001370: 7c00 8301 1900 6407 1900 8302 7d08 6408  |.....d.....}.d.
-00001380: 7c03 7c01 8301 7c04 7c01 8301 7403 a004  |.|...|.|...t...
-00001390: 7c02 a101 1400 1700 7c05 7c01 8301 7403  |.......|.|...t.
-000013a0: a004 7c02 a101 6409 1300 1400 1700 1300  ..|...d.........
-000013b0: 7d09 6408 7c06 7c01 8301 7c07 7c01 8301  }.d.|.|...|.|...
-000013c0: 7403 a004 7c02 a101 1400 1700 7c08 7c01  t...|.......|.|.
-000013d0: 8301 7403 a004 7c02 a101 6409 1300 1400  ..t...|...d.....
-000013e0: 1700 1300 7d0a 7c09 7c0a 6602 5300 290a  ....}.|.|.f.S.).
-000013f0: 615e 0200 000a 2020 2020 4675 6e63 7469  a^....    Functi
-00001400: 6f6e 2074 6861 7420 7265 7475 726e 7320  on that returns 
-00001410: 7468 6520 6261 7279 6f6e 2066 7261 6374  the baryon fract
-00001420: 696f 6e20 6669 7474 696e 6720 6c69 6d69  ion fitting limi
-00001430: 7473 2061 7320 6120 6675 6e63 7469 6f6e  ts as a function
-00001440: 206f 6620 6861 6c6f 206d 6173 730a 2020   of halo mass.  
-00001450: 2020 616e 6420 7265 6473 6869 6674 2e0a    and redshift..
-00001460: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00001470: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00001480: 2020 2053 4f20 3a20 696e 740a 2020 2020     SO : int.    
-00001490: 2020 2020 7370 6865 7269 6361 6c20 6f76      spherical ov
-000014a0: 6572 2d64 656e 7369 7479 2e20 4f6e 6c79  er-density. Only
-000014b0: 2061 6363 6570 7473 2032 3030 206f 7220   accepts 200 or 
-000014c0: 3530 300a 2020 2020 7a20 3a20 666c 6f61  500.    z : floa
-000014d0: 740a 2020 2020 2020 2020 7265 6473 6869  t.        redshi
-000014e0: 6674 207a 2e20 4f6e 6c79 2061 6363 6570  ft z. Only accep
-000014f0: 7473 2076 616c 7565 7320 6f66 207a 203c  ts values of z <
-00001500: 3d20 330a 2020 2020 6d5f 6861 6c6f 3a20  = 3.    m_halo: 
-00001510: 6172 7261 7920 6f66 2066 6c6f 6174 0a20  array of float. 
-00001520: 2020 2020 2020 2068 616c 6f20 6d61 7373         halo mass
-00001530: 2069 6e20 4d5f 7375 6e20 756e 6974 730a   in M_sun units.
-00001540: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00001550: 202d 2d2d 2d2d 2d2d 0a20 2020 206d 696e   -------.    min
-00001560: 5f66 623a 2061 7272 6179 206f 6620 666c  _fb: array of fl
-00001570: 6f61 740a 2020 2020 2020 2020 6c6f 7765  oat.        lowe
-00001580: 7220 6669 7474 696e 6720 6c69 6d69 7420  r fitting limit 
-00001590: 666f 7220 7468 6520 6261 7279 6f6e 2066  for the baryon f
-000015a0: 7261 6374 696f 6e20 6e6f 726d 616c 6973  raction normalis
-000015b0: 6564 2062 7920 7468 6520 756e 6976 6572  ed by the univer
-000015c0: 7361 6c20 6261 7279 6f6e 2066 7261 6374  sal baryon fract
-000015d0: 696f 6e0a 2020 2020 6d61 785f 6662 3a20  ion.    max_fb: 
-000015e0: 6172 7261 7920 6f66 2066 6c6f 6174 0a20  array of float. 
-000015f0: 2020 2020 2020 2075 7070 6572 2066 6974         upper fit
-00001600: 7469 6e67 206c 696d 6974 2066 6f72 2074  ting limit for t
-00001610: 6865 2062 6172 796f 6e20 6672 6163 7469  he baryon fracti
-00001620: 6f6e 206e 6f72 6d61 6c69 7365 6420 6279  on normalised by
-00001630: 2074 6865 2075 6e69 7665 7273 616c 2062   the universal b
-00001640: 6172 796f 6e20 6672 6163 7469 6f6e 0a20  aryon fraction. 
-00001650: 2020 2072 2c00 0000 5a06 6d69 6e5f 7830     r,...Z.min_x0
-00001660: 5a06 6d69 6e5f 7831 5a06 6d69 6e5f 7832  Z.min_x1Z.min_x2
-00001670: 5a06 6d61 785f 7830 5a06 6d61 785f 7831  Z.max_x0Z.max_x1
-00001680: 5a06 6d61 785f 7832 7225 0000 0072 1400  Z.max_x2r%...r..
-00001690: 0000 2905 da14 5f41 6b69 6d61 3144 496e  ..)..._Akima1DIn
-000016a0: 7465 7270 6f6c 6174 6f72 da07 5f6c 696d  terpolator.._lim
-000016b0: 6974 73da 0373 7472 720a 0000 00da 056c  its..strr......l
-000016c0: 6f67 3130 290b 722b 0000 0072 2c00 0000  og10).r+...r,...
-000016d0: 720c 0000 005a 0c69 6e74 6572 5f6d 696e  r....Z.inter_min
-000016e0: 5f78 305a 0c69 6e74 6572 5f6d 696e 5f78  _x0Z.inter_min_x
-000016f0: 315a 0c69 6e74 6572 5f6d 696e 5f78 325a  1Z.inter_min_x2Z
-00001700: 0c69 6e74 6572 5f6d 6178 5f78 305a 0c69  .inter_max_x0Z.i
-00001710: 6e74 6572 5f6d 6178 5f78 315a 0c69 6e74  nter_max_x1Z.int
-00001720: 6572 5f6d 6178 5f78 32da 066d 696e 5f66  er_max_x2..min_f
-00001730: 62da 066d 6178 5f66 6272 1100 0000 7211  b..max_fbr....r.
-00001740: 0000 0072 1200 0000 da0a 6765 745f 6c69  ...r......get_li
-00001750: 6d69 7473 ad00 0000 7312 0000 0000 1622  mits....s......"
-00001760: 0122 0122 0222 0122 0122 0234 0134 0272  .".".".".".4.4.r
-00001770: 3d00 0000 6302 0000 0000 0000 0000 0000  =...c...........
-00001780: 0004 0000 0006 0000 0043 0000 0073 5200  .........C...sR.
-00001790: 0000 6900 7d02 7a34 7400 7401 7c00 8301  ..i.}.z4t.t.|...
-000017a0: 1900 4400 5d22 7d03 7402 6401 7c01 1700  ..D.]"}.t.d.|...
-000017b0: 7400 7401 7c00 8301 1900 7c03 1900 8302  t.t.|.....|.....
-000017c0: 7c02 7c03 3c00 7112 5700 6e14 0100 0100  |.|.<.q.W.n.....
-000017d0: 0100 7403 6402 8301 8201 5900 6e02 5800  ..t.d.....Y.n.X.
-000017e0: 7c02 5300 2903 615e 0100 000a 2020 2020  |.S.).a^....    
-000017f0: 436f 6d70 7574 6573 2074 6865 2062 6573  Computes the bes
-00001800: 7420 6669 7420 7061 7261 6d65 7465 7273  t fit parameters
-00001810: 2066 6f72 2074 6865 2053 5028 6b29 206d   for the SP(k) m
-00001820: 6f64 656c 2061 7420 6120 7370 6563 6966  odel at a specif
-00001830: 6963 2072 6564 7368 6966 742e 200a 0a20  ic redshift. .. 
-00001840: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00001850: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00001860: 2053 4f20 3a20 696e 740a 2020 2020 2020   SO : int.      
-00001870: 2020 7370 6865 7269 6361 6c20 6f76 6572    spherical over
-00001880: 2d64 656e 7369 7479 2e20 4f6e 6c79 2061  -density. Only a
-00001890: 6363 6570 7473 2032 3030 206f 7220 3530  ccepts 200 or 50
-000018a0: 300a 2020 2020 7a20 3a20 666c 6f61 740a  0.    z : float.
-000018b0: 2020 2020 2020 2020 7265 6473 6869 6674          redshift
-000018c0: 207a 2e20 4f6e 6c79 2061 6363 6570 7473   z. Only accepts
-000018d0: 2076 616c 7565 7320 6f66 207a 203c 3d20   values of z <= 
-000018e0: 3320 0a0a 2020 2020 5265 7475 726e 730a  3 ..    Returns.
-000018f0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00001900: 7061 7261 6d73 3a20 6469 6374 0a20 2020  params: dict.   
-00001910: 2020 2020 2062 6573 7420 6669 7420 7061       best fit pa
-00001920: 7261 6d65 7465 7273 2066 6f72 2074 6865  rameters for the
-00001930: 2073 7065 6369 6669 6564 2053 4f20 616e   specified SO an
-00001940: 6420 7a2e 0a20 2020 2072 0400 0000 7a95  d z..    r....z.
-00001950: 1b5b 3931 6d0a 2020 2020 2020 2020 2020  .[91m.          
-00001960: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-00001970: 6865 7269 6361 6c20 6f76 6572 6465 6e73  herical overdens
-00001980: 6974 7920 7368 6f75 6c64 2062 6520 7370  ity should be sp
-00001990: 6563 6966 6965 642e 200a 2020 2020 2020  ecified. .      
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 506c 6561 7365 2075 7365 2032 3030    Please use 200
-000019c0: 206f 7220 3530 3020 0a20 2020 2020 2020   or 500 .       
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 201b 5b30 6d29 04da 0e5f 6265 7374 5f66   .[0m)..._best_f
-000019f0: 6974 5f76 616c 7372 3900 0000 7218 0000  it_valsr9...r...
-00001a00: 0072 2700 0000 2904 722b 0000 0072 2c00  .r'...).r+...r,.
-00001a10: 0000 721d 0000 005a 0770 6172 616d 5f69  ..r....Z.param_i
-00001a20: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001a30: 2a00 0000 d100 0000 730e 0000 0000 1004  *.......s.......
-00001a40: 0102 0110 0124 0106 010e 0472 2a00 0000  .....$.....r*...
-00001a50: 6306 0000 0000 0000 0000 0000 000a 0000  c...............
-00001a60: 0006 0000 0043 0000 0073 5e00 0000 6401  .....C...s^...d.
-00001a70: 7c05 6a00 7c05 6a01 1b00 1b00 7d06 7402  |.j.|.j.....}.t.
-00001a80: a003 7c00 a101 6402 1b00 7d07 7402 a004  ..|...d...}.t...
-00001a90: 7c03 6403 1b00 7c01 6404 1800 a102 7d08  |.d...|.d.....}.
-00001aa0: 7402 a004 7c05 a005 7c04 a101 7c05 a005  t...|...|...|...
-00001ab0: 6405 a101 1b00 7c02 a102 7d09 7c06 7c07  d.....|...}.|.|.
-00001ac0: 1400 7c08 1400 7c09 1400 5300 2906 61a9  ..|...|...S.).a.
-00001ad0: 0200 000a 2020 2020 5265 7475 726e 7320  ....    Returns 
-00001ae0: 6120 7265 6473 6869 6674 2064 6570 656e  a redshift depen
-00001af0: 6465 6e74 2070 6f77 6572 2d6c 6177 2066  dent power-law f
-00001b00: 756e 6374 696f 6e20 6f66 2074 6865 2062  unction of the b
-00001b10: 6172 796f 6e20 6672 6163 7469 6f6e 2061  aryon fraction a
-00001b20: 7320 6120 6675 6e63 7469 6f6e 206f 6620  s a function of 
-00001b30: 6861 6c6f 206d 6173 7320 0a20 2020 2061  halo mass .    a
-00001b40: 7320 696e 2041 6b69 6e6f 2065 7420 616c  s in Akino et al
-00001b50: 2e20 3230 3232 0a0a 2020 2020 5061 7261  . 2022..    Para
-00001b60: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00001b70: 2d2d 2d2d 2d0a 2020 2020 616c 7068 6120  -----.    alpha 
-00001b80: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-00001b90: 7365 7473 2074 6865 2070 6f77 6572 206c  sets the power l
-00001ba0: 6177 2063 6f6e 7374 616e 740a 2020 2020  aw constant.    
-00001bb0: 6265 7461 203a 2066 6c6f 6174 0a20 2020  beta : float.   
-00001bc0: 2020 2020 2073 6574 7320 7468 6520 706f       sets the po
-00001bd0: 7765 7220 6c61 7720 6578 706f 6e65 6e74  wer law exponent
-00001be0: 0a20 2020 2067 616d 6d61 203a 2066 6c6f  .    gamma : flo
-00001bf0: 6174 0a20 2020 2020 2020 2073 6574 7320  at.        sets 
-00001c00: 706f 7765 7220 6c61 7720 7265 6473 6869  power law redshi
-00001c10: 6674 2064 6570 656e 6465 6e63 652e 200a  ft dependence. .
-00001c20: 2020 2020 6d5f 6861 6c6f 3a20 6172 7261      m_halo: arra
-00001c30: 7920 6f66 2066 6c6f 6174 0a20 2020 2020  y of float.     
-00001c40: 2020 2068 616c 6f20 6d61 7373 2069 6e20     halo mass in 
-00001c50: 4d5f 7375 6e20 756e 6974 730a 2020 2020  M_sun units.    
-00001c60: 7a20 3a20 666c 6f61 740a 2020 2020 2020  z : float.      
-00001c70: 2020 7265 6473 6869 6674 207a 0a20 2020    redshift z.   
-00001c80: 2063 6f73 6d6f 3a20 6173 7472 6f70 7920   cosmo: astropy 
-00001c90: 636f 736d 6f6c 6f67 7920 6f62 6a65 6374  cosmology object
-00001ca0: 0a20 2020 2020 2020 2061 7374 726f 7079  .        astropy
-00001cb0: 2063 6f73 6d6f 6c6f 6779 206f 626a 6563   cosmology objec
-00001cc0: 7420 7769 7468 2074 6865 2064 6573 6972  t with the desir
-00001cd0: 6564 2063 6f73 6d6f 6c6f 6779 0a20 2020  ed cosmology.   
-00001ce0: 2020 2020 200a 2020 2020 5265 7475 726e       .    Return
-00001cf0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00001d00: 2020 6f75 7470 7574 3a20 6172 7261 7920    output: array 
-00001d10: 6f66 2066 6c6f 6174 0a20 2020 2020 2020  of float.       
-00001d20: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
-00001d30: 206e 6f72 6d61 6c69 7365 6420 6279 2074   normalised by t
-00001d40: 6865 2055 6e69 7665 7273 616c 2062 6172  he Universal bar
-00001d50: 796f 6e20 6672 6163 7469 6f6e 3a20 665f  yon fraction: f_
-00001d60: 6220 2f20 284f 6d65 6761 5f62 202f 204f  b / (Omega_b / O
-00001d70: 6d65 6761 5f6d 290a 2020 2020 6762 a1d6  mega_m).    gb..
-00001d80: 34ef 38c5 3fe9 6400 0000 6700 0090 1ec4  4.8.?.d...g.....
-00001d90: bcd6 4272 0400 0000 6733 3333 3333 33d3  ..Br....g333333.
-00001da0: 3f29 06da 034f 6230 5a03 4f6d 3072 0a00  ?)...Ob0Z.Om0r..
-00001db0: 0000 7230 0000 0072 0b00 0000 5a05 6566  ..r0...r....Z.ef
-00001dc0: 756e 6329 0a72 1900 0000 721a 0000 0072  unc).r....r....r
-00001dd0: 1b00 0000 720c 0000 0072 2c00 0000 da05  ....r....r,.....
-00001de0: 636f 736d 6f72 3200 0000 7233 0000 0072  cosmor2...r3...r
-00001df0: 3400 0000 da01 4472 1100 0000 7211 0000  4.....Dr....r...
-00001e00: 0072 1200 0000 da06 5f61 6b69 6e6f ed00  .r......_akino..
-00001e10: 0000 730a 0000 0000 1a10 010e 0114 011c  ..s.............
-00001e20: 0272 4300 0000 6305 0000 0000 0000 0000  .rC...c.........
-00001e30: 0000 0007 0000 0004 0000 0043 0000 0073  ...........C...s
-00001e40: 2200 0000 6401 7c04 1b00 7d05 7c01 7c02  "...d.|...}.|.|.
-00001e50: 7c00 1800 1b00 7d06 7400 a001 7c05 7c06  |.....}.t...|.|.
-00001e60: 1400 a101 5300 2902 61a0 0200 000a 2020  ....S.).a.....  
-00001e70: 2020 5072 6f70 6167 6174 6573 2074 6865    Propagates the
-00001e80: 2073 7570 7072 6573 7369 6f6e 2075 6e63   suppression unc
-00001e90: 6572 7461 696e 7479 2074 6f20 7468 6520  ertainty to the 
-00001ea0: 6261 7279 6f6e 2066 7261 6374 696f 6e0a  baryon fraction.
-00001eb0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00001ec0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00001ed0: 2020 2073 7570 3a20 6172 7261 7920 6f66     sup: array of
-00001ee0: 2066 6c6f 6174 0a20 2020 2020 2020 2061   float.        a
-00001ef0: 7272 6179 2077 6974 6820 7468 6520 7375  rray with the su
-00001f00: 7070 7265 7373 696f 6e20 6f66 2074 6865  ppression of the
-00001f10: 2074 6f74 616c 206d 6174 7465 7220 706f   total matter po
-00001f20: 7765 7220 7370 6563 7472 756d 2061 7320  wer spectrum as 
-00001f30: 6120 6675 6e63 7469 6f6e 206f 6620 7363  a function of sc
-00001f40: 616c 652e 0a20 2020 206c 616d 6264 615f  ale..    lambda_
-00001f50: 6675 6e63 7420 3a20 6172 7261 790a 2020  funct : array.  
-00001f60: 2020 2020 2020 6c61 6d62 6461 2066 756e        lambda fun
-00001f70: 6374 696f 6e20 666f 7220 6120 7370 6563  ction for a spec
-00001f80: 6966 6963 2072 6564 7368 6966 742e 2044  ific redshift. D
-00001f90: 6566 696e 6564 2069 6e20 6571 2e28 3829  efined in eq.(8)
-00001fa0: 2069 6e20 5361 6c63 6964 6f20 6574 2061   in Salcido et a
-00001fb0: 6c2e 2028 3230 3232 292e 0a20 2020 206d  l. (2022)..    m
-00001fc0: 755f 6675 6e63 7420 3a20 6172 7261 790a  u_funct : array.
-00001fd0: 2020 2020 2020 2020 6d75 2066 756e 6374          mu funct
-00001fe0: 696f 6e20 666f 7220 6120 7370 6563 6966  ion for a specif
-00001ff0: 6963 2072 6564 7368 6966 742e 2044 6566  ic redshift. Def
-00002000: 696e 6564 2069 6e20 6571 2e28 3829 2069  ined in eq.(8) i
-00002010: 6e20 5361 6c63 6964 6f20 6574 2061 6c2e  n Salcido et al.
-00002020: 2028 3230 3232 292e 0a20 2020 206e 755f   (2022)..    nu_
-00002030: 6675 6e63 7420 3a20 6172 7261 790a 2020  funct : array.  
-00002040: 2020 2020 2020 6e75 2066 756e 6374 696f        nu functio
-00002050: 6e20 666f 7220 6120 7370 6563 6966 6963  n for a specific
-00002060: 2072 6564 7368 6966 742e 2044 6566 696e   redshift. Defin
-00002070: 6564 2069 6e20 6571 2e28 3829 2069 6e20  ed in eq.(8) in 
-00002080: 5361 6c63 6964 6f20 6574 2061 6c2e 2028  Salcido et al. (
-00002090: 3230 3232 292e 0a20 2020 2020 2020 200a  2022)..        .
-000020a0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000020b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6f75 7470  -------.    outp
-000020c0: 7574 3a20 6172 7261 7920 6f66 2066 6c6f  ut: array of flo
-000020d0: 6174 0a20 2020 2020 2020 2061 7272 6179  at.        array
-000020e0: 2077 6974 6820 7468 6520 6572 726f 7220   with the error 
-000020f0: 696e 2074 6865 2062 6172 796f 6e20 6672  in the baryon fr
-00002100: 6163 7469 6f6e 2e20 0a20 2020 20e9 ffff  action. .    ...
-00002110: ffff 2902 720a 0000 00da 0361 6273 2907  ..).r......abs).
-00002120: da03 7375 70da 0565 7272 6f72 5a0c 6c61  ..sup..errorZ.la
-00002130: 6d62 6461 5f66 756e 6374 5a08 6d75 5f66  mbda_functZ.mu_f
-00002140: 756e 6374 5a07 6e75 5f66 756e 6372 3200  unctZ.nu_funcr2.
-00002150: 0000 7233 0000 0072 1100 0000 7211 0000  ..r3...r....r...
-00002160: 0072 1200 0000 da12 5f5f 7072 6f70 6167  .r......__propag
-00002170: 6174 655f 6572 726f 7273 0f01 0000 7306  ate_errors....s.
-00002180: 0000 0000 1408 010c 0272 4800 0000 46e7  .........rH...F.
-00002190: 9a99 9999 9999 b93f 7221 0000 0072 3f00  .......?r!...r?.
-000021a0: 0000 6311 0000 0000 0000 0000 0000 002f  ..c............/
-000021b0: 0000 0008 0000 0043 0000 0073 b603 0000  .......C...s....
-000021c0: 7c01 6401 6b00 7212 7400 6402 8301 6403  |.d.k.r.t.d...d.
-000021d0: 8202 7c01 6404 6b04 7224 7400 6405 8301  ..|.d.k.r$t.d...
-000021e0: 6403 8202 7c01 6406 6b00 723a 7401 6a02  d...|.d.k.r:t.j.
-000021f0: 6407 6408 6409 8d02 0100 7c0d 640a 6b04  d.d.d.....|.d.k.
-00002200: 724c 7400 640b 8301 6403 8202 7c0d 640c  rLt.d...d...|.d.
-00002210: 6b04 7262 7401 6a02 640d 6408 6409 8d02  k.rbt.j.d.d.d...
-00002220: 0100 7c0b 6403 6b09 727a 7c0b 6a03 737a  ..|.d.k.rz|.j.sz
-00002230: 7400 640e 8301 6403 8202 7404 7c00 7c01  t.d...d...t.|.|.
-00002240: 8302 7d11 7405 a006 7405 a007 7405 a008  ..}.t...t...t...
-00002250: 7c0c a101 7405 a008 7c0d a101 7c0e a103  |...t...|...|...
-00002260: 640f a102 7d12 7405 a008 7c12 a101 7d13  d...}.t...|...}.
-00002270: 7409 7c12 7c11 8302 7d14 7c02 6403 6b09  t.|.|...}.|.d.k.
-00002280: 73cc 7c03 6403 6b09 9001 7210 7c10 72e0  s.|.d.k...r.|.r.
-00002290: 740a 6410 7c01 7c04 6602 1600 8301 0100  t.d.|.|.f.......
-000022a0: 7a16 740b 6411 7c14 1300 7c02 7c03 7c04  z.t.d.|...|.|.|.
-000022b0: 8304 7d15 5700 6e16 0100 0100 0100 7400  ..}.W.n.......t.
-000022c0: 6412 8301 6403 8202 5900 6e02 5800 6eb4  d...d...Y.n.X.n.
-000022d0: 7c05 6403 6b09 9001 7324 7c06 6403 6b09  |.d.k...s$|.d.k.
-000022e0: 9001 7280 7c10 9001 7236 740a 6413 7c01  ..r.|...r6t.d.|.
-000022f0: 1600 8301 0100 7a32 740c 7405 a008 7c05  ......z2t.t...|.
-00002300: a101 7405 a008 7c06 a101 8302 7d16 7c07  ..t...|.....}.|.
-00002310: 9001 725a 6414 7c16 5f0d 6411 7c16 7c14  ..rZd.|._.d.|.|.
-00002320: 8301 1300 7d15 5700 6e14 0100 0100 0100  ....}.W.n.......
-00002330: 7400 6415 8301 8201 5900 6e02 5800 6e44  t.d.....Y.n.X.nD
-00002340: 7c10 9001 7292 740a 6416 7c01 1600 8301  |...r.t.d.|.....
-00002350: 0100 7a1a 740e 7c08 7c09 7c0a 6411 7c14  ..z.t.|.|.|.d.|.
-00002360: 1300 7c01 7c0b 8306 7d15 5700 6e16 0100  ..|.|...}.W.n...
-00002370: 0100 0100 7400 6417 8301 6403 8202 5900  ....t.d...d...Y.
-00002380: 6e02 5800 740f 7c00 7c01 6411 7c14 1300  n.X.t.|.|.d.|...
-00002390: 8303 5c02 7d17 7d18 7c15 7c17 6b00 7d19  ..\.}.}.|.|.k.}.
-000023a0: 7c15 7c18 6b04 7d1a 7c14 7c19 1900 7d1b  |.|.k.}.|.|...}.
-000023b0: 7410 7c19 8301 9002 7220 7401 6a02 6418  t.|.....r t.j.d.
-000023c0: 6411 7c1b a011 a100 1300 6411 7c1b a012  d.|.......d.|...
-000023d0: a100 1300 6602 1600 6408 6409 8d02 0100  ....f...d.d.....
-000023e0: 7c14 7c1a 1900 7d1c 7410 7c1a 8301 9002  |.|...}.t.|.....
-000023f0: 7258 7401 6a02 6419 6411 7c1c a011 a100  rXt.j.d.d.|.....
-00002400: 1300 6411 7c1c a012 a100 1300 6602 1600  ..d.|.......f...
-00002410: 6408 6409 8d02 0100 7405 a013 7c19 7c1a  d.d.....t...|.|.
-00002420: a102 7d1d 7414 7c13 7c11 8302 7d1e 7415  ..}.t.|.|...}.t.
-00002430: 7c13 7c11 8302 7d1f 7416 7c13 7c11 8302  |.|...}.t.|.|...
-00002440: 7d20 7c1e 7c1e 7c1f 1800 7405 a017 7c20  } |.|.|...t...| 
-00002450: 0b00 7c15 1400 a101 1400 1800 7d21 7405  ..|.........}!t.
-00002460: 6a18 7c21 7c1d 3c00 7c0f 9003 72aa 7419  j.|!|.<.|...r.t.
-00002470: a01a 741b 641a 741c 7c00 8301 1700 641b  ..t.d.t.|.....d.
-00002480: 1700 a102 a01d 641c a101 a01e a100 7d22  ......d.......}"
-00002490: 7405 6a1f 7c22 641d 641e 641f 8d03 7d23  t.j.|"d.d.d...}#
-000024a0: 7c23 6403 6403 8502 6401 641e 6408 6703  |#d.d...d.d.d.g.
-000024b0: 6602 1900 7d24 7420 7c24 7c23 6403 6403  f...}$t |$|#d.d.
-000024c0: 8502 6420 6602 1900 6414 6421 8d03 7d25  ..d f...d.d!..}%
-000024d0: 7420 7c24 7c23 6403 6403 8502 6422 6602  t |$|#d.d...d"f.
-000024e0: 1900 6414 6421 8d03 7d26 7420 7c24 7c23  ..d.d!..}&t |$|#
-000024f0: 6403 6403 8502 640f 6602 1900 6414 6421  d.d...d.f...d.d!
-00002500: 8d03 7d27 7420 7c24 7c23 6403 6403 8502  ..}'t |$|#d.d...
-00002510: 6423 6602 1900 6414 6421 8d03 7d28 7405  d#f...d.d!..}(t.
-00002520: a021 7c12 7c01 a102 7d29 7405 a022 7c12  .!|.|...})t.."|.
-00002530: 7c15 7c29 6703 a101 7d2a 7c25 7c2a 8301  |.|)g...}*|%|*..
-00002540: 7d2b 7c26 7c2a 8301 7d2c 7c27 7c2a 8301  }+|&|*..},|'|*..
-00002550: 7d2d 7c28 7c2a 8301 7d2e 7c12 7c21 7c2b  }-|(|*..}.|.|!|+
-00002560: 7c2c 7c2d 7c2e 6606 5300 7c12 7c21 6602  |,|-|.f.S.|.|!f.
-00002570: 5300 6403 5300 2924 7536 0d00 000a 2020  S.d.S.)$u6....  
-00002580: 2020 5265 7475 726e 7320 7468 6520 7375    Returns the su
-00002590: 7070 7265 7373 696f 6e20 6f66 2074 6865  ppression of the
-000025a0: 2074 6f74 616c 206d 6174 7465 7220 706f   total matter po
-000025b0: 7765 7220 7370 6563 7472 756d 2061 7320  wer spectrum as 
-000025c0: 6120 6675 6e63 7469 6f6e 206f 6620 7363  a function of sc
-000025d0: 616c 6520 276b 2720 7573 696e 6720 7468  ale 'k' using th
-000025e0: 6520 5350 286b 2920 6d6f 6465 6c2e 0a20  e SP(k) model.. 
-000025f0: 2020 2041 7574 6f6d 6174 6963 616c 6c79     Automatically
-00002600: 2073 656c 6563 7473 2074 6865 2072 6571   selects the req
-00002610: 7569 7265 6420 6f70 7469 6d61 6c20 6d61  uired optimal ma
-00002620: 7373 2061 7320 6120 6675 6e63 7469 6f6e  ss as a function
-00002630: 206f 6620 7363 616c 6520 616e 6420 7265   of scale and re
-00002640: 6473 6869 6674 2e20 5265 7175 6972 6573  dshift. Requires
-00002650: 2074 6865 2062 6172 796f 6e20 0a20 2020   the baryon .   
-00002660: 2066 7261 6374 696f 6e20 2d20 6861 6c6f   fraction - halo
-00002670: 206d 6173 7320 7265 6c61 7469 6f6e 2c20   mass relation, 
-00002680: 6569 7468 6572 2062 7920 7370 6563 6966  either by specif
-00002690: 7969 6e67 2070 6f77 6572 2d6c 6177 2066  ying power-law f
-000026a0: 6974 7469 6e67 2070 6172 616d 6574 6572  itting parameter
-000026b0: 732c 206f 7220 6e6f 6e2d 7061 7261 6d65  s, or non-parame
-000026c0: 7472 6963 200a 2020 2020 7072 6f76 696e  tric .    provin
-000026d0: 6720 6172 7261 7973 2077 6974 6820 6662  g arrays with fb
-000026e0: 2061 6e64 204d 5f68 616c 6f20 6174 2061   and M_halo at a
-000026f0: 2073 7065 6369 6669 6320 7265 6473 6869   specific redshi
-00002700: 6674 2e20 5468 6520 6675 6e63 7469 6f6e  ft. The function
-00002710: 2061 6363 6570 7473 2061 2073 696d 706c   accepts a simpl
-00002720: 6520 706f 7765 7220 6c61 7720 666f 726d  e power law form
-00002730: 200a 2020 2020 6f72 2061 6e20 416b 696e   .    or an Akin
-00002740: 6f20 6574 2061 6c20 3230 3232 2066 7563  o et al 2022 fuc
-00002750: 6e74 696f 6e61 6c20 666f 726d 2e20 4966  ntional form. If
-00002760: 2061 206e 6f6e 2d70 6172 616d 6574 7269   a non-parametri
-00002770: 6320 7265 6c61 7469 6f6e 2069 7320 6769  c relation is gi
-00002780: 7665 6e2c 2061 6e20 0a20 2020 2069 6e74  ven, an .    int
-00002790: 6572 706f 6c61 746f 7220 6973 2075 7365  erpolator is use
-000027a0: 6420 746f 2063 6f6d 7075 7465 2066 6220  d to compute fb 
-000027b0: 6174 2074 6865 206f 7074 696d 616c 206d  at the optimal m
-000027c0: 6173 732e 200a 0a20 2020 2050 6172 616d  ass. ..    Param
-000027d0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-000027e0: 2d2d 2d2d 0a20 2020 2053 4f20 3a20 696e  ----.    SO : in
-000027f0: 740a 2020 2020 2020 2020 7370 6865 7269  t.        spheri
-00002800: 6361 6c20 6f76 6572 2d64 656e 7369 7479  cal over-density
-00002810: 2e20 4f6e 6c79 2061 6363 6570 7473 2032  . Only accepts 2
-00002820: 3030 206f 7220 3530 300a 2020 2020 7a20  00 or 500.    z 
-00002830: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-00002840: 7265 6473 6869 6674 207a 2e20 4f6e 6c79  redshift z. Only
-00002850: 2061 6363 6570 7473 2076 616c 7565 7320   accepts values 
-00002860: 6f66 207a 203c 3d20 330a 2020 2020 6662  of z <= 3.    fb
-00002870: 5f61 203a 2066 6c6f 6174 2c20 6f70 7469  _a : float, opti
-00002880: 6f6e 616c 0a20 2020 2020 2020 2070 6f77  onal.        pow
-00002890: 6572 206c 6177 2063 6f6e 7374 616e 740a  er law constant.
-000028a0: 2020 2020 6662 5f70 6f77 203a 2066 6c6f      fb_pow : flo
-000028b0: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-000028c0: 2020 2020 2070 6f77 6572 206c 6177 2065       power law e
-000028d0: 7870 6f6e 656e 740a 2020 2020 6662 5f70  xponent.    fb_p
-000028e0: 6976 6f74 203a 2066 6c6f 6174 2c20 6f70  ivot : float, op
-000028f0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00002900: 310a 2020 2020 2020 2020 706f 7765 7220  1.        power 
-00002910: 6c61 7720 7069 766f 7420 706f 696e 742e  law pivot point.
-00002920: 200a 2020 2020 6662 203a 2061 7272 6179   .    fb : array
-00002930: 206f 6620 666c 6f61 742c 206f 7074 696f   of float, optio
-00002940: 6e61 6c0a 2020 2020 2020 2020 6172 7261  nal.        arra
-00002950: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00002960: 2028 6269 6e6e 6564 2920 6261 7279 6f6e   (binned) baryon
-00002970: 2066 7261 6374 696f 6e20 6e6f 726d 616c   fraction normal
-00002980: 6973 6564 2062 7920 7468 6520 756e 6976  ised by the univ
-00002990: 6572 7361 6c20 6261 7279 6f6e 2066 7261  ersal baryon fra
-000029a0: 6374 696f 6e3a 200a 2020 2020 2020 2020  ction: .        
-000029b0: 665f 6220 2f20 284f 6d65 6761 5f62 202f  f_b / (Omega_b /
-000029c0: 204f 6d65 6761 5f6d 2920 666f 7220 7468   Omega_m) for th
-000029d0: 6520 6662 202d 204d 2d68 616c 6f20 7265  e fb - M-halo re
-000029e0: 6c61 7469 6f6e 2e0a 2020 2020 4d5f 6861  lation..    M_ha
-000029f0: 6c6f 203a 2061 7272 6179 206f 6620 666c  lo : array of fl
-00002a00: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-00002a10: 2020 2020 2020 6172 7261 7920 636f 6e74        array cont
-00002a20: 6169 6e69 6e67 2074 6865 2028 6269 6e6e  aining the (binn
-00002a30: 6564 2920 6861 6c6f 206d 6173 7320 666f  ed) halo mass fo
-00002a40: 7220 7468 6520 6662 202d 204d 2d68 616c  r the fb - M-hal
-00002a50: 6f20 7265 6c61 7469 6f6e 2069 6e20 4d5f  o relation in M_
-00002a60: 7375 6e20 756e 6974 732e 0a20 2020 2020  sun units..     
-00002a70: 2020 2046 6f72 2069 6e74 6572 706f 6c61     For interpola
-00002a80: 7469 6f6e 2c20 6f75 742d 6f66 2d62 6f75  tion, out-of-bou
-00002a90: 6e64 7320 706f 696e 7473 2072 6574 7572  nds points retur
-00002aa0: 6e20 4e61 4e73 2e0a 2020 2020 6578 7472  n NaNs..    extr
-00002ab0: 6170 6f6c 6174 653a 2062 6f6f 6c65 616e  apolate: boolean
-00002ac0: 2c20 6465 6661 756c 7420 4661 6c73 650a  , default False.
-00002ad0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00002ae0: 746f 2065 7874 7261 706f 6c61 7465 2074  to extrapolate t
-00002af0: 6f20 6f75 742d 6f66 2d62 6f75 6e64 7320  o out-of-bounds 
-00002b00: 706f 696e 7473 2062 6173 6564 206f 6e20  points based on 
-00002b10: 6669 7273 7420 616e 6420 6c61 7374 2069  first and last i
-00002b20: 6e74 6572 7661 6c73 2c20 6f72 2074 6f20  ntervals, or to 
-00002b30: 7265 7475 726e 204e 614e 732e 0a20 2020  return NaNs..   
-00002b40: 2061 6c70 6861 203a 2066 6c6f 6174 2c20   alpha : float, 
-00002b50: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00002b60: 2073 6574 7320 7468 6520 416b 696e 6f20   sets the Akino 
-00002b70: 706f 7765 7220 6c61 7720 636f 6e73 7461  power law consta
-00002b80: 6e74 0a20 2020 2062 6574 6120 3a20 666c  nt.    beta : fl
-00002b90: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-00002ba0: 2020 2020 2020 7365 7473 2074 6865 2041        sets the A
-00002bb0: 6b69 6e6f 2070 6f77 6572 206c 6177 2065  kino power law e
-00002bc0: 7870 6f6e 656e 740a 2020 2020 6761 6d6d  xponent.    gamm
-00002bd0: 6120 3a20 666c 6f61 742c 206f 7074 696f  a : float, optio
-00002be0: 6e61 6c0a 2020 2020 2020 2020 7365 7473  nal.        sets
-00002bf0: 2074 6865 2041 6b69 6e6f 2070 6f77 6572   the Akino power
-00002c00: 206c 6177 2072 6564 7368 6966 7420 6465   law redshift de
-00002c10: 7065 6e64 656e 6365 2e20 0a20 2020 2063  pendence. .    c
-00002c20: 6f73 6d6f 3a20 6173 7472 6f70 7920 636f  osmo: astropy co
-00002c30: 736d 6f6c 6f67 7920 6f62 6a65 6374 2c20  smology object, 
-00002c40: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00002c50: 2061 7374 726f 7079 2063 6f73 6d6f 6c6f   astropy cosmolo
-00002c60: 6779 206f 626a 6563 7420 7769 7468 2074  gy object with t
-00002c70: 6865 2064 6573 6972 6564 2063 6f73 6d6f  he desired cosmo
-00002c80: 6c6f 6779 0a20 2020 206b 5f6d 696e 203a  logy.    k_min :
-00002c90: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-00002ca0: 302e 310a 2020 2020 2020 2020 6d69 6e69  0.1.        mini
-00002cb0: 6d75 6d20 636f 2d6d 6f76 696e 6720 7761  mum co-moving wa
-00002cc0: 7665 6e75 6d62 6572 2069 6e20 756e 6974  venumber in unit
-00002cd0: 7320 5b68 2f4d 7063 5d0a 2020 2020 6b5f  s [h/Mpc].    k_
-00002ce0: 6d61 7820 3a20 666c 6f61 742c 2064 6566  max : float, def
-00002cf0: 6175 6c74 2038 2c20 6d61 7820 3132 0a20  ault 8, max 12. 
-00002d00: 2020 2020 2020 206d 6178 696d 756d 2063         maximum c
-00002d10: 6f2d 6d6f 7669 6e67 2077 6176 656e 756d  o-moving wavenum
-00002d20: 6265 7220 696e 2075 6e69 7473 205b 682f  ber in units [h/
-00002d30: 4d70 635d 2e20 4465 6661 756c 7420 6973  Mpc]. Default is
-00002d40: 2073 6574 2074 6f20 7468 6520 4e79 7175   set to the Nyqu
-00002d50: 6973 7420 6672 6571 7565 6e63 7920 6f66  ist frequency of
-00002d60: 2074 6865 2041 6e74 696c 6c65 730a 2020   the Antilles.  
-00002d70: 2020 2020 2020 7369 6d75 6c61 7469 6f6e        simulation
-00002d80: 7320 2873 6565 2053 616c 6369 646f 2065  s (see Salcido e
-00002d90: 7420 616c 2e20 3230 3232 292e 200a 2020  t al. 2022). .  
-00002da0: 2020 6e20 3a20 696e 742c 2064 6566 6175    n : int, defau
-00002db0: 6c74 2031 3030 0a20 2020 2020 2020 206e  lt 100.        n
-00002dc0: 756d 6265 7220 6f66 2065 7175 616c 6c79  umber of equally
-00002dd0: 2073 7061 6365 6420 636f 2d6d 6f76 696e   spaced co-movin
-00002de0: 6720 7761 7665 6e75 6d62 6572 2069 6e20  g wavenumber in 
-00002df0: 6c6f 672d 7370 6163 6564 2062 6574 7765  log-spaced betwe
-00002e00: 656e 206b 5f6d 696e 2061 6e64 206b 5f6d  en k_min and k_m
-00002e10: 6178 2e0a 2020 2020 6572 726f 7273 203a  ax..    errors :
-00002e20: 2062 6f6f 6c65 616e 2c20 6465 6661 756c   boolean, defaul
-00002e30: 7420 4661 6c73 650a 2020 2020 2020 2020  t False.        
-00002e40: 656e 6162 6c65 7320 6164 6469 7469 6f6e  enables addition
-00002e50: 616c 206f 7574 7075 7420 7769 7468 2074  al output with t
-00002e60: 6865 2062 6f6f 7473 7472 6170 7065 6420  he bootstrapped 
-00002e70: 3638 2520 616e 6420 3935 2520 636f 6e66  68% and 95% conf
-00002e80: 6964 656e 6365 2069 6e74 6572 7661 6c73  idence intervals
-00002e90: 2066 726f 6d20 7374 6174 6973 7469 6361   from statistica
-00002ea0: 6c20 6572 726f 7273 2e0a 2020 2020 7665  l errors..    ve
-00002eb0: 7262 6f73 6520 3a20 626f 6f6c 6561 6e2c  rbose : boolean,
-00002ec0: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
-00002ed0: 2020 2020 2020 7275 6e20 696e 2076 6572        run in ver
-00002ee0: 626f 7365 206d 6f64 650a 2020 2020 2020  bose mode.      
-00002ef0: 2020 0a20 2020 2052 6574 7572 6e73 0a20    .    Returns. 
-00002f00: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 206b     -------.    k
-00002f10: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
-00002f20: 0a20 2020 2020 2020 2061 7272 6179 2077  .        array w
-00002f30: 6974 6820 7468 6520 636f 2d6d 6f76 696e  ith the co-movin
-00002f40: 6720 7761 7665 6e75 6d62 6572 2069 6e20  g wavenumber in 
-00002f50: 756e 6974 7320 5b68 2f4d 7063 5d0a 2020  units [h/Mpc].  
-00002f60: 2020 7375 703a 2061 7272 6179 206f 6620    sup: array of 
-00002f70: 666c 6f61 740a 2020 2020 2020 2020 6172  float.        ar
-00002f80: 7261 7920 7769 7468 2074 6865 2073 7570  ray with the sup
-00002f90: 7072 6573 7369 6f6e 206f 6620 7468 6520  pression of the 
-00002fa0: 746f 7461 6c20 6d61 7474 6572 2070 6f77  total matter pow
-00002fb0: 6572 2073 7065 6374 7275 6d20 6173 2061  er spectrum as a
-00002fc0: 2066 756e 6374 696f 6e20 6f66 2073 6361   function of sca
-00002fd0: 6c65 0a20 2020 2065 7272 6f72 5f36 385f  le.    error_68_
-00002fe0: 6d20 3a20 6172 7261 7920 6f66 2066 6c6f  m : array of flo
-00002ff0: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-00003000: 2020 2020 2061 7272 6179 2077 6974 6820       array with 
-00003010: 7468 6520 2d31 2073 6967 6d61 2063 6f6e  the -1 sigma con
-00003020: 6669 6465 6e63 6520 696e 7465 7276 616c  fidence interval
-00003030: 200a 2020 2020 6572 726f 725f 3638 5f70   .    error_68_p
-00003040: 203a 2061 7272 6179 206f 6620 666c 6f61   : array of floa
-00003050: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-00003060: 2020 2020 6172 7261 7920 7769 7468 2074      array with t
-00003070: 6865 202b 3120 7369 676d 6120 636f 6e66  he +1 sigma conf
-00003080: 6964 656e 6365 2069 6e74 6572 7661 6c20  idence interval 
-00003090: 0a20 2020 2065 7272 6f72 5f39 355f 6d20  .    error_95_m 
-000030a0: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
-000030b0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-000030c0: 2020 2061 7272 6179 2077 6974 6820 7468     array with th
-000030d0: 6520 2d32 2073 6967 6d61 2063 6f6e 6669  e -2 sigma confi
-000030e0: 6465 6e63 6520 696e 7465 7276 616c 200a  dence interval .
-000030f0: 2020 2020 6572 726f 725f 3935 5f70 203a      error_95_p :
-00003100: 2061 7272 6179 206f 6620 666c 6f61 742c   array of float,
-00003110: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00003120: 2020 6172 7261 7920 7769 7468 2074 6865    array with the
-00003130: 202b 3220 7369 676d 6120 636f 6e66 6964   +2 sigma confid
-00003140: 656e 6365 2069 6e74 6572 7661 6c20 0a0a  ence interval ..
-00003150: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
-00003160: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2054 6865  --------.    The
-00003170: 206d 6178 696d 756d 2063 6f2d 6d6f 7669   maximum co-movi
-00003180: 6e67 2077 6176 656e 756d 6265 7220 696e  ng wavenumber in
-00003190: 2075 6e69 7473 205b 682f 4d70 635d 2069   units [h/Mpc] i
-000031a0: 7320 7365 7420 746f 2074 6865 204e 7971  s set to the Nyq
-000031b0: 7569 7374 2066 7265 7175 656e 6379 206f  uist frequency o
-000031c0: 6620 7468 6520 416e 7469 6c6c 6573 2073  f the Antilles s
-000031d0: 696d 756c 6174 696f 6e73 200a 2020 2020  imulations .    
-000031e0: 2873 6565 2053 616c 6369 646f 2065 7420  (see Salcido et 
-000031f0: 616c 2e20 3230 3232 292e 2041 6c74 686f  al. 2022). Altho
-00003200: 7567 6820 5350 286b 2920 7761 7320 6669  ugh SP(k) was fi
-00003210: 7474 6564 2075 7020 746f 206b 203d 2031  tted up to k = 1
-00003220: 3220 5b68 2f4d 7063 5d2c 2077 6520 6361  2 [h/Mpc], we ca
-00003230: 7574 696f 6e20 7468 6520 7573 6572 2074  ution the user t
-00003240: 6861 7420 7365 7474 696e 6720 0a20 2020  hat setting .   
-00003250: 20f0 9d91 9820 3e20 f09d 9198 4e79 2028   .... > ....Ny (
-00003260: 3820 5b68 2f4d 7063 5d29 206d 6967 6874  8 [h/Mpc]) might
-00003270: 206e 6f74 2062 6520 7265 7072 6573 656e   not be represen
-00003280: 7461 7469 7665 206f 6620 7468 6520 7472  tative of the tr
-00003290: 7565 2075 6e63 6572 7461 696e 7469 6573  ue uncertainties
-000032a0: 2069 6e20 7468 6520 6461 7461 2e20 0a20   in the data. . 
-000032b0: 2020 2072 0100 0000 fa1c 1b5b 3931 6d49     r.......[91mI
-000032c0: 6e63 6f72 7265 6374 2072 6564 7368 6966  ncorrect redshif
-000032d0: 742e 1b5b 306d 4ee9 0300 0000 fa46 1b5b  t..[0mN......F.[
-000032e0: 3931 6d70 792d 7370 6b20 7761 7320 6361  91mpy-spk was ca
-000032f0: 6c69 6272 6174 6564 2075 7020 746f 207a  librated up to z
-00003300: 203d 2033 2e30 2e20 506c 6561 7365 2073   = 3.0. Please s
-00003310: 7065 6369 6679 207a 203c 3d20 332e 3020  pecify z <= 3.0 
-00003320: 1b5b 306d e700 0000 0000 00c0 3ffa 751b  .[0m........?.u.
-00003330: 5b33 336d 7079 2d73 706b 2077 6173 2063  [33mpy-spk was c
-00003340: 616c 6962 7261 7465 6420 646f 776e 2074  alibrated down t
-00003350: 6f20 7a20 3d20 302e 3132 352e 2052 6564  o z = 0.125. Red
-00003360: 7368 6966 7473 207a 203c 2030 2e31 3235  shifts z < 0.125
-00003370: 206d 6179 206e 6f74 2062 6520 6163 6375   may not be accu
-00003380: 7261 7465 6c79 2072 6570 726f 6475 6365  rately reproduce
-00003390: 6420 6279 2074 6865 206d 6f64 656c 2e20  d by the model. 
-000033a0: 1b5b 306d 7214 0000 0072 2300 0000 7220  .[0mr....r#...r 
-000033b0: 0000 007a 5b1b 5b39 316d 7079 2d73 706b  ...z[.[91mpy-spk
-000033c0: 2077 6173 2063 616c 6962 7261 7465 6420   was calibrated 
-000033d0: 7570 2074 6f20 6b5f 6d61 7820 3d20 3132  up to k_max = 12
-000033e0: 205b 682f 4d70 635d 2050 6c65 6173 6520   [h/Mpc] Please 
-000033f0: 7370 6563 6966 7920 6b5f 6d61 7820 3c3d  specify k_max <=
-00003400: 2031 3220 5b68 2f4d 7063 5d20 1b5b 306d   12 [h/Mpc] .[0m
-00003410: 7221 0000 0072 2200 0000 7a3a 1b5b 3931  r!...r"...z:.[91
-00003420: 6d49 6e63 6f72 7265 6374 2063 6f73 6d6f  mIncorrect cosmo
-00003430: 6c6f 6779 2e20 506c 6561 7365 2073 7065  logy. Please spe
-00003440: 6369 6679 204f 6d65 6761 5f62 6172 796f  cify Omega_baryo
-00003450: 6e2e 1b5b 306d e906 0000 007a 5c1b 5b33  n..[0m.....z\.[3
-00003460: 366d 5573 696e 6720 706f 7765 722d 6c61  6mUsing power-la
-00003470: 7720 6669 7420 666f 7220 6662 202d 204d  w fit for fb - M
-00003480: 5f68 616c 6f20 6174 207a 3d25 2e33 662c  _halo at z=%.3f,
-00003490: 206e 6f72 6d61 6c69 7365 6420 6174 204d   normalised at M
-000034a0: 5f68 616c 6f20 3d20 252e 3265 205b 4d5f  _halo = %.2e [M_
-000034b0: 7375 6e5d 201b 5b30 6d72 2500 0000 7a62  sun] .[0mr%...zb
-000034c0: 1b5b 3931 6d57 6865 6e20 7573 696e 6720  .[91mWhen using 
-000034d0: 6120 706f 7765 722d 6c61 772c 2062 6f74  a power-law, bot
-000034e0: 6820 7061 7261 6d65 7465 7273 2073 686f  h parameters sho
-000034f0: 756c 6420 6265 2067 6976 656e 2e20 506c  uld be given. Pl
-00003500: 6561 7365 2073 7065 6369 6679 3a20 6662  ease specify: fb
-00003510: 5f61 2061 6e64 2066 625f 706f 7720 1b5b  _a and fb_pow .[
-00003520: 306d 7a35 1b5b 3336 6d55 7369 6e67 2062  0mz5.[36mUsing b
-00003530: 696e 6e65 6420 6461 7461 2066 6f72 2066  inned data for f
-00003540: 6220 2d20 4d5f 6861 6c6f 2061 7420 7a3d  b - M_halo at z=
-00003550: 252e 3366 201b 5b30 6d54 7aa7 1b5b 3931  %.3f .[0mTz..[91
-00003560: 6d57 6865 6e20 7573 696e 6720 6269 6e6e  mWhen using binn
-00003570: 6564 2064 6174 612c 2062 6f74 6820 6861  ed data, both ha
-00003580: 6c6f 206d 6173 7320 616e 6420 6261 7279  lo mass and bary
-00003590: 6f6e 2066 7261 6374 696f 6e20 7368 6f75  on fraction shou
-000035a0: 6c64 2062 6520 6769 7665 6e20 6173 206d  ld be given as m
-000035b0: 6f6e 6f74 6f6e 6963 616c 6c79 2069 6e63  onotonically inc
-000035c0: 7265 6173 696e 6720 6172 7261 7973 2e20  reasing arrays. 
-000035d0: 506c 6561 7365 2073 7065 6369 6679 3a20  Please specify: 
-000035e0: 4d5f 6861 6c6f 2028 6172 7261 7929 2061  M_halo (array) a
-000035f0: 6e64 2066 6220 2861 7272 6179 292e 201b  nd fb (array). .
-00003600: 5b30 6d7a 4d1b 5b33 366d 5573 696e 6720  [0mzM.[36mUsing 
-00003610: 616e 2041 6b69 6e6f 2065 7420 616c 2e20  an Akino et al. 
-00003620: 3230 3232 2070 6f77 6572 2d6c 6177 2066  2022 power-law f
-00003630: 6974 2066 6f72 2066 6220 2d20 4d5f 6861  it for fb - M_ha
-00003640: 6c6f 2061 7420 7a3d 252e 3366 2e20 1b5b  lo at z=%.3f. .[
-00003650: 306d 7a5d 1b5b 3931 6d55 7369 6e67 2061  0mz].[91mUsing a
-00003660: 6e20 416b 696e 6f20 706f 7765 722d 6c61  n Akino power-la
-00003670: 772e 2050 6c65 6173 6520 7370 6563 6966  w. Please specif
-00003680: 793a 2061 6c70 6861 2c20 6265 7461 2c20  y: alpha, beta, 
-00003690: 6761 6d6d 612c 2061 6e64 2063 6f73 6d6f  gamma, and cosmo
-000036a0: 6c6f 6779 2028 636f 736d 6f29 201b 5b30  logy (cosmo) .[0
-000036b0: 6d7a a91b 5b39 316d 466f 756e 6420 6261  mz..[91mFound ba
-000036c0: 7279 6f6e 2066 7261 6374 696f 6e20 7661  ryon fraction va
-000036d0: 6c75 6573 206f 7574 7369 6465 2066 6974  lues outside fit
-000036e0: 7469 6e67 206c 696d 6974 732e 2066 6220  ting limits. fb 
-000036f0: 3c20 6c6f 7765 725f 6c69 6d69 7420 6265  < lower_limit be
-00003700: 7477 6565 6e20 252e 3165 203c 3d20 4d5f  tween %.1e <= M_
-00003710: 6861 6c6f 205b 4d5f 7375 6e5d 203c 3d20  halo [M_sun] <= 
-00003720: 252e 3165 2e20 7375 705f 6d6f 6465 6c28  %.1e. sup_model(
-00003730: 2920 7769 6c6c 2072 6574 7572 6e20 4e61  ) will return Na
-00003740: 4e73 2077 6974 6869 6e20 7468 6f73 6520  Ns within those 
-00003750: 6c69 6d69 7473 2e20 1b5b 306d 7aa9 1b5b  limits. .[0mz..[
-00003760: 3931 6d46 6f75 6e64 2062 6172 796f 6e20  91mFound baryon 
-00003770: 6672 6163 7469 6f6e 2076 616c 7565 7320  fraction values 
-00003780: 6f75 7473 6964 6520 6669 7474 696e 6720  outside fitting 
-00003790: 6c69 6d69 7473 2e20 6662 203e 2075 7070  limits. fb > upp
-000037a0: 6572 5f6c 696d 6974 2062 6574 7765 656e  er_limit between
-000037b0: 2025 2e31 6520 3c3d 204d 5f68 616c 6f20   %.1e <= M_halo 
-000037c0: 5b4d 5f73 756e 5d20 3c3d 2025 2e31 652e  [M_sun] <= %.1e.
-000037d0: 2073 7570 5f6d 6f64 656c 2829 2077 696c   sup_model() wil
-000037e0: 6c20 7265 7475 726e 204e 614e 7320 7769  l return NaNs wi
-000037f0: 7468 696e 2074 686f 7365 206c 696d 6974  thin those limit
-00003800: 732e 201b 5b30 6d5a 0c73 7461 745f 6572  s. .[0mZ.stat_er
-00003810: 726f 7273 5f7a 042e 6373 767a 0575 7466  rors_z..csvz.utf
-00003820: 2d38 fa01 2c72 0400 0000 2902 da09 6465  -8..,r....)...de
-00003830: 6c69 6d69 7465 72da 0873 6b69 7072 6f77  limiter..skiprow
-00003840: 73e9 0400 0000 2901 5a07 7265 7363 616c  s.....).Z.rescal
-00003850: 65e9 0500 0000 e907 0000 0029 2372 2700  e..........)#r'.
-00003860: 0000 7228 0000 0072 2900 0000 7240 0000  ..r(...r)...r@..
-00003870: 0072 2a00 0000 720a 0000 00da 0572 6f75  .r*...r......rou
-00003880: 6e64 da08 6c6f 6773 7061 6365 723a 0000  nd..logspacer:..
-00003890: 0072 1f00 0000 da05 7072 696e 7472 1300  .r......printr..
-000038a0: 0000 7237 0000 00da 0b65 7874 7261 706f  ..r7.....extrapo
-000038b0: 6c61 7465 7243 0000 0072 3d00 0000 da03  laterC...r=.....
-000038c0: 616e 79da 036d 696e 7226 0000 00da 0a6c  any..minr&.....l
-000038d0: 6f67 6963 616c 5f6f 7272 3100 0000 7235  ogical_orr1...r5
-000038e0: 0000 0072 3600 0000 7230 0000 00da 034e  ...r6...r0.....N
-000038f0: 414e da08 5f70 6b67 7574 696c da08 6765  AN.._pkgutil..ge
-00003900: 745f 6461 7461 da08 5f5f 6e61 6d65 5f5f  t_data..__name__
-00003910: 7239 0000 00da 0664 6563 6f64 65da 0a73  r9.....decode..s
-00003920: 706c 6974 6c69 6e65 73da 076c 6f61 6474  plitlines..loadt
-00003930: 7874 da15 5f4c 696e 6561 724e 4449 6e74  xt.._LinearNDInt
-00003940: 6572 706f 6c61 746f 72da 0966 756c 6c5f  erpolator..full_
-00003950: 6c69 6b65 da0c 636f 6c75 6d6e 5f73 7461  like..column_sta
-00003960: 636b 292f 722b 0000 0072 2c00 0000 720d  ck)/r+...r,...r.
-00003970: 0000 0072 0e00 0000 720f 0000 005a 064d  ...r....r....Z.M
-00003980: 5f68 616c 6f72 1000 0000 7259 0000 0072  _halor....rY...r
-00003990: 1900 0000 721a 0000 0072 1b00 0000 7241  ....r....r....rA
-000039a0: 0000 00da 056b 5f6d 696e 722d 0000 00da  .....k_minr-....
-000039b0: 016e da06 6572 726f 7273 da07 7665 7262  .n..errors..verb
-000039c0: 6f73 6572 1d00 0000 721c 0000 00da 046c  oser....r......l
-000039d0: 6f67 6bda 0962 6573 745f 6d61 7373 da03  ogk..best_mass..
-000039e0: 665f 625a 0866 625f 696e 7465 7272 3b00  f_bZ.fb_interr;.
-000039f0: 0000 723c 0000 00da 076f 7574 5f6d 696e  ..r<.....out_min
-00003a00: da07 6f75 745f 6d61 78da 0c6d 6173 735f  ..out_max..mass_
-00003a10: 6f75 745f 6d69 6eda 0c6d 6173 735f 6f75  out_min..mass_ou
-00003a20: 745f 6d61 78da 046d 6173 6bda 0278 30da  t_max..mask..x0.
-00003a30: 0278 31da 0278 3272 4600 0000 5a09 7261  .x1..x2rF...Z.ra
-00003a40: 775f 7461 626c 65da 0574 6162 6c65 da06  w_table..table..
-00003a50: 636f 6f72 6473 5a0b 696e 7465 7270 5f36  coordsZ.interp_6
-00003a60: 385f 6d5a 0b69 6e74 6572 705f 3638 5f70  8_mZ.interp_68_p
-00003a70: 5a0b 696e 7465 7270 5f39 355f 6d5a 0b69  Z.interp_95_mZ.i
-00003a80: 6e74 6572 705f 3935 5f70 5a07 7a5f 6172  nterp_95_pZ.z_ar
-00003a90: 7261 79da 0464 6174 615a 0a65 7272 6f72  ray..dataZ.error
-00003aa0: 5f36 385f 6d5a 0a65 7272 6f72 5f36 385f  _68_mZ.error_68_
-00003ab0: 705a 0a65 7272 6f72 5f39 355f 6d5a 0a65  pZ.error_95_mZ.e
-00003ac0: 7272 6f72 5f39 355f 7072 1100 0000 7211  rror_95_pr....r.
-00003ad0: 0000 0072 1200 0000 da09 7375 705f 6d6f  ...r......sup_mo
-00003ae0: 6465 6c29 0100 0073 be00 0000 0049 0801  del)...s.....I..
-00003af0: 0a02 0801 0601 02ff 0203 0801 0601 02ff  ................
-00003b00: 0603 0801 0601 02ff 0203 0801 0601 02ff  ................
-00003b10: 0603 0801 0601 0a02 0a01 2201 0a02 0a02  ..........".....
-00003b20: 1201 0401 0401 06ff 0602 0201 1601 0601  ................
-00003b30: 0601 02ff 0a02 1401 0601 0c01 0201 1601  ................
-00003b40: 0601 0601 1001 0601 1004 0601 0401 02ff  ................
-00003b50: 0602 0201 1a01 0601 0601 02ff 0803 1402  ................
-00003b60: 0801 0802 0802 0a01 0603 16fd 0203 02fd  ................
-00003b70: 0605 0802 0a01 0603 16fd 0203 02fd 0605  ................
-00003b80: 0c02 0a01 0a01 0a02 1c02 0a02 0601 2201  ..............".
-00003b90: 1001 1601 1a01 1a01 1a01 1a02 0c01 1001  ................
-00003ba0: 0801 0801 0801 0802 1003 7279 0000 0063  ..........ry...c
-00003bb0: 0500 0000 0000 0000 0000 0000 1500 0000  ................
-00003bc0: 0600 0000 4300 0000 73e2 0100 007c 0364  ....C...s....|.d
-00003bd0: 016b 0072 1274 0064 0283 0164 0382 027c  .k.r.t.d...d...|
-00003be0: 0364 046b 0472 2474 0064 0583 0164 0382  .d.k.r$t.d...d..
-00003bf0: 027c 0364 066b 0072 3a74 016a 0264 0764  .|.d.k.r:t.j.d.d
-00003c00: 0864 098d 0201 007c 01a0 03a1 007d 057c  .d.....|.....}.|
-00003c10: 01a0 04a1 007d 067c 0564 0a6b 0472 8474  .....}.|.d.k.r.t
-00003c20: 016a 0264 0b64 0864 098d 0201 007c 0174  .j.d.d.d.....|.t
-00003c30: 05a0 067c 0164 0a6b 01a1 0119 007d 017c  ...|.d.k.....}.|
-00003c40: 0274 05a0 067c 0164 0a6b 01a1 0119 007d  .t...|.d.k.....}
-00003c50: 027c 0564 0c6b 0472 9a74 016a 0264 0d64  .|.d.k.r.t.j.d.d
-00003c60: 0864 098d 0201 0074 077c 007c 0383 027d  .d.....t.|.|...}
-00003c70: 0774 08a0 097c 01a1 017d 0874 0a7c 017c  .t...|...}.t.|.|
-00003c80: 0783 027d 0974 0b7c 007c 0364 0e7c 0913  ...}.t.|.|.d.|..
-00003c90: 0083 035c 027d 0a7d 0b74 0c7c 087c 0783  ...\.}.}.t.|.|..
-00003ca0: 027d 0c74 0d7c 087c 0783 027d 0d74 0e7c  .}.t.|.|...}.t.|
-00003cb0: 087c 0783 027d 0e64 0f7c 0e1b 000b 0074  .|...}.d.|.....t
-00003cc0: 08a0 0f7c 0c7c 0218 007c 0c7c 0d18 001b  ...|.|...|.|....
-00003cd0: 00a1 0114 007d 0f7c 0f7c 0a6b 007d 1074  .....}.|.|.k.}.t
-00003ce0: 107c 1083 0101 0074 107c 0983 0101 007c  .|.....t.|.....|
-00003cf0: 0f7c 0b6b 047d 117c 097c 1019 007d 1274  .|.k.}.|.|...}.t
-00003d00: 117c 1083 0190 0172 6274 016a 0264 1064  .|.....rbt.j.d.d
-00003d10: 0e7c 12a0 04a1 0013 0064 0e7c 12a0 03a1  .|.......d.|....
-00003d20: 0013 0066 0216 0064 0864 098d 0201 007c  ...f...d.d.....|
-00003d30: 097c 1119 007d 1374 117c 1183 0190 0172  .|...}.t.|.....r
-00003d40: 9a74 016a 0264 1164 0e7c 13a0 04a1 0013  .t.j.d.d.|......
-00003d50: 0064 0e7c 13a0 03a1 0013 0066 0216 0064  .d.|.......f...d
-00003d60: 0864 098d 0201 0074 08a0 127c 107c 11a1  .d.....t...|.|..
-00003d70: 027d 1474 086a 137c 0f7c 143c 007c 0490  .}.t.j.|.|.<.|..
-00003d80: 0172 ce74 1064 1283 0101 0074 08a0 1464  .r.t.d.....t...d
-00003d90: 0e7c 09a1 027c 0f66 0253 0074 08a0 1464  .|...|.f.S.t...d
-00003da0: 0e7c 09a1 027c 0f66 0253 0064 0353 0029  .|...|.f.S.d.S.)
-00003db0: 1375 2a07 0000 0a20 2020 2052 6574 7572  .u*....    Retur
-00003dc0: 6e73 2062 6172 796f 6e20 6672 6163 7469  ns baryon fracti
-00003dd0: 6f6e 202d 2068 616c 6f20 6d61 7373 2072  on - halo mass r
-00003de0: 656c 6174 696f 6e20 6672 6f6d 2074 6865  elation from the
-00003df0: 2073 7570 7072 6573 7369 6f6e 206f 6620   suppression of 
-00003e00: 7468 6520 746f 7461 6c20 6d61 7474 6572  the total matter
-00003e10: 2070 6f77 6572 2073 7065 6374 7275 6d20   power spectrum 
-00003e20: 0a20 2020 2075 7369 6e67 2074 6865 2053  .    using the S
-00003e30: 5028 6b29 206d 6f64 656c 2e20 4175 746f  P(k) model. Auto
-00003e40: 6d61 7469 6361 6c6c 7920 7365 6c65 6374  matically select
-00003e50: 7320 7468 6520 7265 7175 6972 6564 206f  s the required o
-00003e60: 7074 696d 616c 206d 6173 7320 6173 2061  ptimal mass as a
-00003e70: 2066 756e 6374 696f 6e20 6f66 2073 6361   function of sca
-00003e80: 6c65 2061 6e64 2072 6564 7368 6966 742e  le and redshift.
-00003e90: 200a 0a20 2020 2050 6172 616d 6574 6572   ..    Parameter
-00003ea0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00003eb0: 0a0a 2020 2020 534f 203a 2069 6e74 0a20  ..    SO : int. 
-00003ec0: 2020 2020 2020 2073 7068 6572 6963 616c         spherical
-00003ed0: 206f 7665 722d 6465 6e73 6974 792e 204f   over-density. O
-00003ee0: 6e6c 7920 6163 6365 7074 7320 3230 3020  nly accepts 200 
-00003ef0: 6f72 2035 3030 0a20 2020 206b 3a20 6172  or 500.    k: ar
-00003f00: 7261 7920 6f66 2066 6c6f 6174 0a20 2020  ray of float.   
-00003f10: 2020 2020 2061 7272 6179 2077 6974 6820       array with 
-00003f20: 7468 6520 636f 2d6d 6f76 696e 6720 7761  the co-moving wa
-00003f30: 7665 6e75 6d62 6572 2069 6e20 756e 6974  venumber in unit
-00003f40: 7320 5b68 2f4d 7063 5d0a 2020 2020 7375  s [h/Mpc].    su
-00003f50: 703a 2061 7272 6179 206f 6620 666c 6f61  p: array of floa
-00003f60: 740a 2020 2020 2020 2020 6172 7261 7920  t.        array 
-00003f70: 7769 7468 2074 6865 2073 7570 7072 6573  with the suppres
-00003f80: 7369 6f6e 206f 6620 7468 6520 746f 7461  sion of the tota
-00003f90: 6c20 6d61 7474 6572 2070 6f77 6572 2073  l matter power s
-00003fa0: 7065 6374 7275 6d20 6173 2061 2066 756e  pectrum as a fun
-00003fb0: 6374 696f 6e20 6f66 2073 6361 6c65 0a20  ction of scale. 
-00003fc0: 2020 207a 203a 2066 6c6f 6174 0a20 2020     z : float.   
-00003fd0: 2020 2020 2072 6564 7368 6966 7420 7a2e       redshift z.
-00003fe0: 204f 6e6c 7920 6163 6365 7074 7320 7661   Only accepts va
-00003ff0: 6c75 6573 206f 6620 7a20 3c3d 2033 0a20  lues of z <= 3. 
-00004000: 2020 2065 7272 6f72 7320 3a20 626f 6f6c     errors : bool
-00004010: 6561 6e2c 2064 6566 6175 6c74 2046 616c  ean, default Fal
-00004020: 7365 0a20 2020 2020 2020 2065 6e61 626c  se.        enabl
-00004030: 6573 2061 6464 6974 696f 6e61 6c20 6f75  es additional ou
-00004040: 7470 7574 2077 6974 6820 7468 6520 626f  tput with the bo
-00004050: 6f74 7374 7261 7070 6564 2036 3825 2061  otstrapped 68% a
-00004060: 6e64 2039 3525 2063 6f6e 6669 6465 6e63  nd 95% confidenc
-00004070: 6520 696e 7465 7276 616c 7320 6672 6f6d  e intervals from
-00004080: 2073 7461 7469 7374 6963 616c 2065 7272   statistical err
-00004090: 6f72 732e 0a20 2020 2020 2020 200a 2020  ors..        .  
-000040a0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000040b0: 2d2d 2d2d 2d0a 2020 2020 4d5f 6861 6c6f  -----.    M_halo
-000040c0: 203a 2061 7272 6179 206f 6620 666c 6f61   : array of floa
-000040d0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
-000040e0: 2020 2020 6172 7261 7920 636f 6e74 6169      array contai
-000040f0: 6e69 6e67 2074 6865 2028 6269 6e6e 6564  ning the (binned
-00004100: 2920 6861 6c6f 206d 6173 7320 666f 7220  ) halo mass for 
-00004110: 7468 6520 6662 202d 204d 2d68 616c 6f20  the fb - M-halo 
-00004120: 7265 6c61 7469 6f6e 2069 6e20 4d5f 7375  relation in M_su
-00004130: 6e20 756e 6974 732e 0a20 2020 2066 6220  n units..    fb 
-00004140: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
-00004150: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00004160: 2020 2061 7272 6179 2063 6f6e 7461 696e     array contain
-00004170: 696e 6720 7468 6520 2862 696e 6e65 6429  ing the (binned)
-00004180: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
-00004190: 206e 6f72 6d61 6c69 7365 6420 6279 2074   normalised by t
-000041a0: 6865 2075 6e69 7665 7273 616c 2062 6172  he universal bar
-000041b0: 796f 6e20 6672 6163 7469 6f6e 3a20 0a20  yon fraction: . 
-000041c0: 2020 2020 2020 2066 5f62 202f 2028 4f6d         f_b / (Om
-000041d0: 6567 615f 6220 2f20 4f6d 6567 615f 6d29  ega_b / Omega_m)
-000041e0: 2066 6f72 2074 6865 2066 6220 2d20 4d2d   for the fb - M-
-000041f0: 6861 6c6f 2072 656c 6174 696f 6e2e 0a0a  halo relation...
-00004200: 2020 2020 6572 726f 725f 3638 5f6d 203a      error_68_m :
-00004210: 2061 7272 6179 206f 6620 666c 6f61 742c   array of float,
-00004220: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00004230: 2020 6172 7261 7920 7769 7468 2074 6865    array with the
-00004240: 202d 3120 7369 676d 6120 636f 6e66 6964   -1 sigma confid
-00004250: 656e 6365 2069 6e74 6572 7661 6c20 0a20  ence interval . 
-00004260: 2020 2065 7272 6f72 5f36 385f 7020 3a20     error_68_p : 
-00004270: 6172 7261 7920 6f66 2066 6c6f 6174 2c20  array of float, 
-00004280: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00004290: 2061 7272 6179 2077 6974 6820 7468 6520   array with the 
-000042a0: 2b31 2073 6967 6d61 2063 6f6e 6669 6465  +1 sigma confide
-000042b0: 6e63 6520 696e 7465 7276 616c 200a 2020  nce interval .  
-000042c0: 2020 6572 726f 725f 3935 5f6d 203a 2061    error_95_m : a
-000042d0: 7272 6179 206f 6620 666c 6f61 742c 206f  rray of float, o
-000042e0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-000042f0: 6172 7261 7920 7769 7468 2074 6865 202d  array with the -
-00004300: 3220 7369 676d 6120 636f 6e66 6964 656e  2 sigma confiden
-00004310: 6365 2069 6e74 6572 7661 6c20 0a20 2020  ce interval .   
-00004320: 2065 7272 6f72 5f39 355f 7020 3a20 6172   error_95_p : ar
-00004330: 7261 7920 6f66 2066 6c6f 6174 2c20 6f70  ray of float, op
-00004340: 7469 6f6e 616c 0a20 2020 2020 2020 2061  tional.        a
-00004350: 7272 6179 2077 6974 6820 7468 6520 2b32  rray with the +2
-00004360: 2073 6967 6d61 2063 6f6e 6669 6465 6e63   sigma confidenc
-00004370: 6520 696e 7465 7276 616c 200a 0a20 2020  e interval ..   
-00004380: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-00004390: 2d2d 2d2d 2d0a 2020 2020 5468 6520 6d61  -----.    The ma
-000043a0: 7869 6d75 6d20 636f 2d6d 6f76 696e 6720  ximum co-moving 
-000043b0: 7761 7665 6e75 6d62 6572 2069 6e20 756e  wavenumber in un
-000043c0: 6974 7320 5b68 2f4d 7063 5d20 6973 2073  its [h/Mpc] is s
-000043d0: 6574 2074 6f20 7468 6520 4e79 7175 6973  et to the Nyquis
-000043e0: 7420 6672 6571 7565 6e63 7920 6f66 2074  t frequency of t
-000043f0: 6865 2041 6e74 696c 6c65 7320 7369 6d75  he Antilles simu
-00004400: 6c61 7469 6f6e 7320 0a20 2020 2028 7365  lations .    (se
-00004410: 6520 5361 6c63 6964 6f20 6574 2061 6c2e  e Salcido et al.
-00004420: 2032 3032 3229 2e20 416c 7468 6f75 6768   2022). Although
-00004430: 2053 5028 6b29 2077 6173 2066 6974 7465   SP(k) was fitte
-00004440: 6420 7570 2074 6f20 6b20 3d20 3132 205b  d up to k = 12 [
-00004450: 682f 4d70 635d 2c20 7765 2063 6175 7469  h/Mpc], we cauti
-00004460: 6f6e 2074 6865 2075 7365 7220 7468 6174  on the user that
-00004470: 2073 6574 7469 6e67 200a 2020 2020 f09d   setting .    ..
-00004480: 9198 203e 20f0 9d91 984e 7920 2838 205b  .. > ....Ny (8 [
-00004490: 682f 4d70 635d 2920 6d69 6768 7420 6e6f  h/Mpc]) might no
-000044a0: 7420 6265 2072 6570 7265 7365 6e74 6174  t be representat
-000044b0: 6976 6520 6f66 2074 6865 2074 7275 6520  ive of the true 
-000044c0: 756e 6365 7274 6169 6e74 6965 7320 696e  uncertainties in
-000044d0: 2074 6865 2064 6174 612e 200a 2020 2020   the data. .    
-000044e0: 7201 0000 0072 4a00 0000 4e72 4b00 0000  r....rJ...NrK...
-000044f0: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
-00004500: 1400 0000 7223 0000 0072 2000 0000 7a58  ....r#...r ...zX
-00004510: 1b5b 3931 6d70 792d 7370 6b20 7761 7320  .[91mpy-spk was 
-00004520: 6361 6c69 6272 6174 6564 2075 7020 746f  calibrated up to
-00004530: 206b 5f6d 6178 203d 2031 3220 5b68 2f4d   k_max = 12 [h/M
-00004540: 7063 5d20 5573 696e 6720 7661 6c75 6573  pc] Using values
-00004550: 206f 6620 6b20 3c3d 2031 3220 5b68 2f4d   of k <= 12 [h/M
-00004560: 7063 5d20 1b5b 306d 7221 0000 0072 2200  pc] .[0mr!...r".
-00004570: 0000 7225 0000 0072 0400 0000 7aa8 1b5b  ..r%...r....z..[
-00004580: 3931 6d46 6f75 6e64 2062 6172 796f 6e20  91mFound baryon 
-00004590: 6672 6163 7469 6f6e 2076 616c 7565 7320  fraction values 
-000045a0: 6f75 7473 6964 6520 6669 7474 696e 6720  outside fitting 
-000045b0: 6c69 6d69 7473 2e20 6662 203c 206c 6f77  limits. fb < low
-000045c0: 6572 5f6c 696d 6974 2062 6574 7765 656e  er_limit between
-000045d0: 2025 2e31 6520 3c3d 204d 5f68 616c 6f20   %.1e <= M_halo 
-000045e0: 5b4d 5f73 756e 5d20 3c3d 2025 2e31 652e  [M_sun] <= %.1e.
-000045f0: 2066 625f 6d6f 6465 6c28 2920 7769 6c6c   fb_model() will
-00004600: 2072 6574 7572 6e20 4e61 4e73 2077 6974   return NaNs wit
-00004610: 6869 6e20 7468 6f73 6520 6c69 6d69 7473  hin those limits
-00004620: 2e20 1b5b 306d 7aa8 1b5b 3931 6d46 6f75  . .[0mz..[91mFou
-00004630: 6e64 2062 6172 796f 6e20 6672 6163 7469  nd baryon fracti
-00004640: 6f6e 2076 616c 7565 7320 6f75 7473 6964  on values outsid
-00004650: 6520 6669 7474 696e 6720 6c69 6d69 7473  e fitting limits
-00004660: 2e20 6662 203e 2075 7070 6572 5f6c 696d  . fb > upper_lim
-00004670: 6974 2062 6574 7765 656e 2025 2e31 6520  it between %.1e 
-00004680: 3c3d 204d 5f68 616c 6f20 5b4d 5f73 756e  <= M_halo [M_sun
-00004690: 5d20 3c3d 2025 2e31 652e 2066 625f 6d6f  ] <= %.1e. fb_mo
-000046a0: 6465 6c28 2920 7769 6c6c 2072 6574 7572  del() will retur
-000046b0: 6e20 4e61 4e73 2077 6974 6869 6e20 7468  n NaNs within th
-000046c0: 6f73 6520 6c69 6d69 7473 2e20 1b5b 306d  ose limits. .[0m
-000046d0: 7a1a 4572 726f 7273 206e 6f74 2069 6d70  z.Errors not imp
-000046e0: 6c65 6d65 6e74 6564 2079 6574 2915 7227  lemented yet).r'
-000046f0: 0000 0072 2800 0000 7229 0000 0072 2600  ...r(...r)...r&.
-00004700: 0000 725b 0000 00da 026e 70da 0577 6865  ..r[.....np..whe
-00004710: 7265 722a 0000 0072 0a00 0000 723a 0000  rer*...r....r:..
-00004720: 0072 1f00 0000 723d 0000 0072 3100 0000  .r....r=...r1...
-00004730: 7235 0000 0072 3600 0000 da03 6c6f 6772  r5...r6.....logr
-00004740: 5800 0000 725a 0000 0072 5c00 0000 725d  X...rZ...r\...r]
-00004750: 0000 0072 0b00 0000 2915 722b 0000 0072  ...r....).r+...r
-00004760: 1c00 0000 7246 0000 0072 2c00 0000 7269  ....rF...r,...ri
-00004770: 0000 0072 2d00 0000 7267 0000 0072 1d00  ...r-...rg...r..
-00004780: 0000 726b 0000 0072 6c00 0000 723b 0000  ..rk...rl...r;..
-00004790: 0072 3c00 0000 7273 0000 0072 7400 0000  .r<...rs...rt...
-000047a0: 7275 0000 0072 6d00 0000 726e 0000 0072  ru...rm...rn...r
-000047b0: 6f00 0000 7270 0000 0072 7100 0000 7272  o...rp...rq...rr
-000047c0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-000047d0: 0000 da0a 5f5f 6662 5f6d 6f64 656c e401  ....__fb_model..
-000047e0: 0000 736c 0000 0000 2b08 010a 0208 0106  ..sl....+.......
-000047f0: 0102 ff02 0308 0106 0102 ff06 0308 0108  ................
-00004800: 0208 0106 0102 ff06 0212 0112 0208 0106  ................
-00004810: 0102 ff06 030a 010a 010a 0214 020a 010a  ................
-00004820: 010a 0220 0208 0108 0108 0108 0208 020a  ... ............
-00004830: 0106 0316 fd02 0302 fd06 0508 020a 0106  ................
-00004840: 0316 fd02 0302 fd06 050c 020a 0206 0108  ................
-00004850: 0110 1872 7d00 0000 2901 7204 0000 0029  ...r}...).r....)
-00004860: 0f4e 4e72 0400 0000 4e4e 464e 4e4e 4e72  .NNr....NNFNNNNr
-00004870: 4900 0000 7221 0000 0072 3f00 0000 4646  I...r!...r?...FF
-00004880: 2901 4629 1fda 056e 756d 7079 720a 0000  ).F)...numpyr...
-00004890: 005a 1173 6369 7079 2e69 6e74 6572 706f  .Z.scipy.interpo
-000048a0: 6c61 7465 7202 0000 0072 3700 0000 7203  later....r7...r.
-000048b0: 0000 0072 6400 0000 5a08 6669 745f 7661  ...rd...Z.fit_va
-000048c0: 6c73 7205 0000 0072 3e00 0000 7206 0000  lsr....r>...r...
-000048d0: 0072 3800 0000 da08 7761 726e 696e 6773  .r8.....warnings
-000048e0: 7228 0000 00da 0770 6b67 7574 696c 725e  r(.....pkgutilr^
-000048f0: 0000 00da 0e66 696c 7465 7277 6172 6e69  .....filterwarni
-00004900: 6e67 73da 0b55 7365 7257 6172 6e69 6e67  ngs..UserWarning
-00004910: 7213 0000 0072 1800 0000 721f 0000 0072  r....r....r....r
-00004920: 2e00 0000 7231 0000 0072 3500 0000 7236  ....r1...r5...r6
-00004930: 0000 0072 3d00 0000 722a 0000 0072 4300  ...r=...r*...rC.
-00004940: 0000 7248 0000 0072 7900 0000 727d 0000  ..rH...ry...r}..
-00004950: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
-00004960: 7212 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00004970: 0000 0073 3e00 0000 0801 0c01 0c01 0c01  ...s>...........
-00004980: 0c01 0801 0802 0e03 0a18 0814 0814 0820  ............... 
-00004990: 0814 0817 0816 0824 081c 0822 081a 0001  .......$..."....
-000049a0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000049b0: 00fe 0a7f 003c                           .....<
+00000000: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+00000010: 5f6e 700a 6672 6f6d 2073 6369 7079 2e69  _np.from scipy.i
+00000020: 6e74 6572 706f 6c61 7465 2069 6d70 6f72  nterpolate impor
+00000030: 7420 416b 696d 6131 4449 6e74 6572 706f  t Akima1DInterpo
+00000040: 6c61 746f 7220 6173 205f 416b 696d 6131  lator as _Akima1
+00000050: 4449 6e74 6572 706f 6c61 746f 720a 6672  DInterpolator.fr
+00000060: 6f6d 2073 6369 7079 2e69 6e74 6572 706f  om scipy.interpo
+00000070: 6c61 7465 2069 6d70 6f72 7420 4c69 6e65  late import Line
+00000080: 6172 4e44 496e 7465 7270 6f6c 6174 6f72  arNDInterpolator
+00000090: 2061 7320 5f4c 696e 6561 724e 4449 6e74   as _LinearNDInt
+000000a0: 6572 706f 6c61 746f 720a 6672 6f6d 202e  erpolator.from .
+000000b0: 6669 745f 7661 6c73 2069 6d70 6f72 7420  fit_vals import 
+000000c0: 6265 7374 5f66 6974 5f76 616c 7320 6173  best_fit_vals as
+000000d0: 205f 6265 7374 5f66 6974 5f76 616c 730a   _best_fit_vals.
+000000e0: 6672 6f6d 202e 6669 745f 7661 6c73 2069  from .fit_vals i
+000000f0: 6d70 6f72 7420 6c69 6d69 7473 2061 7320  mport limits as 
+00000100: 5f6c 696d 6974 730a 696d 706f 7274 2077  _limits.import w
+00000110: 6172 6e69 6e67 7320 6173 205f 7761 726e  arnings as _warn
+00000120: 696e 6773 0a69 6d70 6f72 7420 706b 6775  ings.import pkgu
+00000130: 7469 6c20 6173 205f 706b 6775 7469 6c0a  til as _pkgutil.
+00000140: 0a5f 7761 726e 696e 6773 2e66 696c 7465  ._warnings.filte
+00000150: 7277 6172 6e69 6e67 7328 2261 6c77 6179  rwarnings("alway
+00000160: 7322 2c20 6361 7465 676f 7279 3d55 7365  s", category=Use
+00000170: 7257 6172 6e69 6e67 290a 0a64 6566 205f  rWarning)..def _
+00000180: 706f 7765 725f 6c61 7728 6d5f 6861 6c6f  power_law(m_halo
+00000190: 2c20 6662 5f61 2c20 6662 5f70 6f77 2c20  , fb_a, fb_pow, 
+000001a0: 6662 5f70 6976 6f74 3d31 293a 0a20 2020  fb_pivot=1):.   
+000001b0: 2022 2222 0a20 2020 2053 696d 706c 6520   """.    Simple 
+000001c0: 706f 7765 722d 6c61 7720 6675 6e63 7469  power-law functi
+000001d0: 6f6e 2066 6974 2074 6f20 7468 6520 6261  on fit to the ba
+000001e0: 7279 6f6e 2066 7261 6374 696f 6e20 2d20  ryon fraction - 
+000001f0: 6861 6c6f 206d 6173 7320 7265 6c61 7469  halo mass relati
+00000200: 6f6e 0a0a 2020 2020 5061 7261 6d65 7465  on..    Paramete
+00000210: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00000220: 2d0a 2020 2020 6d5f 6861 6c6f 3a20 6172  -.    m_halo: ar
+00000230: 7261 7920 6f66 2066 6c6f 6174 0a20 2020  ray of float.   
+00000240: 2020 2020 2068 616c 6f20 6d61 7373 2069       halo mass i
+00000250: 6e20 4d5f 7375 6e20 756e 6974 730a 2020  n M_sun units.  
+00000260: 2020 6662 5f61 203a 2066 6c6f 6174 0a20    fb_a : float. 
+00000270: 2020 2020 2020 2070 6f77 6572 206c 6177         power law
+00000280: 2063 6f6e 7374 616e 740a 2020 2020 6662   constant.    fb
+00000290: 5f70 6f77 203a 2066 6c6f 6174 0a20 2020  _pow : float.   
+000002a0: 2020 2020 2070 6f77 6572 206c 6177 2065       power law e
+000002b0: 7870 6f6e 656e 740a 2020 2020 6662 5f70  xponent.    fb_p
+000002c0: 6976 6f74 203a 2066 6c6f 6174 2c20 6465  ivot : float, de
+000002d0: 6661 756c 7420 310a 2020 2020 2020 2020  fault 1.        
+000002e0: 706f 7765 7220 6c61 7720 7069 766f 7420  power law pivot 
+000002f0: 706f 696e 742e 200a 0a20 2020 2052 6574  point. ..    Ret
+00000300: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00000310: 0a20 2020 206f 7574 7075 743a 2061 7272  .    output: arr
+00000320: 6179 206f 6620 666c 6f61 740a 2020 2020  ay of float.    
+00000330: 2020 2020 6261 7279 6f6e 2066 7261 6374      baryon fract
+00000340: 696f 6e20 6e6f 726d 616c 6973 6564 2062  ion normalised b
+00000350: 7920 7468 6520 556e 6976 6572 7361 6c20  y the Universal 
+00000360: 6261 7279 6f6e 2066 7261 6374 696f 6e3a  baryon fraction:
+00000370: 2066 5f62 202f 2028 4f6d 6567 615f 6220   f_b / (Omega_b 
+00000380: 2f20 4f6d 6567 615f 6d29 0a20 2020 2022  / Omega_m).    "
+00000390: 2222 0a20 2020 2066 6220 3d20 6662 5f61  "".    fb = fb_a
+000003a0: 202a 205f 6e70 2e70 6f77 6572 286d 5f68   * _np.power(m_h
+000003b0: 616c 6f20 2f20 6662 5f70 6976 6f74 2c20  alo / fb_pivot, 
+000003c0: 6662 5f70 6f77 290a 2020 2020 7265 7475  fb_pow).    retu
+000003d0: 726e 2066 620a 0a0a 6465 6620 5f70 6f6c  rn fb...def _pol
+000003e0: 795f 3228 782c 2076 616c 7329 3a0a 2020  y_2(x, vals):.  
+000003f0: 2020 2222 220a 2020 2020 5369 6d70 6c65    """.    Simple
+00000400: 2070 6f6c 796e 6f6d 6961 6c20 6f66 206f   polynomial of o
+00000410: 7264 6572 2032 2e20 0a0a 2020 2020 5061  rder 2. ..    Pa
+00000420: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00000430: 2d2d 2d2d 2d2d 2d0a 2020 2020 7820 3a20  -------.    x : 
+00000440: 6172 7261 7920 6f66 2066 6c6f 6174 0a20  array of float. 
+00000450: 2020 2020 2020 2069 6e64 6570 656e 6465         independe
+00000460: 6e74 2076 6172 6961 626c 6520 0a20 2020  nt variable .   
+00000470: 2076 616c 7320 3a20 6172 7261 7920 6f66   vals : array of
+00000480: 2066 6c6f 6174 0a20 2020 2020 2020 2061   float.        a
+00000490: 7272 6179 2063 6f6e 7461 696e 696e 6720  rray containing 
+000004a0: 7468 6520 706f 6c79 6e6f 6d69 616c 2063  the polynomial c
+000004b0: 6f65 6666 6963 6965 6e74 730a 0a20 2020  oefficients..   
+000004c0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+000004d0: 2d2d 2d2d 0a20 2020 2079 3a20 6172 7261  ----.    y: arra
+000004e0: 7920 6f66 2066 6c6f 6174 0a20 2020 2020  y of float.     
+000004f0: 2020 2064 6570 656e 6465 6e74 2076 6172     dependent var
+00000500: 6961 626c 6520 0a20 2020 2022 2222 0a20  iable .    """. 
+00000510: 2020 2079 203d 2076 616c 735b 325d 202a     y = vals[2] *
+00000520: 205f 6e70 2e70 6f77 6572 2878 2c20 3229   _np.power(x, 2)
+00000530: 202b 2076 616c 735b 315d 202a 2078 202b   + vals[1] * x +
+00000540: 2076 616c 735b 305d 200a 2020 2020 7265   vals[0] .    re
+00000550: 7475 726e 2079 0a0a 0a64 6566 205f 6f70  turn y...def _op
+00000560: 7469 6d61 6c5f 6d61 7373 5f66 756e 6374  timal_mass_funct
+00000570: 286b 2c20 7061 7261 6d73 293a 0a20 2020  (k, params):.   
+00000580: 2022 2222 0a20 2020 204f 7074 696d 616c   """.    Optimal
+00000590: 206d 6173 7320 6675 6e63 7469 6f6e 2064   mass function d
+000005a0: 6566 696e 6564 2069 6e20 6571 2e28 3229  efined in eq.(2)
+000005b0: 2069 6e20 5361 6c63 6964 6f20 6574 2061   in Salcido et a
+000005c0: 6c2e 2028 3230 3232 292e 0a0a 2020 2020  l. (2022)...    
+000005d0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000005e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6b20  ---------.    k 
+000005f0: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
+00000600: 0a20 2020 2020 2020 2063 6f2d 6d6f 7669  .        co-movi
+00000610: 6e67 2077 6176 656e 756d 6265 7220 696e  ng wavenumber in
+00000620: 2075 6e69 7473 205b 682f 4d70 635d 0a20   units [h/Mpc]. 
+00000630: 2020 2070 7261 6d73 203a 2064 6963 740a     prams : dict.
+00000640: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
+00000650: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
+00000660: 6520 6265 7374 2066 6974 7469 6e67 2070  e best fitting p
+00000670: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
+00000680: 2053 5028 6b29 206d 6f64 656c 2061 7420   SP(k) model at 
+00000690: 6120 7370 6563 6966 6963 2072 6564 7368  a specific redsh
+000006a0: 6966 742e 200a 0a20 2020 2052 6574 7572  ift. ..    Retur
+000006b0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+000006c0: 2020 206f 7574 7075 743a 2061 7272 6179     output: array
+000006d0: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
+000006e0: 2020 6c6f 675f 3130 206f 6620 7468 6520    log_10 of the 
+000006f0: 6f70 7469 6d61 6c20 6d61 7373 2069 6e20  optimal mass in 
+00000700: 4d5f 7375 6e20 756e 6974 730a 2020 2020  M_sun units.    
+00000710: 2222 220a 2020 2020 6f75 7470 7574 203d  """.    output =
+00000720: 2070 6172 616d 735b 2761 6c70 6861 275d   params['alpha']
+00000730: 202d 2028 7061 7261 6d73 5b27 616c 7068   - (params['alph
+00000740: 6127 5d20 2d20 7061 7261 6d73 5b27 6265  a'] - params['be
+00000750: 7461 275d 2920 2a20 5f6e 702e 706f 7765  ta']) * _np.powe
+00000760: 7228 6b2c 2070 6172 616d 735b 2767 616d  r(k, params['gam
+00000770: 6d61 275d 290a 2020 2020 7265 7475 726e  ma']).    return
+00000780: 206f 7574 7075 740a 0a0a 6465 6620 6f70   output...def op
+00000790: 7469 6d61 6c5f 6d61 7373 2853 4f2c 207a  timal_mass(SO, z
+000007a0: 2c20 6b2c 2076 6572 626f 7365 3d46 616c  , k, verbose=Fal
+000007b0: 7365 293a 0a20 2020 2022 2222 0a20 2020  se):.    """.   
+000007c0: 204f 7074 696d 616c 206d 6173 7320 6675   Optimal mass fu
+000007d0: 6e63 7469 6f6e 2061 7320 6120 6675 6e63  nction as a func
+000007e0: 7469 6f6e 206f 6620 7363 616c 6520 616e  tion of scale an
+000007f0: 6420 7265 6473 6869 6674 2066 6f72 2061  d redshift for a
+00000800: 2073 7065 6369 6669 6320 0a20 2020 2073   specific .    s
+00000810: 7068 6572 6963 616c 206f 7665 722d 6465  pherical over-de
+00000820: 6e73 6974 792e 2044 6566 696e 6564 2069  nsity. Defined i
+00000830: 6e20 6571 2e28 3229 2069 6e20 5361 6c63  n eq.(2) in Salc
+00000840: 6964 6f20 6574 2061 6c2e 2028 3230 3232  ido et al. (2022
+00000850: 292e 0a0a 2020 2020 5061 7261 6d65 7465  )...    Paramete
+00000860: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00000870: 2d0a 2020 2020 534f 203a 2069 6e74 0a20  -.    SO : int. 
+00000880: 2020 2020 2020 2073 7068 6572 6963 616c         spherical
+00000890: 206f 7665 722d 6465 6e73 6974 792e 204f   over-density. O
+000008a0: 6e6c 7920 6163 6365 7074 7320 3230 3020  nly accepts 200 
+000008b0: 6f72 2035 3030 0a20 2020 207a 203a 2066  or 500.    z : f
+000008c0: 6c6f 6174 0a20 2020 2020 2020 2072 6564  loat.        red
+000008d0: 7368 6966 7420 7a2e 204f 6e6c 7920 6163  shift z. Only ac
+000008e0: 6365 7074 7320 7661 6c75 6573 206f 6620  cepts values of 
+000008f0: 7a20 3c3d 2033 0a20 2020 206b 203a 2061  z <= 3.    k : a
+00000900: 7272 6179 206f 6620 666c 6f61 740a 2020  rray of float.  
+00000910: 2020 2020 2020 636f 2d6d 6f76 696e 6720        co-moving 
+00000920: 7761 7665 6e75 6d62 6572 2069 6e20 756e  wavenumber in un
+00000930: 6974 7320 5b68 2f4d 7063 5d0a 2020 2020  its [h/Mpc].    
+00000940: 7665 7262 6f73 6520 3a20 626f 6f6c 6561  verbose : boolea
+00000950: 6e2c 2064 6566 6175 6c74 2054 7275 650a  n, default True.
+00000960: 2020 2020 2020 2020 5275 6e20 696e 2076          Run in v
+00000970: 6572 626f 7365 206d 6f64 650a 0a20 2020  erbose mode..   
+00000980: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00000990: 2d2d 2d2d 0a20 2020 206f 7574 7075 743a  ----.    output:
+000009a0: 2061 7272 6179 206f 6620 666c 6f61 740a   array of float.
+000009b0: 2020 2020 2020 2020 6f70 7469 6d61 6c20          optimal 
+000009c0: 6d61 7373 2069 6e20 4d5f 7375 6e20 756e  mass in M_sun un
+000009d0: 6974 730a 2020 2020 2222 220a 2020 2020  its.    """.    
+000009e0: 6b5f 6d61 7820 3d20 5f6e 702e 6d61 7828  k_max = _np.max(
+000009f0: 6b29 0a20 2020 2069 6620 6b5f 6d61 7820  k).    if k_max 
+00000a00: 3e20 3132 3a0a 2020 2020 2020 2020 7261  > 12:.        ra
+00000a10: 6973 6520 4578 6365 7074 696f 6e28 275c  ise Exception('\
+00000a20: 3033 335b 3931 6d70 792d 7370 6b20 7761  033[91mpy-spk wa
+00000a30: 7320 6361 6c69 6272 6174 6564 2075 7020  s calibrated up 
+00000a40: 746f 206b 5f6d 6178 203d 2031 3220 5b68  to k_max = 12 [h
+00000a50: 2f4d 7063 5d20 270a 2020 2020 2020 2020  /Mpc] '.        
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2750 6c65 6173 6520 7370 6563 6966 7920  'Please specify 
+00000a80: 7661 6c75 6573 206f 6620 6b20 3c3d 2031  values of k <= 1
+00000a90: 3220 5b68 2f4d 7063 5d20 5c30 3333 5b30  2 [h/Mpc] \033[0
+00000aa0: 6d27 290a 2020 2020 6966 206b 5f6d 6178  m').    if k_max
+00000ab0: 203e 2038 3a0a 2020 2020 2020 2020 5f77   > 8:.        _w
+00000ac0: 6172 6e69 6e67 732e 7761 726e 2827 5c30  arnings.warn('\0
+00000ad0: 3333 5b33 336d 5363 616c 6573 2077 6974  33[33mScales wit
+00000ae0: 6820 6b5f 6d61 7820 3e20 6b5f 6e79 203d  h k_max > k_ny =
+00000af0: 2038 205b 682f 4d70 635d 2027 0a20 2020   8 [h/Mpc] '.   
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2020 2020 276d 6179 206e 6f74 2062 6520      'may not be 
+00000b20: 6163 6375 7261 7465 6c79 2072 6570 726f  accurately repro
+00000b30: 6475 6365 6420 6279 2074 6865 206d 6f64  duced by the mod
+00000b40: 656c 2e20 5c30 3333 5b30 6d27 2c20 7374  el. \033[0m', st
+00000b50: 6163 6b6c 6576 656c 3d32 290a 0a20 2020  acklevel=2)..   
+00000b60: 2070 6172 616d 7320 3d20 5f67 6574 5f70   params = _get_p
+00000b70: 6172 616d 7328 534f 2c20 7a29 0a20 2020  arams(SO, z).   
+00000b80: 206f 7574 7075 7420 3d20 7061 7261 6d73   output = params
+00000b90: 5b27 616c 7068 6127 5d20 2d20 2870 6172  ['alpha'] - (par
+00000ba0: 616d 735b 2761 6c70 6861 275d 202d 2070  ams['alpha'] - p
+00000bb0: 6172 616d 735b 2762 6574 6127 5d29 202a  arams['beta']) *
+00000bc0: 205f 6e70 2e70 6f77 6572 286b 2c20 7061   _np.power(k, pa
+00000bd0: 7261 6d73 5b27 6761 6d6d 6127 5d29 0a20  rams['gamma']). 
+00000be0: 2020 2072 6574 7572 6e20 5f6e 702e 706f     return _np.po
+00000bf0: 7765 7228 3130 2c20 6f75 7470 7574 290a  wer(10, output).
+00000c00: 0a0a 6465 6620 5f6c 616d 6264 615f 6675  ..def _lambda_fu
+00000c10: 6e63 7428 782c 2070 6172 616d 7329 3a0a  nct(x, params):.
+00000c20: 2020 2020 2222 220a 2020 2020 6c61 6d62      """.    lamb
+00000c30: 6461 2066 756e 6374 696f 6e20 666f 7220  da function for 
+00000c40: 6120 7370 6563 6966 6963 2072 6564 7368  a specific redsh
+00000c50: 6966 742e 2044 6566 696e 6564 2069 6e20  ift. Defined in 
+00000c60: 6571 2e28 3629 2069 6e20 5361 6c63 6964  eq.(6) in Salcid
+00000c70: 6f20 6574 2061 6c2e 2028 3230 3232 292e  o et al. (2022).
+00000c80: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00000c90: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000ca0: 2020 2020 6b20 3a20 6172 7261 7920 6f66      k : array of
+00000cb0: 2066 6c6f 6174 0a20 2020 2020 2020 2063   float.        c
+00000cc0: 6f2d 6d6f 7669 6e67 2077 6176 656e 756d  o-moving wavenum
+00000cd0: 6265 7220 696e 2075 6e69 7473 205b 682f  ber in units [h/
+00000ce0: 4d70 635d 0a20 2020 2070 7261 6d73 203a  Mpc].    prams :
+00000cf0: 2064 6963 740a 2020 2020 2020 2020 6469   dict.        di
+00000d00: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+00000d10: 696e 6720 7468 6520 6265 7374 2066 6974  ing the best fit
+00000d20: 7469 6e67 2070 6172 616d 6574 6572 7320  ting parameters 
+00000d30: 6f66 2074 6865 2053 5028 6b29 206d 6f64  of the SP(k) mod
+00000d40: 656c 2061 7420 6120 7370 6563 6966 6963  el at a specific
+00000d50: 2072 6564 7368 6966 742e 200a 0a20 2020   redshift. ..   
+00000d60: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00000d70: 2d2d 2d2d 0a20 2020 206f 7574 7075 743a  ----.    output:
+00000d80: 2061 7272 6179 206f 6620 666c 6f61 740a   array of float.
+00000d90: 2020 2020 2020 2020 6c61 6d62 6461 0a20          lambda. 
+00000da0: 2020 2022 2222 0a20 2020 206f 7574 7075     """.    outpu
+00000db0: 7420 3d20 3120 2b20 7061 7261 6d73 5b27  t = 1 + params['
+00000dc0: 6c61 6d62 6461 5f61 275d 202a 205f 6e70  lambda_a'] * _np
+00000dd0: 2e65 7870 2870 6172 616d 735b 276c 616d  .exp(params['lam
+00000de0: 6264 615f 6227 5d20 2a20 7829 0a20 2020  bda_b'] * x).   
+00000df0: 2072 6574 7572 6e20 6f75 7470 7574 0a0a   return output..
+00000e00: 0a64 6566 205f 6d75 5f66 756e 6374 2878  .def _mu_funct(x
+00000e10: 2c20 7061 7261 6d73 293a 0a20 2020 2022  , params):.    "
+00000e20: 2222 0a20 2020 206d 7520 6675 6e63 7469  "".    mu functi
+00000e30: 6f6e 2066 6f72 2061 2073 7065 6369 6669  on for a specifi
+00000e40: 6320 7265 6473 6869 6674 2e20 4465 6669  c redshift. Defi
+00000e50: 6e65 6420 696e 2065 712e 2837 2920 696e  ned in eq.(7) in
+00000e60: 2053 616c 6369 646f 2065 7420 616c 2e20   Salcido et al. 
+00000e70: 2832 3032 3229 2e0a 0a20 2020 2050 6172  (2022)...    Par
+00000e80: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00000e90: 2d2d 2d2d 2d2d 0a20 2020 206b 203a 2061  ------.    k : a
+00000ea0: 7272 6179 206f 6620 666c 6f61 740a 2020  rray of float.  
+00000eb0: 2020 2020 2020 636f 2d6d 6f76 696e 6720        co-moving 
+00000ec0: 7761 7665 6e75 6d62 6572 2069 6e20 756e  wavenumber in un
+00000ed0: 6974 7320 5b68 2f4d 7063 5d0a 2020 2020  its [h/Mpc].    
+00000ee0: 7072 616d 7320 3a20 6469 6374 0a20 2020  prams : dict.   
+00000ef0: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
+00000f00: 636f 6e74 6169 6e69 6e67 2074 6865 2062  containing the b
+00000f10: 6573 7420 6669 7474 696e 6720 7061 7261  est fitting para
+00000f20: 6d65 7465 7273 206f 6620 7468 6520 5350  meters of the SP
+00000f30: 286b 2920 6d6f 6465 6c20 6174 2061 2073  (k) model at a s
+00000f40: 7065 6369 6669 6320 7265 6473 6869 6674  pecific redshift
+00000f50: 2e20 0a0a 2020 2020 5265 7475 726e 730a  . ..    Returns.
+00000f60: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000f70: 6f75 7470 7574 3a20 6172 7261 7920 6f66  output: array of
+00000f80: 2066 6c6f 6174 0a20 2020 2020 2020 206d   float.        m
+00000f90: 750a 2020 2020 2222 220a 2020 2020 4120  u.    """.    A 
+00000fa0: 3d20 7061 7261 6d73 5b27 6d75 5f61 275d  = params['mu_a']
+00000fb0: 0a20 2020 2042 203d 2031 202d 2070 6172  .    B = 1 - par
+00000fc0: 616d 735b 276d 755f 6127 5d0a 2020 2020  ams['mu_a'].    
+00000fd0: 4320 3d20 3120 2b20 5f6e 702e 6578 7028  C = 1 + _np.exp(
+00000fe0: 7061 7261 6d73 5b27 6d75 5f62 275d 202a  params['mu_b'] *
+00000ff0: 2078 202b 2070 6172 616d 735b 276d 755f   x + params['mu_
+00001000: 6327 5d29 0a20 2020 206f 7574 7075 7420  c']).    output 
+00001010: 3d20 4120 2b20 2842 202f 2043 290a 2020  = A + (B / C).  
+00001020: 2020 7265 7475 726e 206f 7574 7075 740a    return output.
+00001030: 0a0a 6465 6620 5f6e 755f 6675 6e63 2878  ..def _nu_func(x
+00001040: 2c20 7061 7261 6d73 293a 0a20 2020 2022  , params):.    "
+00001050: 2222 0a20 2020 206e 7520 6675 6e63 7469  "".    nu functi
+00001060: 6f6e 2066 6f72 2061 2073 7065 6369 6669  on for a specifi
+00001070: 6320 7265 6473 6869 6674 2e20 4465 6669  c redshift. Defi
+00001080: 6e65 6420 696e 2065 712e 2838 2920 696e  ned in eq.(8) in
+00001090: 2053 616c 6369 646f 2065 7420 616c 2e20   Salcido et al. 
+000010a0: 2832 3032 3229 2e0a 0a20 2020 2050 6172  (2022)...    Par
+000010b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000010c0: 2d2d 2d2d 2d2d 0a20 2020 206b 203a 2061  ------.    k : a
+000010d0: 7272 6179 206f 6620 666c 6f61 740a 2020  rray of float.  
+000010e0: 2020 2020 2020 636f 2d6d 6f76 696e 6720        co-moving 
+000010f0: 7761 7665 6e75 6d62 6572 2069 6e20 756e  wavenumber in un
+00001100: 6974 7320 5b68 2f4d 7063 5d0a 2020 2020  its [h/Mpc].    
+00001110: 7072 616d 7320 3a20 6469 6374 0a20 2020  prams : dict.   
+00001120: 2020 2020 2064 6963 7469 6f6e 6172 7920       dictionary 
+00001130: 636f 6e74 6169 6e69 6e67 2074 6865 2062  containing the b
+00001140: 6573 7420 6669 7474 696e 6720 7061 7261  est fitting para
+00001150: 6d65 7465 7273 206f 6620 7468 6520 5350  meters of the SP
+00001160: 286b 2920 6d6f 6465 6c20 6174 2061 2073  (k) model at a s
+00001170: 7065 6369 6669 6320 7265 6473 6869 6674  pecific redshift
+00001180: 2e20 0a0a 2020 2020 5265 7475 726e 730a  . ..    Returns.
+00001190: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000011a0: 6f75 7470 7574 3a20 6172 7261 7920 6f66  output: array of
+000011b0: 2066 6c6f 6174 0a20 2020 2020 2020 206e   float.        n
+000011c0: 750a 2020 2020 2222 220a 2020 2020 4120  u.    """.    A 
+000011d0: 3d20 7061 7261 6d73 5b27 6e75 5f61 275d  = params['nu_a']
+000011e0: 0a20 2020 2042 203d 205f 6e70 2e65 7870  .    B = _np.exp
+000011f0: 282d 2e35 202a 2028 2878 202d 2070 6172  (-.5 * ((x - par
+00001200: 616d 735b 276e 755f 6227 5d29 202f 2070  ams['nu_b']) / p
+00001210: 6172 616d 735b 276e 755f 6327 5d29 202a  arams['nu_c']) *
+00001220: 2a20 3229 0a20 2020 206f 7574 7075 7420  * 2).    output 
+00001230: 3d20 4120 2a20 420a 2020 2020 7265 7475  = A * B.    retu
+00001240: 726e 206f 7574 7075 740a 0a0a 6465 6620  rn output...def 
+00001250: 6765 745f 6c69 6d69 7473 2853 4f2c 207a  get_limits(SO, z
+00001260: 2c20 6d5f 6861 6c6f 293a 0a20 2020 2022  , m_halo):.    "
+00001270: 2222 0a20 2020 2046 756e 6374 696f 6e20  "".    Function 
+00001280: 7468 6174 2072 6574 7572 6e73 2074 6865  that returns the
+00001290: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
+000012a0: 2066 6974 7469 6e67 206c 696d 6974 7320   fitting limits 
+000012b0: 6173 2061 2066 756e 6374 696f 6e20 6f66  as a function of
+000012c0: 2068 616c 6f20 6d61 7373 0a20 2020 2061   halo mass.    a
+000012d0: 6e64 2072 6564 7368 6966 742e 0a0a 2020  nd redshift...  
+000012e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000012f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00001300: 534f 203a 2069 6e74 0a20 2020 2020 2020  SO : int.       
+00001310: 2073 7068 6572 6963 616c 206f 7665 722d   spherical over-
+00001320: 6465 6e73 6974 792e 204f 6e6c 7920 6163  density. Only ac
+00001330: 6365 7074 7320 3230 3020 6f72 2035 3030  cepts 200 or 500
+00001340: 0a20 2020 207a 203a 2066 6c6f 6174 0a20  .    z : float. 
+00001350: 2020 2020 2020 2072 6564 7368 6966 7420         redshift 
+00001360: 7a2e 204f 6e6c 7920 6163 6365 7074 7320  z. Only accepts 
+00001370: 7661 6c75 6573 206f 6620 7a20 3c3d 2033  values of z <= 3
+00001380: 0a20 2020 206d 5f68 616c 6f3a 2061 7272  .    m_halo: arr
+00001390: 6179 206f 6620 666c 6f61 740a 2020 2020  ay of float.    
+000013a0: 2020 2020 6861 6c6f 206d 6173 7320 696e      halo mass in
+000013b0: 204d 5f73 756e 2075 6e69 7473 0a0a 2020   M_sun units..  
+000013c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000013d0: 2d2d 2d2d 2d0a 2020 2020 6d69 6e5f 6662  -----.    min_fb
+000013e0: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
+000013f0: 0a20 2020 2020 2020 206c 6f77 6572 2066  .        lower f
+00001400: 6974 7469 6e67 206c 696d 6974 2066 6f72  itting limit for
+00001410: 2074 6865 2062 6172 796f 6e20 6672 6163   the baryon frac
+00001420: 7469 6f6e 206e 6f72 6d61 6c69 7365 6420  tion normalised 
+00001430: 6279 2074 6865 2075 6e69 7665 7273 616c  by the universal
+00001440: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
+00001450: 0a20 2020 206d 6178 5f66 623a 2061 7272  .    max_fb: arr
+00001460: 6179 206f 6620 666c 6f61 740a 2020 2020  ay of float.    
+00001470: 2020 2020 7570 7065 7220 6669 7474 696e      upper fittin
+00001480: 6720 6c69 6d69 7420 666f 7220 7468 6520  g limit for the 
+00001490: 6261 7279 6f6e 2066 7261 6374 696f 6e20  baryon fraction 
+000014a0: 6e6f 726d 616c 6973 6564 2062 7920 7468  normalised by th
+000014b0: 6520 756e 6976 6572 7361 6c20 6261 7279  e universal bary
+000014c0: 6f6e 2066 7261 6374 696f 6e0a 2020 2020  on fraction.    
+000014d0: 2222 220a 0a20 2020 2069 6e74 6572 5f6d  """..    inter_m
+000014e0: 696e 5f78 3020 3d20 5f41 6b69 6d61 3144  in_x0 = _Akima1D
+000014f0: 496e 7465 7270 6f6c 6174 6f72 285f 6c69  Interpolator(_li
+00001500: 6d69 7473 5b73 7472 2853 4f29 5d5b 277a  mits[str(SO)]['z
+00001510: 275d 2c20 5f6c 696d 6974 735b 7374 7228  '], _limits[str(
+00001520: 534f 295d 5b27 6d69 6e5f 7830 275d 290a  SO)]['min_x0']).
+00001530: 2020 2020 696e 7465 725f 6d69 6e5f 7831      inter_min_x1
+00001540: 203d 205f 416b 696d 6131 4449 6e74 6572   = _Akima1DInter
+00001550: 706f 6c61 746f 7228 5f6c 696d 6974 735b  polator(_limits[
+00001560: 7374 7228 534f 295d 5b27 7a27 5d2c 205f  str(SO)]['z'], _
+00001570: 6c69 6d69 7473 5b73 7472 2853 4f29 5d5b  limits[str(SO)][
+00001580: 276d 696e 5f78 3127 5d29 0a20 2020 2069  'min_x1']).    i
+00001590: 6e74 6572 5f6d 696e 5f78 3220 3d20 5f41  nter_min_x2 = _A
+000015a0: 6b69 6d61 3144 496e 7465 7270 6f6c 6174  kima1DInterpolat
+000015b0: 6f72 285f 6c69 6d69 7473 5b73 7472 2853  or(_limits[str(S
+000015c0: 4f29 5d5b 277a 275d 2c20 5f6c 696d 6974  O)]['z'], _limit
+000015d0: 735b 7374 7228 534f 295d 5b27 6d69 6e5f  s[str(SO)]['min_
+000015e0: 7832 275d 290a 0a20 2020 2069 6e74 6572  x2'])..    inter
+000015f0: 5f6d 6178 5f78 3020 3d20 5f41 6b69 6d61  _max_x0 = _Akima
+00001600: 3144 496e 7465 7270 6f6c 6174 6f72 285f  1DInterpolator(_
+00001610: 6c69 6d69 7473 5b73 7472 2853 4f29 5d5b  limits[str(SO)][
+00001620: 277a 275d 2c20 5f6c 696d 6974 735b 7374  'z'], _limits[st
+00001630: 7228 534f 295d 5b27 6d61 785f 7830 275d  r(SO)]['max_x0']
+00001640: 290a 2020 2020 696e 7465 725f 6d61 785f  ).    inter_max_
+00001650: 7831 203d 205f 416b 696d 6131 4449 6e74  x1 = _Akima1DInt
+00001660: 6572 706f 6c61 746f 7228 5f6c 696d 6974  erpolator(_limit
+00001670: 735b 7374 7228 534f 295d 5b27 7a27 5d2c  s[str(SO)]['z'],
+00001680: 205f 6c69 6d69 7473 5b73 7472 2853 4f29   _limits[str(SO)
+00001690: 5d5b 276d 6178 5f78 3127 5d29 0a20 2020  ]['max_x1']).   
+000016a0: 2069 6e74 6572 5f6d 6178 5f78 3220 3d20   inter_max_x2 = 
+000016b0: 5f41 6b69 6d61 3144 496e 7465 7270 6f6c  _Akima1DInterpol
+000016c0: 6174 6f72 285f 6c69 6d69 7473 5b73 7472  ator(_limits[str
+000016d0: 2853 4f29 5d5b 277a 275d 2c20 5f6c 696d  (SO)]['z'], _lim
+000016e0: 6974 735b 7374 7228 534f 295d 5b27 6d61  its[str(SO)]['ma
+000016f0: 785f 7832 275d 290a 0a20 2020 206d 696e  x_x2'])..    min
+00001700: 5f66 6220 3d20 3130 202a 2a20 2869 6e74  _fb = 10 ** (int
+00001710: 6572 5f6d 696e 5f78 3028 7a29 202b 2069  er_min_x0(z) + i
+00001720: 6e74 6572 5f6d 696e 5f78 3128 7a29 202a  nter_min_x1(z) *
+00001730: 205f 6e70 2e6c 6f67 3130 286d 5f68 616c   _np.log10(m_hal
+00001740: 6f29 202b 2069 6e74 6572 5f6d 696e 5f78  o) + inter_min_x
+00001750: 3228 7a29 202a 205f 6e70 2e6c 6f67 3130  2(z) * _np.log10
+00001760: 286d 5f68 616c 6f29 202a 2a20 3229 0a20  (m_halo) ** 2). 
+00001770: 2020 206d 6178 5f66 6220 3d20 3130 202a     max_fb = 10 *
+00001780: 2a20 2869 6e74 6572 5f6d 6178 5f78 3028  * (inter_max_x0(
+00001790: 7a29 202b 2069 6e74 6572 5f6d 6178 5f78  z) + inter_max_x
+000017a0: 3128 7a29 202a 205f 6e70 2e6c 6f67 3130  1(z) * _np.log10
+000017b0: 286d 5f68 616c 6f29 202b 2069 6e74 6572  (m_halo) + inter
+000017c0: 5f6d 6178 5f78 3228 7a29 202a 205f 6e70  _max_x2(z) * _np
+000017d0: 2e6c 6f67 3130 286d 5f68 616c 6f29 202a  .log10(m_halo) *
+000017e0: 2a20 3229 0a0a 2020 2020 7265 7475 726e  * 2)..    return
+000017f0: 206d 696e 5f66 622c 206d 6178 5f66 620a   min_fb, max_fb.
+00001800: 0a0a 6465 6620 5f67 6574 5f70 6172 616d  ..def _get_param
+00001810: 7328 534f 2c20 7a29 3a0a 2020 2020 2222  s(SO, z):.    ""
+00001820: 220a 2020 2020 436f 6d70 7574 6573 2074  ".    Computes t
+00001830: 6865 2062 6573 7420 6669 7420 7061 7261  he best fit para
+00001840: 6d65 7465 7273 2066 6f72 2074 6865 2053  meters for the S
+00001850: 5028 6b29 206d 6f64 656c 2061 7420 6120  P(k) model at a 
+00001860: 7370 6563 6966 6963 2072 6564 7368 6966  specific redshif
+00001870: 742e 200a 0a20 2020 2050 6172 616d 6574  t. ..    Paramet
+00001880: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00001890: 2d2d 0a20 2020 2053 4f20 3a20 696e 740a  --.    SO : int.
+000018a0: 2020 2020 2020 2020 7370 6865 7269 6361          spherica
+000018b0: 6c20 6f76 6572 2d64 656e 7369 7479 2e20  l over-density. 
+000018c0: 4f6e 6c79 2061 6363 6570 7473 2032 3030  Only accepts 200
+000018d0: 206f 7220 3530 300a 2020 2020 7a20 3a20   or 500.    z : 
+000018e0: 666c 6f61 740a 2020 2020 2020 2020 7265  float.        re
+000018f0: 6473 6869 6674 207a 2e20 4f6e 6c79 2061  dshift z. Only a
+00001900: 6363 6570 7473 2076 616c 7565 7320 6f66  ccepts values of
+00001910: 207a 203c 3d20 3320 0a0a 2020 2020 5265   z <= 3 ..    Re
+00001920: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00001930: 2d0a 2020 2020 7061 7261 6d73 3a20 6469  -.    params: di
+00001940: 6374 0a20 2020 2020 2020 2062 6573 7420  ct.        best 
+00001950: 6669 7420 7061 7261 6d65 7465 7273 2066  fit parameters f
+00001960: 6f72 2074 6865 2073 7065 6369 6669 6564  or the specified
+00001970: 2053 4f20 616e 6420 7a2e 0a20 2020 2022   SO and z..    "
+00001980: 2222 0a20 2020 2070 6172 616d 7320 3d20  "".    params = 
+00001990: 7b7d 0a20 2020 2074 7279 3a0a 2020 2020  {}.    try:.    
+000019a0: 2020 2020 666f 7220 7061 7261 6d5f 6920      for param_i 
+000019b0: 696e 205f 6265 7374 5f66 6974 5f76 616c  in _best_fit_val
+000019c0: 735b 7374 7228 534f 295d 3a0a 2020 2020  s[str(SO)]:.    
+000019d0: 2020 2020 2020 2020 7061 7261 6d73 5b70          params[p
+000019e0: 6172 616d 5f69 5d20 3d20 5f70 6f6c 795f  aram_i] = _poly_
+000019f0: 3228 3120 2b20 7a2c 205f 6265 7374 5f66  2(1 + z, _best_f
+00001a00: 6974 5f76 616c 735b 7374 7228 534f 295d  it_vals[str(SO)]
+00001a10: 5b70 6172 616d 5f69 5d29 0a20 2020 2065  [param_i]).    e
+00001a20: 7863 6570 743a 0a20 2020 2020 2020 2072  xcept:.        r
+00001a30: 6169 7365 2045 7863 6570 7469 6f6e 2827  aise Exception('
+00001a40: 2727 5c30 3333 5b39 316d 0a20 2020 2020  ''\033[91m.     
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2053 7068 6572 6963 616c 206f 7665     Spherical ove
+00001a70: 7264 656e 7369 7479 2073 686f 756c 6420  rdensity should 
+00001a80: 6265 2073 7065 6369 6669 6564 2e20 0a20  be specified. . 
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 2020 2050 6c65 6173 6520 7573         Please us
+00001ab0: 6520 3230 3020 6f72 2035 3030 200a 2020  e 200 or 500 .  
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 2020 5c30 3333 5b30 6d27 2727        \033[0m'''
+00001ae0: 290a 2020 2020 7265 7475 726e 2070 6172  ).    return par
+00001af0: 616d 730a 0a0a 6465 6620 5f61 6b69 6e6f  ams...def _akino
+00001b00: 2861 6c70 6861 2c20 6265 7461 2c20 6761  (alpha, beta, ga
+00001b10: 6d6d 612c 206d 5f68 616c 6f2c 207a 2c20  mma, m_halo, z, 
+00001b20: 636f 736d 6f29 3a0a 2020 2020 2222 220a  cosmo):.    """.
+00001b30: 2020 2020 5265 7475 726e 7320 6120 7265      Returns a re
+00001b40: 6473 6869 6674 2064 6570 656e 6465 6e74  dshift dependent
+00001b50: 2070 6f77 6572 2d6c 6177 2066 756e 6374   power-law funct
+00001b60: 696f 6e20 6f66 2074 6865 2062 6172 796f  ion of the baryo
+00001b70: 6e20 6672 6163 7469 6f6e 2061 7320 6120  n fraction as a 
+00001b80: 6675 6e63 7469 6f6e 206f 6620 6861 6c6f  function of halo
+00001b90: 206d 6173 7320 0a20 2020 2061 7320 696e   mass .    as in
+00001ba0: 2041 6b69 6e6f 2065 7420 616c 2e20 3230   Akino et al. 20
+00001bb0: 3232 0a0a 2020 2020 5061 7261 6d65 7465  22..    Paramete
+00001bc0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00001bd0: 2d0a 2020 2020 616c 7068 6120 3a20 666c  -.    alpha : fl
+00001be0: 6f61 740a 2020 2020 2020 2020 7365 7473  oat.        sets
+00001bf0: 2074 6865 2070 6f77 6572 206c 6177 2063   the power law c
+00001c00: 6f6e 7374 616e 740a 2020 2020 6265 7461  onstant.    beta
+00001c10: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
+00001c20: 2073 6574 7320 7468 6520 706f 7765 7220   sets the power 
+00001c30: 6c61 7720 6578 706f 6e65 6e74 0a20 2020  law exponent.   
+00001c40: 2067 616d 6d61 203a 2066 6c6f 6174 0a20   gamma : float. 
+00001c50: 2020 2020 2020 2073 6574 7320 706f 7765         sets powe
+00001c60: 7220 6c61 7720 7265 6473 6869 6674 2064  r law redshift d
+00001c70: 6570 656e 6465 6e63 652e 200a 2020 2020  ependence. .    
+00001c80: 6d5f 6861 6c6f 3a20 6172 7261 7920 6f66  m_halo: array of
+00001c90: 2066 6c6f 6174 0a20 2020 2020 2020 2068   float.        h
+00001ca0: 616c 6f20 6d61 7373 2069 6e20 4d5f 7375  alo mass in M_su
+00001cb0: 6e20 756e 6974 730a 2020 2020 7a20 3a20  n units.    z : 
+00001cc0: 666c 6f61 740a 2020 2020 2020 2020 7265  float.        re
+00001cd0: 6473 6869 6674 207a 0a20 2020 2063 6f73  dshift z.    cos
+00001ce0: 6d6f 3a20 6173 7472 6f70 7920 636f 736d  mo: astropy cosm
+00001cf0: 6f6c 6f67 7920 6f62 6a65 6374 0a20 2020  ology object.   
+00001d00: 2020 2020 2061 7374 726f 7079 2063 6f73       astropy cos
+00001d10: 6d6f 6c6f 6779 206f 626a 6563 7420 7769  mology object wi
+00001d20: 7468 2074 6865 2064 6573 6972 6564 2063  th the desired c
+00001d30: 6f73 6d6f 6c6f 6779 0a20 2020 2020 2020  osmology.       
+00001d40: 200a 2020 2020 5265 7475 726e 730a 2020   .    Returns.  
+00001d50: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6f75    -------.    ou
+00001d60: 7470 7574 3a20 6172 7261 7920 6f66 2066  tput: array of f
+00001d70: 6c6f 6174 0a20 2020 2020 2020 2062 6172  loat.        bar
+00001d80: 796f 6e20 6672 6163 7469 6f6e 206e 6f72  yon fraction nor
+00001d90: 6d61 6c69 7365 6420 6279 2074 6865 2055  malised by the U
+00001da0: 6e69 7665 7273 616c 2062 6172 796f 6e20  niversal baryon 
+00001db0: 6672 6163 7469 6f6e 3a20 665f 6220 2f20  fraction: f_b / 
+00001dc0: 284f 6d65 6761 5f62 202f 204f 6d65 6761  (Omega_b / Omega
+00001dd0: 5f6d 290a 2020 2020 2222 220a 0a20 2020  _m).    """..   
+00001de0: 2041 203d 2030 2e31 3635 3820 2f20 2863   A = 0.1658 / (c
+00001df0: 6f73 6d6f 2e4f 6230 202f 2063 6f73 6d6f  osmo.Ob0 / cosmo
+00001e00: 2e4f 6d30 290a 2020 2020 4220 3d20 5f6e  .Om0).    B = _n
+00001e10: 702e 6578 7028 616c 7068 6129 202f 2031  p.exp(alpha) / 1
+00001e20: 3030 0a20 2020 2043 203d 205f 6e70 2e70  00.    C = _np.p
+00001e30: 6f77 6572 286d 5f68 616c 6f20 2f20 3165  ower(m_halo / 1e
+00001e40: 3134 2c20 6265 7461 202d 2031 290a 2020  14, beta - 1).  
+00001e50: 2020 4420 3d20 5f6e 702e 706f 7765 7228    D = _np.power(
+00001e60: 636f 736d 6f2e 6566 756e 6328 7a29 202f  cosmo.efunc(z) /
+00001e70: 2063 6f73 6d6f 2e65 6675 6e63 2830 2e33   cosmo.efunc(0.3
+00001e80: 292c 2067 616d 6d61 290a 0a20 2020 2072  ), gamma)..    r
+00001e90: 6574 7572 6e20 4120 2a20 4220 2a20 4320  eturn A * B * C 
+00001ea0: 2a20 440a 0a0a 6465 6620 7375 705f 6d6f  * D...def sup_mo
+00001eb0: 6465 6c28 534f 2c20 7a2c 2066 625f 613d  del(SO, z, fb_a=
+00001ec0: 4e6f 6e65 2c20 6662 5f70 6f77 3d4e 6f6e  None, fb_pow=Non
+00001ed0: 652c 2066 625f 7069 766f 743d 312c 204d  e, fb_pivot=1, M
+00001ee0: 5f68 616c 6f3d 4e6f 6e65 2c20 6662 3d4e  _halo=None, fb=N
+00001ef0: 6f6e 652c 2065 7874 7261 706f 6c61 7465  one, extrapolate
+00001f00: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00001f10: 2020 2020 2020 616c 7068 613d 4e6f 6e65        alpha=None
+00001f20: 2c20 6265 7461 3d4e 6f6e 652c 2067 616d  , beta=None, gam
+00001f30: 6d61 3d4e 6f6e 652c 2063 6f73 6d6f 3d4e  ma=None, cosmo=N
+00001f40: 6f6e 652c 206b 5f6d 696e 3d30 2e31 2c20  one, k_min=0.1, 
+00001f50: 6b5f 6d61 783d 382c 206e 3d31 3030 2c20  k_max=8, n=100, 
+00001f60: 0a20 2020 2020 2020 2020 2020 2020 2065  .              e
+00001f70: 7272 6f72 733d 4661 6c73 652c 2076 6572  rrors=False, ver
+00001f80: 626f 7365 3d46 616c 7365 293a 0a20 2020  bose=False):.   
+00001f90: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
+00001fa0: 2074 6865 2073 7570 7072 6573 7369 6f6e   the suppression
+00001fb0: 206f 6620 7468 6520 746f 7461 6c20 6d61   of the total ma
+00001fc0: 7474 6572 2070 6f77 6572 2073 7065 6374  tter power spect
+00001fd0: 7275 6d20 6173 2061 2066 756e 6374 696f  rum as a functio
+00001fe0: 6e20 6f66 2073 6361 6c65 2027 6b27 2075  n of scale 'k' u
+00001ff0: 7369 6e67 2074 6865 2053 5028 6b29 206d  sing the SP(k) m
+00002000: 6f64 656c 2e0a 2020 2020 4175 746f 6d61  odel..    Automa
+00002010: 7469 6361 6c6c 7920 7365 6c65 6374 7320  tically selects 
+00002020: 7468 6520 7265 7175 6972 6564 206f 7074  the required opt
+00002030: 696d 616c 206d 6173 7320 6173 2061 2066  imal mass as a f
+00002040: 756e 6374 696f 6e20 6f66 2073 6361 6c65  unction of scale
+00002050: 2061 6e64 2072 6564 7368 6966 742e 2052   and redshift. R
+00002060: 6571 7569 7265 7320 7468 6520 6261 7279  equires the bary
+00002070: 6f6e 200a 2020 2020 6672 6163 7469 6f6e  on .    fraction
+00002080: 202d 2068 616c 6f20 6d61 7373 2072 656c   - halo mass rel
+00002090: 6174 696f 6e2c 2065 6974 6865 7220 6279  ation, either by
+000020a0: 2073 7065 6369 6679 696e 6720 706f 7765   specifying powe
+000020b0: 722d 6c61 7720 6669 7474 696e 6720 7061  r-law fitting pa
+000020c0: 7261 6d65 7465 7273 2c20 6f72 206e 6f6e  rameters, or non
+000020d0: 2d70 6172 616d 6574 7269 6320 0a20 2020  -parametric .   
+000020e0: 2070 726f 7669 6e67 2061 7272 6179 7320   proving arrays 
+000020f0: 7769 7468 2066 6220 616e 6420 4d5f 6861  with fb and M_ha
+00002100: 6c6f 2061 7420 6120 7370 6563 6966 6963  lo at a specific
+00002110: 2072 6564 7368 6966 742e 2054 6865 2066   redshift. The f
+00002120: 756e 6374 696f 6e20 6163 6365 7074 7320  unction accepts 
+00002130: 6120 7369 6d70 6c65 2070 6f77 6572 206c  a simple power l
+00002140: 6177 2066 6f72 6d20 0a20 2020 206f 7220  aw form .    or 
+00002150: 616e 2041 6b69 6e6f 2065 7420 616c 2032  an Akino et al 2
+00002160: 3032 3220 6675 636e 7469 6f6e 616c 2066  022 fucntional f
+00002170: 6f72 6d2e 2049 6620 6120 6e6f 6e2d 7061  orm. If a non-pa
+00002180: 7261 6d65 7472 6963 2072 656c 6174 696f  rametric relatio
+00002190: 6e20 6973 2067 6976 656e 2c20 616e 200a  n is given, an .
+000021a0: 2020 2020 696e 7465 7270 6f6c 6174 6f72      interpolator
+000021b0: 2069 7320 7573 6564 2074 6f20 636f 6d70   is used to comp
+000021c0: 7574 6520 6662 2061 7420 7468 6520 6f70  ute fb at the op
+000021d0: 7469 6d61 6c20 6d61 7373 2e20 0a0a 2020  timal mass. ..  
+000021e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000021f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00002200: 534f 203a 2069 6e74 0a20 2020 2020 2020  SO : int.       
+00002210: 2073 7068 6572 6963 616c 206f 7665 722d   spherical over-
+00002220: 6465 6e73 6974 792e 204f 6e6c 7920 6163  density. Only ac
+00002230: 6365 7074 7320 3230 3020 6f72 2035 3030  cepts 200 or 500
+00002240: 0a20 2020 207a 203a 2066 6c6f 6174 0a20  .    z : float. 
+00002250: 2020 2020 2020 2072 6564 7368 6966 7420         redshift 
+00002260: 7a2e 204f 6e6c 7920 6163 6365 7074 7320  z. Only accepts 
+00002270: 7661 6c75 6573 206f 6620 7a20 3c3d 2033  values of z <= 3
+00002280: 0a20 2020 2066 625f 6120 3a20 666c 6f61  .    fb_a : floa
+00002290: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+000022a0: 2020 2020 706f 7765 7220 6c61 7720 636f      power law co
+000022b0: 6e73 7461 6e74 0a20 2020 2066 625f 706f  nstant.    fb_po
+000022c0: 7720 3a20 666c 6f61 742c 206f 7074 696f  w : float, optio
+000022d0: 6e61 6c0a 2020 2020 2020 2020 706f 7765  nal.        powe
+000022e0: 7220 6c61 7720 6578 706f 6e65 6e74 0a20  r law exponent. 
+000022f0: 2020 2066 625f 7069 766f 7420 3a20 666c     fb_pivot : fl
+00002300: 6f61 742c 206f 7074 696f 6e61 6c2c 2064  oat, optional, d
+00002310: 6566 6175 6c74 2031 0a20 2020 2020 2020  efault 1.       
+00002320: 2070 6f77 6572 206c 6177 2070 6976 6f74   power law pivot
+00002330: 2070 6f69 6e74 2e20 0a20 2020 2066 6220   point. .    fb 
+00002340: 3a20 6172 7261 7920 6f66 2066 6c6f 6174  : array of float
+00002350: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00002360: 2020 2061 7272 6179 2063 6f6e 7461 696e     array contain
+00002370: 696e 6720 7468 6520 2862 696e 6e65 6429  ing the (binned)
+00002380: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
+00002390: 206e 6f72 6d61 6c69 7365 6420 6279 2074   normalised by t
+000023a0: 6865 2075 6e69 7665 7273 616c 2062 6172  he universal bar
+000023b0: 796f 6e20 6672 6163 7469 6f6e 3a20 0a20  yon fraction: . 
+000023c0: 2020 2020 2020 2066 5f62 202f 2028 4f6d         f_b / (Om
+000023d0: 6567 615f 6220 2f20 4f6d 6567 615f 6d29  ega_b / Omega_m)
+000023e0: 2066 6f72 2074 6865 2066 6220 2d20 4d2d   for the fb - M-
+000023f0: 6861 6c6f 2072 656c 6174 696f 6e2e 0a20  halo relation.. 
+00002400: 2020 204d 5f68 616c 6f20 3a20 6172 7261     M_halo : arra
+00002410: 7920 6f66 2066 6c6f 6174 2c20 6f70 7469  y of float, opti
+00002420: 6f6e 616c 0a20 2020 2020 2020 2061 7272  onal.        arr
+00002430: 6179 2063 6f6e 7461 696e 696e 6720 7468  ay containing th
+00002440: 6520 2862 696e 6e65 6429 2068 616c 6f20  e (binned) halo 
+00002450: 6d61 7373 2066 6f72 2074 6865 2066 6220  mass for the fb 
+00002460: 2d20 4d2d 6861 6c6f 2072 656c 6174 696f  - M-halo relatio
+00002470: 6e20 696e 204d 5f73 756e 2075 6e69 7473  n in M_sun units
+00002480: 2e0a 2020 2020 2020 2020 466f 7220 696e  ..        For in
+00002490: 7465 7270 6f6c 6174 696f 6e2c 206f 7574  terpolation, out
+000024a0: 2d6f 662d 626f 756e 6473 2070 6f69 6e74  -of-bounds point
+000024b0: 7320 7265 7475 726e 204e 614e 732e 0a20  s return NaNs.. 
+000024c0: 2020 2065 7874 7261 706f 6c61 7465 3a20     extrapolate: 
+000024d0: 626f 6f6c 6561 6e2c 2064 6566 6175 6c74  boolean, default
+000024e0: 2046 616c 7365 0a20 2020 2020 2020 2057   False.        W
+000024f0: 6865 7468 6572 2074 6f20 6578 7472 6170  hether to extrap
+00002500: 6f6c 6174 6520 746f 206f 7574 2d6f 662d  olate to out-of-
+00002510: 626f 756e 6473 2070 6f69 6e74 7320 6261  bounds points ba
+00002520: 7365 6420 6f6e 2066 6972 7374 2061 6e64  sed on first and
+00002530: 206c 6173 7420 696e 7465 7276 616c 732c   last intervals,
+00002540: 206f 7220 746f 2072 6574 7572 6e20 4e61   or to return Na
+00002550: 4e73 2e0a 2020 2020 616c 7068 6120 3a20  Ns..    alpha : 
+00002560: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+00002570: 2020 2020 2020 2020 7365 7473 2074 6865          sets the
+00002580: 2041 6b69 6e6f 2070 6f77 6572 206c 6177   Akino power law
+00002590: 2063 6f6e 7374 616e 740a 2020 2020 6265   constant.    be
+000025a0: 7461 203a 2066 6c6f 6174 2c20 6f70 7469  ta : float, opti
+000025b0: 6f6e 616c 0a20 2020 2020 2020 2073 6574  onal.        set
+000025c0: 7320 7468 6520 416b 696e 6f20 706f 7765  s the Akino powe
+000025d0: 7220 6c61 7720 6578 706f 6e65 6e74 0a20  r law exponent. 
+000025e0: 2020 2067 616d 6d61 203a 2066 6c6f 6174     gamma : float
+000025f0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00002600: 2020 2073 6574 7320 7468 6520 416b 696e     sets the Akin
+00002610: 6f20 706f 7765 7220 6c61 7720 7265 6473  o power law reds
+00002620: 6869 6674 2064 6570 656e 6465 6e63 652e  hift dependence.
+00002630: 200a 2020 2020 636f 736d 6f3a 2061 7374   .    cosmo: ast
+00002640: 726f 7079 2063 6f73 6d6f 6c6f 6779 206f  ropy cosmology o
+00002650: 626a 6563 742c 206f 7074 696f 6e61 6c0a  bject, optional.
+00002660: 2020 2020 2020 2020 6173 7472 6f70 7920          astropy 
+00002670: 636f 736d 6f6c 6f67 7920 6f62 6a65 6374  cosmology object
+00002680: 2077 6974 6820 7468 6520 6465 7369 7265   with the desire
+00002690: 6420 636f 736d 6f6c 6f67 790a 2020 2020  d cosmology.    
+000026a0: 6b5f 6d69 6e20 3a20 666c 6f61 742c 2064  k_min : float, d
+000026b0: 6566 6175 6c74 2030 2e31 0a20 2020 2020  efault 0.1.     
+000026c0: 2020 206d 696e 696d 756d 2063 6f2d 6d6f     minimum co-mo
+000026d0: 7669 6e67 2077 6176 656e 756d 6265 7220  ving wavenumber 
+000026e0: 696e 2075 6e69 7473 205b 682f 4d70 635d  in units [h/Mpc]
+000026f0: 0a20 2020 206b 5f6d 6178 203a 2066 6c6f  .    k_max : flo
+00002700: 6174 2c20 6465 6661 756c 7420 382c 206d  at, default 8, m
+00002710: 6178 2031 320a 2020 2020 2020 2020 6d61  ax 12.        ma
+00002720: 7869 6d75 6d20 636f 2d6d 6f76 696e 6720  ximum co-moving 
+00002730: 7761 7665 6e75 6d62 6572 2069 6e20 756e  wavenumber in un
+00002740: 6974 7320 5b68 2f4d 7063 5d2e 2044 6566  its [h/Mpc]. Def
+00002750: 6175 6c74 2069 7320 7365 7420 746f 2074  ault is set to t
+00002760: 6865 204e 7971 7569 7374 2066 7265 7175  he Nyquist frequ
+00002770: 656e 6379 206f 6620 7468 6520 416e 7469  ency of the Anti
+00002780: 6c6c 6573 0a20 2020 2020 2020 2073 696d  lles.        sim
+00002790: 756c 6174 696f 6e73 2028 7365 6520 5361  ulations (see Sa
+000027a0: 6c63 6964 6f20 6574 2061 6c2e 2032 3032  lcido et al. 202
+000027b0: 3229 2e20 0a20 2020 206e 203a 2069 6e74  2). .    n : int
+000027c0: 2c20 6465 6661 756c 7420 3130 300a 2020  , default 100.  
+000027d0: 2020 2020 2020 6e75 6d62 6572 206f 6620        number of 
+000027e0: 6571 7561 6c6c 7920 7370 6163 6564 2063  equally spaced c
+000027f0: 6f2d 6d6f 7669 6e67 2077 6176 656e 756d  o-moving wavenum
+00002800: 6265 7220 696e 206c 6f67 2d73 7061 6365  ber in log-space
+00002810: 6420 6265 7477 6565 6e20 6b5f 6d69 6e20  d between k_min 
+00002820: 616e 6420 6b5f 6d61 782e 0a20 2020 2065  and k_max..    e
+00002830: 7272 6f72 7320 3a20 626f 6f6c 6561 6e2c  rrors : boolean,
+00002840: 2064 6566 6175 6c74 2046 616c 7365 0a20   default False. 
+00002850: 2020 2020 2020 2065 6e61 626c 6573 2061         enables a
+00002860: 6464 6974 696f 6e61 6c20 6f75 7470 7574  dditional output
+00002870: 2077 6974 6820 7468 6520 626f 6f74 7374   with the bootst
+00002880: 7261 7070 6564 2036 3825 2061 6e64 2039  rapped 68% and 9
+00002890: 3525 2063 6f6e 6669 6465 6e63 6520 696e  5% confidence in
+000028a0: 7465 7276 616c 7320 6672 6f6d 2073 7461  tervals from sta
+000028b0: 7469 7374 6963 616c 2065 7272 6f72 732e  tistical errors.
+000028c0: 0a20 2020 2076 6572 626f 7365 203a 2062  .    verbose : b
+000028d0: 6f6f 6c65 616e 2c20 6465 6661 756c 7420  oolean, default 
+000028e0: 5472 7565 0a20 2020 2020 2020 2072 756e  True.        run
+000028f0: 2069 6e20 7665 7262 6f73 6520 6d6f 6465   in verbose mode
+00002900: 0a20 2020 2020 2020 200a 2020 2020 5265  .        .    Re
+00002910: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00002920: 2d0a 2020 2020 6b3a 2061 7272 6179 206f  -.    k: array o
+00002930: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+00002940: 6172 7261 7920 7769 7468 2074 6865 2063  array with the c
+00002950: 6f2d 6d6f 7669 6e67 2077 6176 656e 756d  o-moving wavenum
+00002960: 6265 7220 696e 2075 6e69 7473 205b 682f  ber in units [h/
+00002970: 4d70 635d 0a20 2020 2073 7570 3a20 6172  Mpc].    sup: ar
+00002980: 7261 7920 6f66 2066 6c6f 6174 0a20 2020  ray of float.   
+00002990: 2020 2020 2061 7272 6179 2077 6974 6820       array with 
+000029a0: 7468 6520 7375 7070 7265 7373 696f 6e20  the suppression 
+000029b0: 6f66 2074 6865 2074 6f74 616c 206d 6174  of the total mat
+000029c0: 7465 7220 706f 7765 7220 7370 6563 7472  ter power spectr
+000029d0: 756d 2061 7320 6120 6675 6e63 7469 6f6e  um as a function
+000029e0: 206f 6620 7363 616c 650a 2020 2020 6572   of scale.    er
+000029f0: 726f 725f 3638 5f6d 203a 2061 7272 6179  ror_68_m : array
+00002a00: 206f 6620 666c 6f61 742c 206f 7074 696f   of float, optio
+00002a10: 6e61 6c0a 2020 2020 2020 2020 6172 7261  nal.        arra
+00002a20: 7920 7769 7468 2074 6865 202d 3120 7369  y with the -1 si
+00002a30: 676d 6120 636f 6e66 6964 656e 6365 2069  gma confidence i
+00002a40: 6e74 6572 7661 6c20 0a20 2020 2065 7272  nterval .    err
+00002a50: 6f72 5f36 385f 7020 3a20 6172 7261 7920  or_68_p : array 
+00002a60: 6f66 2066 6c6f 6174 2c20 6f70 7469 6f6e  of float, option
+00002a70: 616c 0a20 2020 2020 2020 2061 7272 6179  al.        array
+00002a80: 2077 6974 6820 7468 6520 2b31 2073 6967   with the +1 sig
+00002a90: 6d61 2063 6f6e 6669 6465 6e63 6520 696e  ma confidence in
+00002aa0: 7465 7276 616c 200a 2020 2020 6572 726f  terval .    erro
+00002ab0: 725f 3935 5f6d 203a 2061 7272 6179 206f  r_95_m : array o
+00002ac0: 6620 666c 6f61 742c 206f 7074 696f 6e61  f float, optiona
+00002ad0: 6c0a 2020 2020 2020 2020 6172 7261 7920  l.        array 
+00002ae0: 7769 7468 2074 6865 202d 3220 7369 676d  with the -2 sigm
+00002af0: 6120 636f 6e66 6964 656e 6365 2069 6e74  a confidence int
+00002b00: 6572 7661 6c20 0a20 2020 2065 7272 6f72  erval .    error
+00002b10: 5f39 355f 7020 3a20 6172 7261 7920 6f66  _95_p : array of
+00002b20: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00002b30: 0a20 2020 2020 2020 2061 7272 6179 2077  .        array w
+00002b40: 6974 6820 7468 6520 2b32 2073 6967 6d61  ith the +2 sigma
+00002b50: 2063 6f6e 6669 6465 6e63 6520 696e 7465   confidence inte
+00002b60: 7276 616c 200a 0a20 2020 204e 6f74 6573  rval ..    Notes
+00002b70: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00002b80: 2020 2020 5468 6520 6d61 7869 6d75 6d20      The maximum 
+00002b90: 636f 2d6d 6f76 696e 6720 7761 7665 6e75  co-moving wavenu
+00002ba0: 6d62 6572 2069 6e20 756e 6974 7320 5b68  mber in units [h
+00002bb0: 2f4d 7063 5d20 6973 2073 6574 2074 6f20  /Mpc] is set to 
+00002bc0: 7468 6520 4e79 7175 6973 7420 6672 6571  the Nyquist freq
+00002bd0: 7565 6e63 7920 6f66 2074 6865 2041 6e74  uency of the Ant
+00002be0: 696c 6c65 7320 7369 6d75 6c61 7469 6f6e  illes simulation
+00002bf0: 7320 0a20 2020 2028 7365 6520 5361 6c63  s .    (see Salc
+00002c00: 6964 6f20 6574 2061 6c2e 2032 3032 3229  ido et al. 2022)
+00002c10: 2e20 416c 7468 6f75 6768 2053 5028 6b29  . Although SP(k)
+00002c20: 2077 6173 2066 6974 7465 6420 7570 2074   was fitted up t
+00002c30: 6f20 6b20 3d20 3132 205b 682f 4d70 635d  o k = 12 [h/Mpc]
+00002c40: 2c20 7765 2063 6175 7469 6f6e 2074 6865  , we caution the
+00002c50: 2075 7365 7220 7468 6174 2073 6574 7469   user that setti
+00002c60: 6e67 200a 2020 2020 f09d 9198 203e 20f0  ng .    .... > .
+00002c70: 9d91 984e 7920 2838 205b 682f 4d70 635d  ...Ny (8 [h/Mpc]
+00002c80: 2920 6d69 6768 7420 6e6f 7420 6265 2072  ) might not be r
+00002c90: 6570 7265 7365 6e74 6174 6976 6520 6f66  epresentative of
+00002ca0: 2074 6865 2074 7275 6520 756e 6365 7274   the true uncert
+00002cb0: 6169 6e74 6965 7320 696e 2074 6865 2064  ainties in the d
+00002cc0: 6174 612e 200a 2020 2020 2222 220a 0a20  ata. .    """.. 
+00002cd0: 2020 2069 6620 7a20 3c20 303a 0a20 2020     if z < 0:.   
+00002ce0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00002cf0: 7469 6f6e 2827 5c30 3333 5b39 316d 496e  tion('\033[91mIn
+00002d00: 636f 7272 6563 7420 7265 6473 6869 6674  correct redshift
+00002d10: 2e5c 3033 335b 306d 2729 2066 726f 6d20  .\033[0m') from 
+00002d20: 4e6f 6e65 0a20 2020 2020 2020 200a 2020  None.        .  
+00002d30: 2020 6966 207a 203e 2033 3a0a 2020 2020    if z > 3:.    
+00002d40: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+00002d50: 696f 6e28 275c 3033 335b 3931 6d70 792d  ion('\033[91mpy-
+00002d60: 7370 6b20 7761 7320 6361 6c69 6272 6174  spk was calibrat
+00002d70: 6564 2075 7020 746f 207a 203d 2033 2e30  ed up to z = 3.0
+00002d80: 2e20 270a 2020 2020 2020 2020 2020 2020  . '.            
+00002d90: 2020 2020 2020 2020 2020 2020 2750 6c65              'Ple
+00002da0: 6173 6520 7370 6563 6966 7920 7a20 3c3d  ase specify z <=
+00002db0: 2033 2e30 205c 3033 335b 306d 2729 2066   3.0 \033[0m') f
+00002dc0: 726f 6d20 4e6f 6e65 0a0a 2020 2020 6966  rom None..    if
+00002dd0: 207a 203c 2030 2e31 3235 3a0a 2020 2020   z < 0.125:.    
+00002de0: 2020 2020 5f77 6172 6e69 6e67 732e 7761      _warnings.wa
+00002df0: 726e 2827 5c30 3333 5b33 336d 7079 2d73  rn('\033[33mpy-s
+00002e00: 706b 2077 6173 2063 616c 6962 7261 7465  pk was calibrate
+00002e10: 6420 646f 776e 2074 6f20 7a20 3d20 302e  d down to z = 0.
+00002e20: 3132 352e 2052 6564 7368 6966 7473 2027  125. Redshifts '
+00002e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002e40: 2020 2020 2020 2020 277a 203c 2030 2e31          'z < 0.1
+00002e50: 3235 206d 6179 206e 6f74 2062 6520 6163  25 may not be ac
+00002e60: 6375 7261 7465 6c79 2072 6570 726f 6475  curately reprodu
+00002e70: 6365 6420 6279 2074 6865 206d 6f64 656c  ced by the model
+00002e80: 2e20 5c30 3333 5b30 6d27 2c20 7374 6163  . \033[0m', stac
+00002e90: 6b6c 6576 656c 3d32 290a 0a20 2020 2069  klevel=2)..    i
+00002ea0: 6620 6b5f 6d61 7820 3e20 3132 3a0a 2020  f k_max > 12:.  
+00002eb0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+00002ec0: 7074 696f 6e28 275c 3033 335b 3931 6d70  ption('\033[91mp
+00002ed0: 792d 7370 6b20 7761 7320 6361 6c69 6272  y-spk was calibr
+00002ee0: 6174 6564 2075 7020 746f 206b 5f6d 6178  ated up to k_max
+00002ef0: 203d 2031 3220 5b68 2f4d 7063 5d20 270a   = 12 [h/Mpc] '.
+00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f10: 2020 2020 2020 2020 2750 6c65 6173 6520          'Please 
+00002f20: 7370 6563 6966 7920 6b5f 6d61 7820 3c3d  specify k_max <=
+00002f30: 2031 3220 5b68 2f4d 7063 5d20 5c30 3333   12 [h/Mpc] \033
+00002f40: 5b30 6d27 2920 6672 6f6d 204e 6f6e 650a  [0m') from None.
+00002f50: 2020 2020 2020 2020 0a20 2020 2069 6620          .    if 
+00002f60: 6b5f 6d61 7820 3e20 383a 0a20 2020 2020  k_max > 8:.     
+00002f70: 2020 205f 7761 726e 696e 6773 2e77 6172     _warnings.war
+00002f80: 6e28 275c 3033 335b 3333 6d53 6361 6c65  n('\033[33mScale
+00002f90: 7320 7769 7468 206b 5f6d 6178 203e 206b  s with k_max > k
+00002fa0: 5f6e 7920 3d20 3820 5b68 2f4d 7063 5d20  _ny = 8 [h/Mpc] 
+00002fb0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00002fc0: 2020 2020 2020 2020 2027 6d61 7920 6e6f           'may no
+00002fd0: 7420 6265 2061 6363 7572 6174 656c 7920  t be accurately 
+00002fe0: 7265 7072 6f64 7563 6564 2062 7920 7468  reproduced by th
+00002ff0: 6520 6d6f 6465 6c2e 205c 3033 335b 306d  e model. \033[0m
+00003000: 272c 2073 7461 636b 6c65 7665 6c3d 3229  ', stacklevel=2)
+00003010: 0a0a 2020 2020 6966 2063 6f73 6d6f 2069  ..    if cosmo i
+00003020: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003030: 2020 2020 6966 206e 6f74 2063 6f73 6d6f      if not cosmo
+00003040: 2e4f 6230 3a0a 2020 2020 2020 2020 2020  .Ob0:.          
+00003050: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+00003060: 6e28 275c 3033 335b 3931 6d49 6e63 6f72  n('\033[91mIncor
+00003070: 7265 6374 2063 6f73 6d6f 6c6f 6779 2e20  rect cosmology. 
+00003080: 506c 6561 7365 2073 7065 6369 6679 204f  Please specify O
+00003090: 6d65 6761 5f62 6172 796f 6e2e 5c30 3333  mega_baryon.\033
+000030a0: 5b30 6d27 2920 6672 6f6d 204e 6f6e 650a  [0m') from None.
+000030b0: 0a20 2020 2070 6172 616d 7320 3d20 5f67  .    params = _g
+000030c0: 6574 5f70 6172 616d 7328 534f 2c20 7a29  et_params(SO, z)
+000030d0: 0a20 2020 206b 203d 205f 6e70 2e72 6f75  .    k = _np.rou
+000030e0: 6e64 285f 6e70 2e6c 6f67 7370 6163 6528  nd(_np.logspace(
+000030f0: 5f6e 702e 6c6f 6731 3028 6b5f 6d69 6e29  _np.log10(k_min)
+00003100: 2c20 5f6e 702e 6c6f 6731 3028 6b5f 6d61  , _np.log10(k_ma
+00003110: 7829 2c20 6e29 2c20 3629 0a20 2020 206c  x), n), 6).    l
+00003120: 6f67 6b20 3d20 5f6e 702e 6c6f 6731 3028  ogk = _np.log10(
+00003130: 6b29 0a0a 2020 2020 6265 7374 5f6d 6173  k)..    best_mas
+00003140: 7320 3d20 5f6f 7074 696d 616c 5f6d 6173  s = _optimal_mas
+00003150: 735f 6675 6e63 7428 6b2c 2070 6172 616d  s_funct(k, param
+00003160: 7329 0a0a 2020 2020 6966 2028 6662 5f61  s)..    if (fb_a
+00003170: 2069 7320 6e6f 7420 4e6f 6e65 2920 6f72   is not None) or
+00003180: 2028 6662 5f70 6f77 2069 7320 6e6f 7420   (fb_pow is not 
+00003190: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+000031a0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+000031b0: 2020 2020 2020 2070 7269 6e74 2827 5c30         print('\0
+000031c0: 3333 5b33 366d 5573 696e 6720 706f 7765  33[36mUsing powe
+000031d0: 722d 6c61 7720 6669 7420 666f 7220 6662  r-law fit for fb
+000031e0: 202d 204d 5f68 616c 6f20 6174 207a 3d25   - M_halo at z=%
+000031f0: 2e33 662c 2027 200a 2020 2020 2020 2020  .3f, ' .        
+00003200: 2020 2020 2020 2020 2020 276e 6f72 6d61            'norma
+00003210: 6c69 7365 6420 6174 204d 5f68 616c 6f20  lised at M_halo 
+00003220: 3d20 252e 3265 205b 4d5f 7375 6e5d 205c  = %.2e [M_sun] \
+00003230: 3033 335b 306d 2720 2520 287a 2c20 6662  033[0m' % (z, fb
+00003240: 5f70 6976 6f74 2929 0a20 2020 2020 2020  _pivot)).       
+00003250: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00003260: 2020 665f 6220 3d20 5f70 6f77 6572 5f6c    f_b = _power_l
+00003270: 6177 2831 3020 2a2a 2062 6573 745f 6d61  aw(10 ** best_ma
+00003280: 7373 2c20 6662 5f61 2c20 6662 5f70 6f77  ss, fb_a, fb_pow
+00003290: 2c20 6662 5f70 6976 6f74 290a 2020 2020  , fb_pivot).    
+000032a0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+000032b0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+000032c0: 6365 7074 696f 6e28 275c 3033 335b 3931  ception('\033[91
+000032d0: 6d57 6865 6e20 7573 696e 6720 6120 706f  mWhen using a po
+000032e0: 7765 722d 6c61 772c 2062 6f74 6820 7061  wer-law, both pa
+000032f0: 7261 6d65 7465 7273 2073 686f 756c 6420  rameters should 
+00003300: 6265 2067 6976 656e 2e20 270a 2020 2020  be given. '.    
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 2020 2020 2020 2020 2750 6c65 6173 6520          'Please 
+00003330: 7370 6563 6966 793a 2066 625f 6120 616e  specify: fb_a an
+00003340: 6420 6662 5f70 6f77 205c 3033 335b 306d  d fb_pow \033[0m
+00003350: 2729 2066 726f 6d20 4e6f 6e65 0a20 2020  ') from None.   
+00003360: 2065 6c69 6620 284d 5f68 616c 6f20 6973   elif (M_halo is
+00003370: 206e 6f74 204e 6f6e 6529 206f 7220 2866   not None) or (f
+00003380: 6220 6973 206e 6f74 204e 6f6e 6529 3a0a  b is not None):.
+00003390: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+000033a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000033b0: 7072 696e 7428 275c 3033 335b 3336 6d55  print('\033[36mU
+000033c0: 7369 6e67 2062 696e 6e65 6420 6461 7461  sing binned data
+000033d0: 2066 6f72 2066 6220 2d20 4d5f 6861 6c6f   for fb - M_halo
+000033e0: 2061 7420 7a3d 252e 3366 205c 3033 335b   at z=%.3f \033[
+000033f0: 306d 2720 2520 7a29 0a20 2020 2020 2020  0m' % z).       
+00003400: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00003410: 2020 6662 5f69 6e74 6572 203d 205f 416b    fb_inter = _Ak
+00003420: 696d 6131 4449 6e74 6572 706f 6c61 746f  ima1DInterpolato
+00003430: 7228 5f6e 702e 6c6f 6731 3028 4d5f 6861  r(_np.log10(M_ha
+00003440: 6c6f 292c 205f 6e70 2e6c 6f67 3130 2866  lo), _np.log10(f
+00003450: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
+00003460: 6966 2065 7874 7261 706f 6c61 7465 3a0a  if extrapolate:.
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 6662 5f69 6e74 6572 2e65 7874 7261 706f  fb_inter.extrapo
+00003490: 6c61 7465 203d 2054 7275 650a 2020 2020  late = True.    
+000034a0: 2020 2020 2020 2020 665f 6220 3d20 3130          f_b = 10
+000034b0: 202a 2a20 6662 5f69 6e74 6572 2862 6573   ** fb_inter(bes
+000034c0: 745f 6d61 7373 290a 2020 2020 2020 2020  t_mass).        
+000034d0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000034e0: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
+000034f0: 696f 6e28 275c 3033 335b 3931 6d57 6865  ion('\033[91mWhe
+00003500: 6e20 7573 696e 6720 6269 6e6e 6564 2064  n using binned d
+00003510: 6174 612c 2062 6f74 6820 6861 6c6f 206d  ata, both halo m
+00003520: 6173 7320 616e 6420 6261 7279 6f6e 2027  ass and baryon '
+00003530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003540: 2020 2020 2020 2020 2020 2020 2027 6672               'fr
+00003550: 6163 7469 6f6e 2073 686f 756c 6420 6265  action should be
+00003560: 2067 6976 656e 2061 7320 6d6f 6e6f 746f   given as monoto
+00003570: 6e69 6361 6c6c 7920 696e 6372 6561 7369  nically increasi
+00003580: 6e67 2061 7272 6179 732e 2027 0a20 2020  ng arrays. '.   
+00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035a0: 2020 2020 2020 2020 2027 506c 6561 7365           'Please
+000035b0: 2073 7065 6369 6679 3a20 4d5f 6861 6c6f   specify: M_halo
+000035c0: 2028 6172 7261 7929 2061 6e64 2066 6220   (array) and fb 
+000035d0: 2861 7272 6179 292e 205c 3033 335b 306d  (array). \033[0m
+000035e0: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
+000035f0: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
+00003600: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00003610: 6e74 2827 5c30 3333 5b33 366d 5573 696e  nt('\033[36mUsin
+00003620: 6720 616e 2041 6b69 6e6f 2065 7420 616c  g an Akino et al
+00003630: 2e20 3230 3232 2070 6f77 6572 2d6c 6177  . 2022 power-law
+00003640: 2066 6974 2066 6f72 2066 6220 2720 0a20   fit for fb ' . 
+00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003660: 2027 2d20 4d5f 6861 6c6f 2061 7420 7a3d   '- M_halo at z=
+00003670: 252e 3366 2e20 5c30 3333 5b30 6d27 2025  %.3f. \033[0m' %
+00003680: 207a 290a 2020 2020 2020 2020 7472 793a   z).        try:
+00003690: 0a20 2020 2020 2020 2020 2020 2066 5f62  .            f_b
+000036a0: 203d 205f 616b 696e 6f28 616c 7068 612c   = _akino(alpha,
+000036b0: 2062 6574 612c 2067 616d 6d61 2c20 3130   beta, gamma, 10
+000036c0: 202a 2a20 6265 7374 5f6d 6173 732c 207a   ** best_mass, z
+000036d0: 2c20 636f 736d 6f29 0a20 2020 2020 2020  , cosmo).       
+000036e0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+000036f0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00003700: 7469 6f6e 2827 5c30 3333 5b39 316d 5573  tion('\033[91mUs
+00003710: 696e 6720 616e 2041 6b69 6e6f 2070 6f77  ing an Akino pow
+00003720: 6572 2d6c 6177 2e20 270a 2020 2020 2020  er-law. '.      
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 2020 2020 2020 2750 6c65 6173 6520 7370        'Please sp
+00003750: 6563 6966 793a 2061 6c70 6861 2c20 6265  ecify: alpha, be
+00003760: 7461 2c20 6761 6d6d 612c 2061 6e64 2063  ta, gamma, and c
+00003770: 6f73 6d6f 6c6f 6779 2028 636f 736d 6f29  osmology (cosmo)
+00003780: 205c 3033 335b 306d 2729 2066 726f 6d20   \033[0m') from 
+00003790: 4e6f 6e65 0a0a 2020 2020 6d69 6e5f 6662  None..    min_fb
+000037a0: 2c20 6d61 785f 6662 203d 2067 6574 5f6c  , max_fb = get_l
+000037b0: 696d 6974 7328 534f 2c20 7a2c 2031 3020  imits(SO, z, 10 
+000037c0: 2a2a 2062 6573 745f 6d61 7373 290a 0a20  ** best_mass).. 
+000037d0: 2020 206f 7574 5f6d 696e 203d 2066 5f62     out_min = f_b
+000037e0: 203c 206d 696e 5f66 620a 2020 2020 6f75   < min_fb.    ou
+000037f0: 745f 6d61 7820 3d20 665f 6220 3e20 6d61  t_max = f_b > ma
+00003800: 785f 6662 0a0a 2020 2020 6d61 7373 5f6f  x_fb..    mass_o
+00003810: 7574 5f6d 696e 203d 2062 6573 745f 6d61  ut_min = best_ma
+00003820: 7373 5b6f 7574 5f6d 696e 5d0a 0a20 2020  ss[out_min]..   
+00003830: 2069 6620 616e 7928 6f75 745f 6d69 6e29   if any(out_min)
+00003840: 3a0a 2020 2020 2020 2020 5f77 6172 6e69  :.        _warni
+00003850: 6e67 732e 7761 726e 2827 5c30 3333 5b39  ngs.warn('\033[9
+00003860: 316d 466f 756e 6420 6261 7279 6f6e 2066  1mFound baryon f
+00003870: 7261 6374 696f 6e20 7661 6c75 6573 206f  raction values o
+00003880: 7574 7369 6465 2066 6974 7469 6e67 206c  utside fitting l
+00003890: 696d 6974 732e 2027 0a20 2020 2020 2020  imits. '.       
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038b0: 2766 6220 3c20 6c6f 7765 725f 6c69 6d69  'fb < lower_limi
+000038c0: 7420 6265 7477 6565 6e20 252e 3165 203c  t between %.1e <
+000038d0: 3d20 4d5f 6861 6c6f 205b 4d5f 7375 6e5d  = M_halo [M_sun]
+000038e0: 203c 3d20 252e 3165 2e20 2720 0a20 2020   <= %.1e. ' .   
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2773 7570 5f6d 6f64 656c 2829      'sup_model()
+00003910: 2077 696c 6c20 7265 7475 726e 204e 614e   will return NaN
+00003920: 7320 7769 7468 696e 2074 686f 7365 206c  s within those l
+00003930: 696d 6974 732e 205c 3033 335b 306d 2720  imits. \033[0m' 
+00003940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003950: 2020 2020 2020 2020 2520 2831 3020 2a2a          % (10 **
+00003960: 206d 6173 735f 6f75 745f 6d69 6e2e 6d69   mass_out_min.mi
+00003970: 6e28 292c 2031 3020 2a2a 206d 6173 735f  n(), 10 ** mass_
+00003980: 6f75 745f 6d69 6e2e 6d61 7828 2929 2c20  out_min.max()), 
+00003990: 7374 6163 6b6c 6576 656c 3d32 290a 0a20  stacklevel=2).. 
+000039a0: 2020 206d 6173 735f 6f75 745f 6d61 7820     mass_out_max 
+000039b0: 3d20 6265 7374 5f6d 6173 735b 6f75 745f  = best_mass[out_
+000039c0: 6d61 785d 0a0a 2020 2020 6966 2061 6e79  max]..    if any
+000039d0: 286f 7574 5f6d 6178 293a 0a20 2020 2020  (out_max):.     
+000039e0: 2020 205f 7761 726e 696e 6773 2e77 6172     _warnings.war
+000039f0: 6e28 275c 3033 335b 3931 6d46 6f75 6e64  n('\033[91mFound
+00003a00: 2062 6172 796f 6e20 6672 6163 7469 6f6e   baryon fraction
+00003a10: 2076 616c 7565 7320 6f75 7473 6964 6520   values outside 
+00003a20: 6669 7474 696e 6720 6c69 6d69 7473 2e20  fitting limits. 
+00003a30: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00003a40: 2020 2020 2020 2020 2027 6662 203e 2075           'fb > u
+00003a50: 7070 6572 5f6c 696d 6974 2062 6574 7765  pper_limit betwe
+00003a60: 656e 2025 2e31 6520 3c3d 204d 5f68 616c  en %.1e <= M_hal
+00003a70: 6f20 5b4d 5f73 756e 5d20 3c3d 2025 2e31  o [M_sun] <= %.1
+00003a80: 652e 2027 200a 2020 2020 2020 2020 2020  e. ' .          
+00003a90: 2020 2020 2020 2020 2020 2020 2027 7375               'su
+00003aa0: 705f 6d6f 6465 6c28 2920 7769 6c6c 2072  p_model() will r
+00003ab0: 6574 7572 6e20 4e61 4e73 2077 6974 6869  eturn NaNs withi
+00003ac0: 6e20 7468 6f73 6520 6c69 6d69 7473 2e20  n those limits. 
+00003ad0: 5c30 3333 5b30 6d27 200a 2020 2020 2020  \033[0m' .      
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2025 2028 3130 202a 2a20 6d61 7373 5f6f   % (10 ** mass_o
+00003b00: 7574 5f6d 6178 2e6d 696e 2829 2c20 3130  ut_max.min(), 10
+00003b10: 202a 2a20 6d61 7373 5f6f 7574 5f6d 6178   ** mass_out_max
+00003b20: 2e6d 6178 2829 292c 2073 7461 636b 6c65  .max()), stackle
+00003b30: 7665 6c3d 3229 0a0a 2020 2020 6d61 736b  vel=2)..    mask
+00003b40: 203d 205f 6e70 2e6c 6f67 6963 616c 5f6f   = _np.logical_o
+00003b50: 7228 6f75 745f 6d69 6e2c 6f75 745f 6d61  r(out_min,out_ma
+00003b60: 7829 0a0a 2020 2020 7830 203d 205f 6c61  x)..    x0 = _la
+00003b70: 6d62 6461 5f66 756e 6374 286c 6f67 6b2c  mbda_funct(logk,
+00003b80: 2070 6172 616d 7329 0a20 2020 2078 3120   params).    x1 
+00003b90: 3d20 5f6d 755f 6675 6e63 7428 6c6f 676b  = _mu_funct(logk
+00003ba0: 2c20 7061 7261 6d73 290a 2020 2020 7832  , params).    x2
+00003bb0: 203d 205f 6e75 5f66 756e 6328 6c6f 676b   = _nu_func(logk
+00003bc0: 2c20 7061 7261 6d73 290a 0a20 2020 2073  , params)..    s
+00003bd0: 7570 203d 2078 3020 2d20 2878 3020 2d20  up = x0 - (x0 - 
+00003be0: 7831 2920 2a20 5f6e 702e 6578 7028 2d78  x1) * _np.exp(-x
+00003bf0: 3220 2a20 665f 6229 0a0a 2020 2020 7375  2 * f_b)..    su
+00003c00: 705b 6d61 736b 5d20 3d20 5f6e 702e 4e41  p[mask] = _np.NA
+00003c10: 4e0a 0a20 2020 2069 6620 6572 726f 7273  N..    if errors
+00003c20: 3a0a 2020 2020 2020 2020 7261 775f 7461  :.        raw_ta
+00003c30: 626c 6520 3d20 5f70 6b67 7574 696c 2e67  ble = _pkgutil.g
+00003c40: 6574 5f64 6174 6128 5f5f 6e61 6d65 5f5f  et_data(__name__
+00003c50: 2c20 2773 7461 745f 6572 726f 7273 5f27  , 'stat_errors_'
+00003c60: 202b 2073 7472 2028 534f 2920 2b20 272e   + str (SO) + '.
+00003c70: 6373 7627 292e 6465 636f 6465 2827 7574  csv').decode('ut
+00003c80: 662d 3827 292e 7370 6c69 746c 696e 6573  f-8').splitlines
+00003c90: 2829 0a20 2020 2020 2020 2074 6162 6c65  ().        table
+00003ca0: 203d 205f 6e70 2e6c 6f61 6474 7874 2872   = _np.loadtxt(r
+00003cb0: 6177 5f74 6162 6c65 2c20 6465 6c69 6d69  aw_table, delimi
+00003cc0: 7465 723d 222c 222c 2073 6b69 7072 6f77  ter=",", skiprow
+00003cd0: 733d 3129 0a20 2020 2020 2020 2063 6f6f  s=1).        coo
+00003ce0: 7264 7320 3d20 7461 626c 655b 3a2c 205b  rds = table[:, [
+00003cf0: 302c 2031 2c20 325d 5d0a 2020 2020 2020  0, 1, 2]].      
+00003d00: 2020 696e 7465 7270 5f36 385f 6d20 3d20    interp_68_m = 
+00003d10: 5f4c 696e 6561 724e 4449 6e74 6572 706f  _LinearNDInterpo
+00003d20: 6c61 746f 7228 636f 6f72 6473 2c20 7461  lator(coords, ta
+00003d30: 626c 655b 3a2c 2034 5d2c 2072 6573 6361  ble[:, 4], resca
+00003d40: 6c65 3d54 7275 6529 0a20 2020 2020 2020  le=True).       
+00003d50: 2069 6e74 6572 705f 3638 5f70 203d 205f   interp_68_p = _
+00003d60: 4c69 6e65 6172 4e44 496e 7465 7270 6f6c  LinearNDInterpol
+00003d70: 6174 6f72 2863 6f6f 7264 732c 2074 6162  ator(coords, tab
+00003d80: 6c65 5b3a 2c20 355d 2c20 7265 7363 616c  le[:, 5], rescal
+00003d90: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+00003da0: 696e 7465 7270 5f39 355f 6d20 3d20 5f4c  interp_95_m = _L
+00003db0: 696e 6561 724e 4449 6e74 6572 706f 6c61  inearNDInterpola
+00003dc0: 746f 7228 636f 6f72 6473 2c20 7461 626c  tor(coords, tabl
+00003dd0: 655b 3a2c 2036 5d2c 2072 6573 6361 6c65  e[:, 6], rescale
+00003de0: 3d54 7275 6529 0a20 2020 2020 2020 2069  =True).        i
+00003df0: 6e74 6572 705f 3935 5f70 203d 205f 4c69  nterp_95_p = _Li
+00003e00: 6e65 6172 4e44 496e 7465 7270 6f6c 6174  nearNDInterpolat
+00003e10: 6f72 2863 6f6f 7264 732c 2074 6162 6c65  or(coords, table
+00003e20: 5b3a 2c20 375d 2c20 7265 7363 616c 653d  [:, 7], rescale=
+00003e30: 5472 7565 290a 0a20 2020 2020 2020 207a  True)..        z
+00003e40: 5f61 7272 6179 203d 205f 6e70 2e66 756c  _array = _np.ful
+00003e50: 6c5f 6c69 6b65 286b 2c20 7a29 0a20 2020  l_like(k, z).   
+00003e60: 2020 2020 2064 6174 6120 3d20 5f6e 702e       data = _np.
+00003e70: 636f 6c75 6d6e 5f73 7461 636b 285b 6b2c  column_stack([k,
+00003e80: 2066 5f62 2c20 7a5f 6172 7261 795d 290a   f_b, z_array]).
+00003e90: 2020 2020 2020 2020 6572 726f 725f 3638          error_68
+00003ea0: 5f6d 203d 2069 6e74 6572 705f 3638 5f6d  _m = interp_68_m
+00003eb0: 2864 6174 6129 0a20 2020 2020 2020 2065  (data).        e
+00003ec0: 7272 6f72 5f36 385f 7020 3d20 696e 7465  rror_68_p = inte
+00003ed0: 7270 5f36 385f 7028 6461 7461 290a 2020  rp_68_p(data).  
+00003ee0: 2020 2020 2020 6572 726f 725f 3935 5f6d        error_95_m
+00003ef0: 203d 2069 6e74 6572 705f 3935 5f6d 2864   = interp_95_m(d
+00003f00: 6174 6129 0a20 2020 2020 2020 2065 7272  ata).        err
+00003f10: 6f72 5f39 355f 7020 3d20 696e 7465 7270  or_95_p = interp
+00003f20: 5f39 355f 7028 6461 7461 290a 0a20 2020  _95_p(data)..   
+00003f30: 2020 2020 2072 6574 7572 6e20 6b2c 2073       return k, s
+00003f40: 7570 2c20 6572 726f 725f 3638 5f6d 2c20  up, error_68_m, 
+00003f50: 6572 726f 725f 3638 5f70 2c20 6572 726f  error_68_p, erro
+00003f60: 725f 3935 5f6d 2c20 6572 726f 725f 3935  r_95_m, error_95
+00003f70: 5f70 0a0a 2020 2020 656c 7365 3a0a 2020  _p..    else:.  
+00003f80: 2020 2020 2020 7265 7475 726e 206b 2c20        return k, 
+00003f90: 7375 700a                                sup.
```

### Comparing `pyspk-1.3/pyspk/fit_vals.py` & `pyspk-1.4/pyspk/fit_vals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Contains the best fit values as in Salcido et al. (2022).
+Contains the best fit values as in Salcido et al. (2023).
 """
 
 
 best_fit_vals = {}
 best_fit_vals['200'] = {'alpha': [15.24311120000861,-1.2436699435560352,0.14837558774401766],
                         'beta': [14.969187892657688,-1.0993025612653198,0.12905587245129102],
                         'gamma': [0.8000441576980428,-0.01715621131893159,0.06131887249968379],
```

### Comparing `pyspk-1.3/pyspk/stat_errors_200.csv` & `pyspk-1.4/pyspk/stat_errors_200.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1,1476 +1,1477 @@
 k,f_b,z,n,error_68_m,error_68_p,error_95_m,error_95_p
-0.0999999999999977,0.45,0.0,22.0,-0.00015922638302328648,0.00017035415371493895,-0.00030888432952992114,0.000351207711089524
-0.0999999999999977,0.51,0.0,17.0,-0.00016874479199262426,0.0002744023143379204,-0.0002942871536180681,0.0006179629165541839
-0.0999999999999977,0.57,0.0,36.0,-0.0001047397261533431,0.00015130631319723448,-0.0001936836973497325,0.0003218012307155347
-0.0999999999999977,0.63,0.0,52.0,-0.0001175510362576794,0.00014918566176102806,-0.00023120090486603766,0.0003078425991951209
-0.0999999999999977,0.69,0.0,55.0,-7.045549192840619e-05,9.689926762260152e-05,-0.00013309549576457185,0.00021565280370523338
-0.0999999999999977,0.75,0.0,70.0,-8.737619287516132e-05,7.752832000824959e-05,-0.00017938032432132054,0.00015129187365124213
-0.0999999999999977,0.81,0.0,151.0,-7.020533147231338e-05,7.523978759357799e-05,-0.0001349901825703263,0.00015045049191335832
-0.0999999999999977,0.87,0.0,91.0,-0.00011893729476225534,0.00010804420770102982,-0.00022539708366672457,0.00022058422571914638
-0.1270454343320573,0.45,0.0,22.0,-0.00027444788977159623,0.0003059450100689835,-0.0005574392061434703,0.0006041854310088455
-0.1270454343320573,0.51,0.0,18.0,-0.00023525308066294412,0.00034004067528212986,-0.00042866994877147746,0.0007191415094130131
-0.1270454343320573,0.57,0.0,40.0,-0.00012901685076701323,0.0001621444819847474,-0.00024174965523044315,0.00035540335281063136
-0.1270454343320573,0.63,0.0,50.0,-0.00015108612065294178,0.00017564458315428438,-0.0002824587670352926,0.00035958285363427487
-0.1270454343320573,0.69,0.0,55.0,-8.342556743807009e-05,0.00010855968502522058,-0.0001597381179758584,0.0002369517401249878
-0.1270454343320573,0.75,0.0,71.0,-9.239263962630408e-05,9.256969136695563e-05,-0.00018293602402897043,0.00018573295840248853
-0.1270454343320573,0.81,0.0,154.0,-7.058777551984996e-05,7.462652267938283e-05,-0.00013455444254782483,0.00015101384224822093
-0.1270454343320573,0.87,0.0,83.0,-0.00012852390400701122,0.00011949190275679736,-0.00024191291181845426,0.00024062366294703495
-0.1614054238462082,0.39,0.0,5.0,-0.0008094945810348528,0.000831452093845675,-0.0013213794583144534,0.0017919446104500247
-0.1614054238462082,0.45,0.0,22.0,-0.0004778848550162816,0.00048663988342720864,-0.0009244027106392716,0.001008831657444288
-0.1614054238462082,0.51,0.0,19.0,-0.0004111037199597134,0.0005051356554787908,-0.0007343261126833471,0.0010753930778915782
-0.1614054238462082,0.57,0.0,41.0,-0.00017566448631033715,0.00019655623029158915,-0.0003386214423017335,0.0003986875770358598
-0.1614054238462082,0.63,0.0,54.0,-0.00018301300696386397,0.00021073072490753364,-0.0003499592449717271,0.0004108930734598025
-0.1614054238462082,0.69,0.0,54.0,-0.00010951796550661682,0.00013688200048043054,-0.0002118292021494599,0.0002835212183996892
-0.1614054238462082,0.75,0.0,70.0,-0.00013079666403304751,0.00010953291037961576,-0.000264953265106457,0.00020374365829501582
-0.1614054238462082,0.81,0.0,154.0,-8.443155296991659e-05,8.453227997789011e-05,-0.00016414952251551912,0.00016949011409380207
-0.1614054238462082,0.87,0.0,78.0,-0.00014098571656705078,0.00013122183630653473,-0.0002776394049309514,0.0002588886971588657
-0.2050582217609075,0.39,0.0,6.0,-0.0016130111045104163,0.001509489252378463,-0.0028243920902878052,0.003077380467538793
-0.2050582217609075,0.45,0.0,21.0,-0.0008093714610602514,0.0007754677400335626,-0.0015150123122671891,0.0016041270358003983
-0.2050582217609075,0.51,0.0,23.0,-0.0005791863081287622,0.0006382335408567536,-0.0010722812069095824,0.0013591823838148829
-0.2050582217609075,0.57,0.0,42.0,-0.0002992557676189483,0.0003066399209244126,-0.0005943062513872223,0.0006103083777978956
-0.2050582217609075,0.63,0.0,56.0,-0.00025790016059669245,0.0002846667091319036,-0.0004905925629135508,0.0005835514054962533
-0.2050582217609075,0.69,0.0,52.0,-0.00014721964550300164,0.00017433408316065404,-0.0002767641454437831,0.0003673893979673408
-0.2050582217609075,0.75,0.0,66.0,-0.000116655789063638,0.00012907482353590244,-0.00022950557762623416,0.0002602227118007279
-0.2050582217609075,0.81,0.0,155.0,-0.00015236749888020062,0.00012646149165683175,-0.00032385186336695757,0.000234760985198898
-0.2050582217609075,0.87,0.0,76.0,-0.00016908703797804695,0.00015719310383776027,-0.0003198452138237729,0.000321624960569688
-0.2605171084697353,0.39,0.0,7.0,-0.002313703951631013,0.002370913717034382,-0.004470595939769998,0.004326084333426659
-0.2605171084697353,0.45,0.0,21.0,-0.0012509142975913306,0.0012354897099031337,-0.0023684379234625093,0.0024001130757307916
-0.2605171084697353,0.51,0.0,28.0,-0.0008142381081844598,0.0007936451180437519,-0.0015465503284260464,0.0016066924221847063
-0.2605171084697353,0.57,0.0,42.0,-0.0004492368458825166,0.0004119535118331316,-0.0008511839077052811,0.0008153292828123254
-0.2605171084697353,0.63,0.0,55.0,-0.0003341887344852829,0.00038768098407886603,-0.0006743688965354472,0.0007270083787679348
-0.2605171084697353,0.69,0.0,54.0,-0.00017395293328945077,0.00021017771912060592,-0.00035125239532826874,0.0004133156029304498
-0.2605171084697353,0.75,0.0,64.0,-0.00015179134946130448,0.00015686716794146985,-0.00031072776449136074,0.00030680179127474163
-0.2605171084697353,0.81,0.0,155.0,-0.00021534566293266813,0.00015915990395087701,-0.00044697070888366237,0.00029901527720872025
-0.2605171084697353,0.87,0.0,70.0,-0.00021093137532267892,0.00019854337237550912,-0.000413011154504926,0.00038413246880481883
-0.3309750919646888,0.39,0.0,9.0,-0.003140639653952147,0.003023417323360503,-0.00606087903481076,0.005841212930494678
-0.3309750919646888,0.45,0.0,19.0,-0.0019316621222344916,0.001731146992903536,-0.0035691025450406227,0.00351376289982361
-0.3309750919646888,0.51,0.0,31.0,-0.0011526452465051673,0.0011157404915720385,-0.0022319817645120557,0.0022001872976923666
-0.3309750919646888,0.57,0.0,47.0,-0.0006104960386082503,0.0005686119798969394,-0.0012179789919614338,0.0011042298880543676
-0.3309750919646888,0.63,0.0,51.0,-0.0004815912590683843,0.00047194508509649515,-0.0009048284554015169,0.0009542080259137615
-0.3309750919646888,0.69,0.0,52.0,-0.0002534673765455757,0.0002559226486597728,-0.0004913220976934569,0.0005277438063205466
-0.3309750919646888,0.75,0.0,66.0,-0.00019875761476632352,0.00018699122272527538,-0.0003856020538231101,0.0003656187904450437
-0.3309750919646888,0.81,0.0,155.0,-0.00023155491766439074,0.0001872432475943191,-0.0004788049475577381,0.0003608340703824873
-0.3309750919646888,0.87,0.0,66.0,-0.00025991798089179593,0.00025067292178453,-0.0005162320178389785,0.0004903204340220818
-0.4204887431174529,0.39,0.0,11.0,-0.0031256314637903453,0.0035775645905443258,-0.005833032008553656,0.007219593193688071
-0.4204887431174529,0.45,0.0,19.0,-0.0025781683426618317,0.00233871876892757,-0.005132762649940785,0.004443146537955792
-0.4204887431174529,0.51,0.0,31.0,-0.0015306895549529983,0.0013789967947905092,-0.002934169180734217,0.0028278514844662242
-0.4204887431174529,0.57,0.0,48.0,-0.0008840960887724186,0.0008412831846673447,-0.001718592760377906,0.0016144627208016502
-0.4204887431174529,0.63,0.0,50.0,-0.0005761230885228891,0.0005750167304567017,-0.0011785838767359692,0.0011453450992751008
-0.4204887431174529,0.69,0.0,50.0,-0.00031855831513255203,0.00032697161184272824,-0.0006256013134783463,0.0006528037031199911
-0.4204887431174529,0.75,0.0,78.0,-0.00022676292654121168,0.00022989169449072022,-0.0004603387067939863,0.00044991027757984055
-0.4204887431174529,0.81,0.0,151.0,-0.00027038796808253175,0.00022613691690864294,-0.0005404860704757706,0.0004227005606683312
-0.4204887431174529,0.87,0.0,59.0,-0.00031512427963597064,0.0002830964836030416,-0.0006354795985797325,0.0005356314097792939
-0.5342117500109752,0.39,0.0,9.0,-0.003533431993171408,0.0038328653115705944,-0.00675511556244114,0.007407520365431713
-0.5342117500109752,0.45,0.0,21.0,-0.002779001073390518,0.002503124450387279,-0.005471366626826465,0.004892441163133933
-0.5342117500109752,0.51,0.0,33.0,-0.0016222861839900143,0.0017024434006837072,-0.0032005024141099404,0.0032888548216130973
-0.5342117500109752,0.57,0.0,47.0,-0.0011727442439312826,0.0011361970599517521,-0.0022491454375873025,0.0022050824345869863
-0.5342117500109752,0.63,0.0,52.0,-0.0006011615704670191,0.0006708058276970163,-0.0011556646050611898,0.0013403552089216177
-0.5342117500109752,0.69,0.0,48.0,-0.00038895156308064885,0.00040004820103079554,-0.0008042154945312651,0.0007549907642266351
-0.5342117500109752,0.75,0.0,105.0,-0.0003818527276837203,0.00031587370044404894,-0.0008292418364593435,0.0005452889326604813
-0.5342117500109752,0.81,0.0,138.0,-0.0002729479850535203,0.0002461698003444744,-0.0005302565085586019,0.0005068146545597839
-0.5342117500109752,0.87,0.0,42.0,-0.0002808712482857991,0.00019935348992323389,-0.0005667275734241611,0.00036867694359973195
-0.6786916380543228,0.39,0.0,8.0,-0.003800239311234535,0.003357022793786704,-0.00714598471927716,0.006603559990852157
-0.6786916380543228,0.45,0.0,28.0,-0.0023443065507847373,0.00242495058280793,-0.00481888614281473,0.004465763739379668
-0.6786916380543228,0.51,0.0,33.0,-0.0018947168090079581,0.0018830202899367576,-0.0036536086769222566,0.0038520774922095415
-0.6786916380543228,0.57,0.0,51.0,-0.0011577145771701073,0.0011338176058808887,-0.0023471394592556967,0.0021629856920678233
-0.6786916380543228,0.63,0.0,46.0,-0.0007853629644109931,0.0007755866318240005,-0.001540585633873444,0.0015810468095891414
-0.6786916380543228,0.69,0.0,51.0,-0.00047375251226593467,0.0004547022221719664,-0.0009412901467818082,0.0009075307984102711
-0.6786916380543228,0.75,0.0,130.0,-0.00042146303848669903,0.0003514022221292113,-0.0008780321323895872,0.000650595347861226
-0.6786916380543228,0.81,0.0,111.0,-0.000306572246332508,0.0003170351206340563,-0.0005952667637584325,0.0006171100342586031
-0.6786916380543228,0.87,0.0,36.0,-0.0001548239959528746,0.00014621263579390928,-0.0003102712064909789,0.0002856170713846469
-0.8622467393414527,0.33,0.0,6.0,-0.003911586542784024,0.003960335949593887,-0.006952610919095434,0.007653128676061274
-0.8622467393414527,0.39,0.0,12.0,-0.0025175359900329033,0.0033623378630443764,-0.004749634585412808,0.007008055498101069
-0.8622467393414527,0.45,0.0,31.0,-0.0023080791034967066,0.0023355462118374837,-0.004860546066163817,0.004442147737020972
-0.8622467393414527,0.51,0.0,27.0,-0.002730856710666338,0.0022540595474475297,-0.005339457662887431,0.004351622944227937
-0.8622467393414527,0.57,0.0,52.0,-0.0013806236331723274,0.0012261279639018535,-0.0028155935400147646,0.0023634727048526846
-0.8622467393414527,0.63,0.0,48.0,-0.0010159518264604255,0.0009886805083668528,-0.001966545617050716,0.0018929560921119863
-0.8622467393414527,0.69,0.0,59.0,-0.0006132180439753745,0.0005493941669168941,-0.0012019745179199244,0.0010975081112454782
-0.8622467393414527,0.75,0.0,132.0,-0.0004773330032597655,0.00041764008445546106,-0.0010372211286484663,0.0007858784626694315
-0.8622467393414527,0.81,0.0,98.0,-0.00041688996554687963,0.00042557117963040573,-0.0008170641805448,0.0008327539411191354
-0.8622467393414527,0.87,0.0,32.0,-0.00020903100562601646,0.000199586735352434,-0.0004092111071077623,0.0003906163746944709
-1.0954451150103377,0.33,0.0,9.0,-0.00323142510692442,0.003331812814196017,-0.006309419686218211,0.006472564468909776
-1.0954451150103377,0.39,0.0,15.0,-0.0025310109664230074,0.0022556560936144907,-0.004960005731144094,0.004327138701197429
-1.0954451150103377,0.45,0.0,35.0,-0.0021122518203651815,0.002160583169764552,-0.004560543950944899,0.0041613762960542216
-1.0954451150103377,0.51,0.0,32.0,-0.0019123432605715873,0.0017982873040505065,-0.004069357697853051,0.0033970584722036274
-1.0954451150103377,0.57,0.0,45.0,-0.0015826190219816003,0.0014485673454200235,-0.0032924746310818266,0.0027108272734750185
-1.0954451150103377,0.63,0.0,51.0,-0.0010367802038163069,0.0010117937835432316,-0.0021319438334886018,0.0019163366927349233
-1.0954451150103377,0.69,0.0,58.0,-0.0006686339359743187,0.0006808469670223982,-0.0012985934125852776,0.0013211320724338185
-1.0954451150103377,0.75,0.0,132.0,-0.0005267765344114072,0.00045343863380183823,-0.0010353460621272202,0.0008775355442190864
-1.0954451150103377,0.81,0.0,93.0,-0.0005633516669075893,0.0005273324985358903,-0.001063040423137346,0.0010599514365340307
-1.0954451150103377,0.87,0.0,26.0,-0.000273950447868202,0.00024029951479775949,-0.0005722354792758819,0.0004667631664202592
-1.391713004234165,0.27,0.0,7.0,-0.002401708000597279,0.0015155516088211085,-0.004995869576499937,0.0027102203632303513
-1.391713004234165,0.33,0.0,13.0,-0.0020577941270343934,0.0019032347196124707,-0.004032961627443978,0.003804417990738143
-1.391713004234165,0.39,0.0,20.0,-0.0014091262753757182,0.0012149043621231851,-0.002706835924802055,0.0024511130066436865
-1.391713004234165,0.45,0.0,37.0,-0.0016103589921449572,0.0013952209902374846,-0.003192025457549801,0.002689404654957238
-1.391713004234165,0.51,0.0,42.0,-0.001105097781650043,0.0012268882886245533,-0.0022079427786298317,0.002409330327430958
-1.391713004234165,0.57,0.0,47.0,-0.0010506773446931415,0.0010771537367577687,-0.002123143908978909,0.002165743829921664
-1.391713004234165,0.63,0.0,33.0,-0.0009703742959782481,0.0009631123347312039,-0.0018624335405990915,0.0018985909655603996
-1.391713004234165,0.69,0.0,65.0,-0.0007435158152060892,0.0007390797957346015,-0.0014335158373960863,0.0014688495652901354
-1.391713004234165,0.75,0.0,114.0,-0.0006068773099049176,0.0005546445511267388,-0.0012567187556676606,0.0010225694548263704
-1.391713004234165,0.81,0.0,98.0,-0.0005914297009944843,0.0005828723340122182,-0.001164494790470801,0.001148377086521687
-1.391713004234165,0.87,0.0,22.0,-0.0005764020788369116,0.00039027544340904336,-0.0012641835340109215,0.0007049150433538917
-1.7681078308849878,0.27,0.0,12.0,-0.0019877734534055934,0.0016762388788895274,-0.004090990348227675,0.0031390906367939914
-1.7681078308849878,0.33,0.0,12.0,-0.0017506210391030979,0.0019601650725512574,-0.003263633476573866,0.003964510785651237
-1.7681078308849878,0.39,0.0,23.0,-0.0013639805956611663,0.001343996792535523,-0.0026379761305398482,0.002703716496902945
-1.7681078308849878,0.45,0.0,39.0,-0.001654280124329411,0.0014105112899437024,-0.003287909431567461,0.0027501966030043404
-1.7681078308849878,0.51,0.0,42.0,-0.001368983994287481,0.0014070230878720528,-0.0025585103569120884,0.0027846287981306466
-1.7681078308849878,0.57,0.0,46.0,-0.0010805185806650047,0.0011308915912997138,-0.002137397099636695,0.0021643702976192635
-1.7681078308849878,0.63,0.0,34.0,-0.0010571124995464693,0.0009590690269331892,-0.0021561671441143056,0.0019440868386764786
-1.7681078308849878,0.69,0.0,63.0,-0.0009265939647333774,0.0008883392771519585,-0.0017503259580225027,0.001822059337685644
-1.7681078308849878,0.75,0.0,118.0,-0.0006618636164152036,0.0006459046864202455,-0.001360851568077366,0.0012145286502228429
-1.7681078308849878,0.81,0.0,91.0,-0.0006491539176137967,0.0006427307806069232,-0.0012985370287815355,0.0012386589847628708
-1.7681078308849878,0.87,0.0,18.0,-0.0006633880105154998,0.0004902742146748837,-0.0013647568443544377,0.0009173870733715425
-2.246300273206917,0.27,0.0,10.0,-0.001323548574937829,0.0012928724295386328,-0.0025642227889451225,0.002538376953739643
-2.246300273206917,0.33,0.0,13.0,-0.002054557539124278,0.0020767413907584295,-0.00415092420216644,0.003887901120336009
-2.246300273206917,0.39,0.0,26.0,-0.0017399146192934019,0.001958659091437712,-0.0034592575305014833,0.003993535800428078
-2.246300273206917,0.45,0.0,32.0,-0.001895162405631814,0.0020550114290973243,-0.0035070141297621994,0.004290553679748222
-2.246300273206917,0.51,0.0,41.0,-0.001831335248096047,0.001843592585250319,-0.00380898029773209,0.0035744051061464732
-2.246300273206917,0.57,0.0,49.0,-0.0019053206124218017,0.0018979539966512949,-0.003727409900541955,0.0035934262013511266
-2.246300273206917,0.63,0.0,54.0,-0.0014979021735091681,0.0014345044443539324,-0.0029982547841262506,0.002846484810261291
-2.246300273206917,0.69,0.0,72.0,-0.0010471712878062811,0.0009892751017187749,-0.001992102961864338,0.002010279352075409
-2.246300273206917,0.75,0.0,119.0,-0.0007570020740122161,0.0007116330794818175,-0.0015163917252018137,0.001432040366236156
-2.246300273206917,0.81,0.0,69.0,-0.0007133328093123951,0.0006420099011951998,-0.0013658063489820908,0.0012923779886621868
-2.246300273206917,0.87,0.0,12.0,-0.0008490743619047631,0.0010135913120011071,-0.0015160060615439818,0.0022316293930709774
-2.8538219384978856,0.21,0.0,5.0,-0.0024891545941875476,0.0034624032956135143,-0.004693305008778248,0.008061966011603116
-2.8538219384978856,0.27,0.0,11.0,-0.001611196443342878,0.0021678471628726846,-0.0030298168785714424,0.00419764598856188
-2.8538219384978856,0.33,0.0,23.0,-0.0016113119807340123,0.0016945642677431245,-0.003169237441157332,0.003256360793101085
-2.8538219384978856,0.39,0.0,29.0,-0.001724559079433922,0.0017645424670036667,-0.0034420013186203385,0.0035357546006652223
-2.8538219384978856,0.45,0.0,41.0,-0.001805736741831331,0.0018566116701802004,-0.00358574688584718,0.0036363132204686624
-2.8538219384978856,0.51,0.0,56.0,-0.0014573354140414935,0.0014464652003786372,-0.0030627061472062937,0.00271705368100161
-2.8538219384978856,0.57,0.0,38.0,-0.0018236107820737578,0.0017684897792598299,-0.003433696582430078,0.0036056653412138632
-2.8538219384978856,0.63,0.0,59.0,-0.001161141816765741,0.0012303142048689986,-0.0024251734182702224,0.0023292672224012466
-2.8538219384978856,0.69,0.0,76.0,-0.0011648671081873592,0.0011696675782143715,-0.0022557191019642597,0.0022630215558972658
-2.8538219384978856,0.75,0.0,108.0,-0.0008148642813210269,0.0007814014885687315,-0.0016513952802787147,0.0015416491230685822
-2.8538219384978856,0.81,0.0,52.0,-0.0008114090882046681,0.000736725322499965,-0.0015915367064274753,0.001426168102992548
-3.625650476828128,0.21,0.0,11.0,-0.0019807039105382293,0.0016269885733515,-0.003976701932524854,0.0029898998600313017
-3.625650476828128,0.27,0.0,18.0,-0.0016437335902701905,0.0015959662079008021,-0.003199470688465396,0.0032025032821004634
-3.625650476828128,0.33,0.0,32.0,-0.0015794724450488675,0.0016350156541848184,-0.002973754495197422,0.0032890504314480595
-3.625650476828128,0.39,0.0,46.0,-0.0014407191246648171,0.0012946657365335667,-0.0027914287523657993,0.00254450785110286
-3.625650476828128,0.45,0.0,52.0,-0.0013050109634824357,0.0013367182243175563,-0.002586932880982448,0.0026736565265704348
-3.625650476828128,0.51,0.0,39.0,-0.001747093930076076,0.0017944674759758708,-0.0034215507443235305,0.0034369968899053745
-3.625650476828128,0.57,0.0,48.0,-0.0015053048620830298,0.0016080252183866643,-0.0031652987728027888,0.003099103923227719
-3.625650476828128,0.63,0.0,44.0,-0.0018449932436984129,0.0018746876472389947,-0.0037745610176396402,0.003690340580354231
-3.625650476828128,0.69,0.0,87.0,-0.0012929297039987278,0.0011700820716867488,-0.0025239541576488602,0.002388391141579603
-3.625650476828128,0.75,0.0,97.0,-0.0009869184739242577,0.0010111607744536278,-0.0019512555624322113,0.001913555406459839
-3.625650476828128,0.81,0.0,23.0,-0.0014244884841039555,0.0015192536866029092,-0.002927452764562414,0.0028364499696328553
-4.606223395648532,0.21,0.0,13.0,-0.0029520282385646374,0.002430764782074033,-0.005993332074924872,0.004485770293649005
-4.606223395648532,0.27,0.0,30.0,-0.001763450771778005,0.0018573462404879477,-0.00370206338396503,0.0035230075770177963
-4.606223395648532,0.33,0.0,43.0,-0.0018225553012305015,0.0017790619456575917,-0.0033260490745199364,0.0037180855020862514
-4.606223395648532,0.39,0.0,52.0,-0.001795530790036036,0.0016942598037541418,-0.003550288627239436,0.00331859657214071
-4.606223395648532,0.45,0.0,39.0,-0.0024430671617909107,0.002173085095143948,-0.004778636643754599,0.0042527533741641265
-4.606223395648532,0.51,0.0,42.0,-0.0026521069777268634,0.0022835386989233162,-0.005219783961714628,0.004437937365457433
-4.606223395648532,0.57,0.0,49.0,-0.0026740561379352203,0.002544446136687555,-0.005462682782872515,0.004829297919158468
-4.606223395648532,0.63,0.0,49.0,-0.0023017253035843475,0.0019600736068823227,-0.0045034297113419695,0.0038443778749523627
-4.606223395648532,0.69,0.0,104.0,-0.0015495169581667034,0.0015217746533018445,-0.0030851302379277684,0.0029626385826028536
-4.606223395648532,0.75,0.0,63.0,-0.0018288579102029578,0.001668278032355245,-0.0034252472152924702,0.0034518070601904775
-4.606223395648532,0.81,0.0,12.0,-0.0027503292971754792,0.002725061549724367,-0.005397072170545714,0.0053552623656540595
-5.851996519306439,0.15,0.0,9.0,-0.004819941340114638,0.004652358212435599,-0.009132692589028105,0.009571028713184786
-5.851996519306439,0.21,0.0,26.0,-0.0023433345527410485,0.00256651343272587,-0.004696018288628838,0.005016499143080822
-5.851996519306439,0.27,0.0,32.0,-0.0022626602987053197,0.002664026640448641,-0.004352215582688817,0.005316929396294131
-5.851996519306439,0.33,0.0,64.0,-0.0018881790323805635,0.0016664093677827298,-0.0036152267478310415,0.0032600280494894567
-5.851996519306439,0.39,0.0,48.0,-0.0028054715902510845,0.0022406846572759894,-0.005483102963338622,0.004463808499941132
-5.851996519306439,0.45,0.0,51.0,-0.003637478609043876,0.003336807712355246,-0.007019175828033875,0.006482543015020354
-5.851996519306439,0.51,0.0,41.0,-0.003929444571923725,0.0032331794313225277,-0.008114525176594483,0.005975864381298692
-5.851996519306439,0.57,0.0,44.0,-0.0032547422743211514,0.0028200792566826526,-0.007031822081092163,0.005125509346657147
-5.851996519306439,0.63,0.0,68.0,-0.002427454950247704,0.002150726453481826,-0.004845666761330982,0.004225236997450062
-5.851996519306439,0.69,0.0,84.0,-0.002265281596001418,0.0021940210110237765,-0.004510055196455961,0.004151744961370587
-5.851996519306439,0.75,0.0,30.0,-0.0026897988016928785,0.0031459437774581213,-0.005157749082557539,0.006384009114203119
-7.434694395049634,0.15,0.0,14.0,-0.003934225891631122,0.004679280869368987,-0.007220369828378501,0.009463586376321616
-7.434694395049634,0.21,0.0,31.0,-0.002241819579053767,0.0023178503398003435,-0.004549361147800602,0.004297934433223997
-7.434694395049634,0.27,0.0,47.0,-0.002341372186339653,0.0025249958820790274,-0.004604275485604637,0.004848138882502935
-7.434694395049634,0.33,0.0,56.0,-0.002035485154884094,0.002078292463479471,-0.004058103013336803,0.003943316571321124
-7.434694395049634,0.39,0.0,69.0,-0.0027643391047832734,0.0026111738772809793,-0.005564156803427623,0.005064706600912046
-7.434694395049634,0.45,0.0,48.0,-0.0035382271897290997,0.0033351406432085094,-0.007203101392640966,0.006626288675556997
-7.434694395049634,0.51,0.0,49.0,-0.0030277084219747846,0.0025502219154183918,-0.0063277719010856725,0.004641650716498966
-7.434694395049634,0.57,0.0,55.0,-0.0029825314246015745,0.0026027673683476386,-0.005676951212815989,0.005045761228393264
-7.434694395049634,0.63,0.0,71.0,-0.002983153492658353,0.0029370069537338855,-0.006002184072738111,0.005389968850004866
-7.434694395049634,0.69,0.0,51.0,-0.0032116079517582907,0.0035039119897161447,-0.006534770305648498,0.006838774468317823
-7.434694395049634,0.75,0.0,8.0,-0.0036610435278431608,0.0042770865008649435,-0.007610188897606639,0.007961960632405785
-9.445439785451782,0.15,0.0,17.0,-0.004324687566128243,0.004065755166896384,-0.00867053725171039,0.007577863062407754
-9.445439785451782,0.21,0.0,42.0,-0.0029432766067810537,0.0031459604994511056,-0.00581859540490032,0.005946198564854722
-9.445439785451782,0.27,0.0,59.0,-0.002850084632609117,0.002861583876384967,-0.00549874121562468,0.005589959089230548
-9.445439785451782,0.33,0.0,80.0,-0.002896376270246987,0.0029625678454928387,-0.005650746444229173,0.005862433188981341
-9.445439785451782,0.39,0.0,60.0,-0.003496563273803083,0.003083378865529547,-0.006936091986338944,0.006270447577523133
-9.445439785451782,0.45,0.0,55.0,-0.003565782322278357,0.0030623038455190447,-0.0071602435783851125,0.005913729119893229
-9.445439785451782,0.51,0.0,44.0,-0.0034315170100522705,0.0031097806565444485,-0.0068379394702544624,0.005888481564828958
-9.445439785451782,0.57,0.0,64.0,-0.003936543828283022,0.0038688937878259906,-0.007782270766344275,0.007434583894969077
-9.445439785451782,0.63,0.0,54.0,-0.004014798357096584,0.003868073800594708,-0.00792438930745846,0.00769730366576486
-9.445439785451782,0.69,0.0,19.0,-0.006779230797590744,0.0070724872848258735,-0.01284762733054647,0.013886079666352098
-11.999999999999996,0.15,0.0,19.0,-0.003904334663076994,0.003996043932125316,-0.008107419772318618,0.0075135354728172775
-11.999999999999996,0.21,0.0,39.0,-0.0035501167989552525,0.0037926167229536873,-0.006879275815570296,0.0072477233474092006
-11.999999999999996,0.27,0.0,73.0,-0.0033610202754501685,0.0035389853787252353,-0.006404949706492687,0.006855192231679692
-11.999999999999996,0.33,0.0,86.0,-0.003323338736005365,0.0032999595838690814,-0.006374843955519737,0.0064106410421703635
-11.999999999999996,0.39,0.0,68.0,-0.0038665934837870414,0.0033662828233066208,-0.007529724246696174,0.006783580504122022
-11.999999999999996,0.45,0.0,58.0,-0.0035398162394626605,0.0033864146124854473,-0.007531864867153225,0.006141049410132631
-11.999999999999996,0.51,0.0,52.0,-0.005554121577040095,0.004477050268301352,-0.010491773127148237,0.008817067984910486
-11.999999999999996,0.57,0.0,51.0,-0.0064655104701155375,0.006144474448776219,-0.012903171710288897,0.01171863642873793
-11.999999999999996,0.63,0.0,34.0,-0.008031845174289514,0.007290698596847901,-0.015222414758542182,0.014929543966309996
-11.999999999999996,0.69,0.0,13.0,-0.012197829705362895,0.012926151619106492,-0.024302782613174846,0.025326538335222325
-0.100000000000002,0.33,0.125,8.0,-0.00023727921526868343,0.0002320805731405029,-0.0004697222481034463,0.00043811955096688393
-0.100000000000002,0.39,0.125,11.0,-0.0001011851452554791,0.00010992857658626865,-0.00019519939151196444,0.00021399760199185126
-0.100000000000002,0.45,0.125,16.0,-8.148994978025067e-05,9.227504263746349e-05,-0.00015630355061084722,0.00018714337369029523
-0.100000000000002,0.51,0.125,31.0,-0.00013633146167691526,0.00019081710355075957,-0.0002453290170979788,0.00041869448316471267
-0.100000000000002,0.57,0.125,43.0,-0.0001292947699970076,0.00016325548059375827,-0.0002360452872471047,0.0003358163524496571
-0.100000000000002,0.63,0.125,48.0,-0.00010302581061085468,0.000124112271530957,-0.00018591223672861188,0.00027205837745878617
-0.100000000000002,0.69,0.125,55.0,-7.580868776195388e-05,0.00010126595227786172,-0.0001405161412878901,0.00020765963698785508
-0.100000000000002,0.75,0.125,112.0,-6.372374084724604e-05,7.097760644927027e-05,-0.00012041132231449428,0.00014671336663029384
-0.100000000000002,0.81,0.125,136.0,-6.532066731585041e-05,7.081810873335756e-05,-0.00012130437941890722,0.00014202351173373575
-0.100000000000002,0.87,0.125,38.0,-0.00010877329216118522,5.32968980292236e-05,-0.00023095553491227593,5.871497816462242e-05
-0.1270454343320575,0.33,0.125,9.0,-0.00038407155169848105,0.00042261839122588696,-0.0007437565528086976,0.0008084869256848653
-0.1270454343320575,0.39,0.125,11.0,-0.00015852927183589283,0.00016754410804807173,-0.00030932027434491357,0.0003169890131889874
-0.1270454343320575,0.45,0.125,19.0,-0.00015808857483082305,0.0002715814714211718,-0.0003059433192787955,0.0005950622025009788
-0.1270454343320575,0.51,0.125,27.0,-0.00015814871635026767,0.000237606613665421,-0.00030211426019861176,0.0005062369754507797
-0.1270454343320575,0.57,0.125,45.0,-0.00015071565743182954,0.0001844395182044055,-0.0002922498500878156,0.000368226300764915
-0.1270454343320575,0.63,0.125,51.0,-0.00010924549472510706,0.00014826944046191103,-0.00020657050674639606,0.00029324292843072925
-0.1270454343320575,0.69,0.125,56.0,-7.888075177248598e-05,0.00011413084015596114,-0.0001535918733492329,0.00022351409506407956
-0.1270454343320575,0.75,0.125,108.0,-6.81491953523359e-05,7.268936084317516e-05,-0.00012790379161102208,0.0001513572554339608
-0.1270454343320575,0.81,0.125,136.0,-6.569061694350357e-05,7.428664879057687e-05,-0.00012527249412992497,0.00014679961843692307
-0.1270454343320575,0.87,0.125,36.0,-0.00011765190563843721,5.889939620632892e-05,-0.00025170300474466477,6.63809189692833e-05
-0.1614054238462049,0.33,0.125,9.0,-0.0007327032056285841,0.0007174755848309043,-0.0014227565911159774,0.001414618227269294
-0.1614054238462049,0.39,0.125,11.0,-0.0002566313554349997,0.0002781072415974894,-0.0004690487784247649,0.0005470906524988958
-0.1614054238462049,0.45,0.125,19.0,-0.00025532627238322963,0.0003379353472060045,-0.0005049891994009467,0.000746474136075059
-0.1614054238462049,0.51,0.125,31.0,-0.0002483533855910458,0.0002925087112637515,-0.0004458281078008293,0.0006202719273946227
-0.1614054238462049,0.57,0.125,48.0,-0.0001644982906611477,0.00021358131995262306,-0.0003203123471122952,0.0004203151414196453
-0.1614054238462049,0.63,0.125,48.0,-0.0001527217224198153,0.00019596981532844633,-0.00028587710845969313,0.00038117988719342164
-0.1614054238462049,0.69,0.125,53.0,-0.00011070178872878042,0.00013028929855508106,-0.00020256294983398785,0.00026845838429547496
-0.1614054238462049,0.75,0.125,111.0,-7.93530803921437e-05,8.133310949737794e-05,-0.00015930716414584362,0.00015987953239857423
-0.1614054238462049,0.81,0.125,133.0,-7.237028589545922e-05,8.093027051547478e-05,-0.00013989062274092503,0.00016015263553066447
-0.1614054238462049,0.87,0.125,35.0,-1.1514560823618324e-05,1.0742225584259905e-05,-2.2540708171389813e-05,2.0823546704746703e-05
-0.2050582217609075,0.33,0.125,9.0,-0.0012498836005360601,0.0011993095483858014,-0.002488276050370458,0.002234582926880888
-0.2050582217609075,0.39,0.125,14.0,-0.00037025152791687925,0.0004111513959472587,-0.0007403138732722226,0.0007953809464199009
-0.2050582217609075,0.45,0.125,20.0,-0.0004819568703838787,0.0005595353832801656,-0.000960073617889469,0.001087177179679424
-0.2050582217609075,0.51,0.125,32.0,-0.00032479421770374993,0.0004228499934690648,-0.00059982285572233,0.0008417426287078733
-0.2050582217609075,0.57,0.125,44.0,-0.00023965933177409851,0.0002963141166151376,-0.0004601483046948559,0.000599920259888355
-0.2050582217609075,0.63,0.125,53.0,-0.0002146259244469206,0.00025595679127941943,-0.00039700834088290244,0.0005114652939607067
-0.2050582217609075,0.69,0.125,49.0,-0.00014696110452519032,0.00017754387940300496,-0.00026807967940368306,0.0003673314031740574
-0.2050582217609075,0.75,0.125,114.0,-0.0001168669667608931,0.00010561701849842579,-0.00022884749095065994,0.00021088161236886924
-0.2050582217609075,0.81,0.125,129.0,-9.475450641488582e-05,0.0001016927559845838,-0.000176639722308393,0.0001996817550122136
-0.2050582217609075,0.87,0.125,34.0,-2.1198738658977343e-05,2.0915230745827484e-05,-4.399655604524124e-05,4.0221418908464544e-05
-0.2605171084697381,0.33,0.125,10.0,-0.0016904613975326972,0.0015721101551715473,-0.003233951019614547,0.0029052193053457527
-0.2605171084697381,0.39,0.125,15.0,-0.0005309937937538736,0.0005623499778554753,-0.0009881934108313052,0.0011509905720600878
-0.2605171084697381,0.45,0.125,21.0,-0.0006369663494981584,0.000708463381136672,-0.0012064105614995062,0.0013843038143873017
-0.2605171084697381,0.51,0.125,32.0,-0.0004504380606727588,0.0005317261529535551,-0.0008522925618615142,0.00109320499313202
-0.2605171084697381,0.57,0.125,47.0,-0.00031032019134435133,0.0003813587347655718,-0.0006021183367965686,0.0007319385744953417
-0.2605171084697381,0.63,0.125,51.0,-0.0002658758200553217,0.00030129548267720526,-0.0004929196076904993,0.000605361439763341
-0.2605171084697381,0.69,0.125,46.0,-0.00017969430693806648,0.00022477948879997913,-0.000358949581935787,0.0004477937841985964
-0.2605171084697381,0.75,0.125,116.0,-0.00015597945139482667,0.00012977740716183067,-0.00032719511401090495,0.00024166924658565345
-0.2605171084697381,0.81,0.125,127.0,-0.00011040059376546915,0.00010793337229114527,-0.00020524778638547178,0.0002289296052781302
-0.2605171084697381,0.87,0.125,33.0,-3.043470861952865e-05,2.8913336882248384e-05,-6.0056121499501854e-05,5.4751092235144034e-05
-0.3309750919646826,0.33,0.125,10.0,-0.0019835629306031053,0.0018680082599240916,-0.004012667777908677,0.003436841136542621
-0.3309750919646826,0.39,0.125,17.0,-0.0008526654343597286,0.0007350755595644063,-0.0016752036177202915,0.0014278384494119426
-0.3309750919646826,0.45,0.125,22.0,-0.0007251530758299986,0.0008829161200087659,-0.0014255455519116005,0.00169494018407678
-0.3309750919646826,0.51,0.125,34.0,-0.000578400635047687,0.0006379761012531134,-0.0010862203328589094,0.0013525450806618764
-0.3309750919646826,0.57,0.125,47.0,-0.00045054933038651926,0.0004961793064504409,-0.0008533433708079184,0.0010193344324037673
-0.3309750919646826,0.63,0.125,50.0,-0.00033199095701356177,0.00037730003964772755,-0.0006263669158683801,0.0007726960394708654
-0.3309750919646826,0.69,0.125,46.0,-0.00025784255416483873,0.0002842738612565876,-0.0004822180681877564,0.000593001807954994
-0.3309750919646826,0.75,0.125,113.0,-0.0001842187869996712,0.00016486589914537037,-0.00038726891366977517,0.0003176474051056823
-0.3309750919646826,0.81,0.125,126.0,-0.00013464057136225793,0.00013620454646156189,-0.00025431381158025373,0.0002728877595376375
-0.3309750919646826,0.87,0.125,32.0,-4.223894018914021e-05,3.787599129812965e-05,-8.447631692695184e-05,7.356263489623087e-05
-0.4204887431174625,0.33,0.125,11.0,-0.002060559760074463,0.0017307778037641626,-0.004327060645708493,0.0032712382542615685
-0.4204887431174625,0.39,0.125,17.0,-0.0008990357499650382,0.0008070651668647403,-0.0017971817432738343,0.001623115001206424
-0.4204887431174625,0.45,0.125,26.0,-0.0009743241670587594,0.0010952219376934094,-0.0017972835348050741,0.0022364554437782
-0.4204887431174625,0.51,0.125,40.0,-0.0006222760147085071,0.0007368200972210083,-0.001197522054561855,0.0015256328895704454
-0.4204887431174625,0.57,0.125,43.0,-0.0006217439665686847,0.0006973428769927144,-0.0012022247678477277,0.0014659198950378789
-0.4204887431174625,0.63,0.125,48.0,-0.0004453948146871643,0.0004855236769189184,-0.0008734145705513133,0.0009782829726446382
-0.4204887431174625,0.69,0.125,46.0,-0.0003266011316747427,0.00037585073162827056,-0.0006327230676324726,0.0007079283905554063
-0.4204887431174625,0.75,0.125,97.0,-0.0002702487493127843,0.00023915433937604769,-0.0005635783881446343,0.0004578401001351239
-0.4204887431174625,0.81,0.125,138.0,-0.00015834842179530173,0.00016946086998780315,-0.00031222369878536587,0.00032567916972028996
-0.4204887431174625,0.87,0.125,30.0,-0.00021111471118736124,0.00010947591294218025,-0.0005202056316337788,0.00017937641100566407
-0.5342117500109698,0.33,0.125,14.0,-0.0015084030145588597,0.0013096454554339823,-0.003100941069299153,0.0024084935816362546
-0.5342117500109698,0.39,0.125,20.0,-0.0009684901253168201,0.0010074201450834997,-0.001989268638934005,0.001995647212003356
-0.5342117500109698,0.45,0.125,29.0,-0.0013011196949612813,0.0014376702764952864,-0.0024474364240289134,0.0028781067413792493
-0.5342117500109698,0.51,0.125,42.0,-0.0009168571771124596,0.000952327678587255,-0.001736784366791465,0.0019349329694566845
-0.5342117500109698,0.57,0.125,38.0,-0.0007769881368653675,0.0008475344521847472,-0.0015090386224194945,0.0017198860135983118
-0.5342117500109698,0.63,0.125,43.0,-0.0005864361025471026,0.0006461168789014069,-0.0011216942854254397,0.001337076873444749
-0.5342117500109698,0.69,0.125,50.0,-0.0004396532600990641,0.0004595883420372929,-0.0008244464981980856,0.0009719489720445676
-0.5342117500109698,0.75,0.125,91.0,-0.00037705241383806685,0.0003407129237769668,-0.0007818426450293866,0.0006573675588972915
-0.5342117500109698,0.81,0.125,143.0,-0.00021187749822672397,0.00021572857684690848,-0.0004231981162818035,0.00043612087373541986
-0.5342117500109698,0.87,0.125,25.0,-0.000327027033520898,0.00019027303260779767,-0.0007870131906083221,0.00031195659555283866
-0.6786916380543185,0.27,0.125,7.0,-0.0034959903764387097,0.003121121596272183,-0.006606829264450299,0.006130814032630176
-0.6786916380543185,0.33,0.125,11.0,-0.0013816521341267374,0.001450328043896092,-0.0024805144773502176,0.0030225468611177393
-0.6786916380543185,0.39,0.125,19.0,-0.001477528685450952,0.0014089230760418565,-0.0029672752921805204,0.0026911366342521636
-0.6786916380543185,0.45,0.125,37.0,-0.0015427224118916638,0.0014227800703340218,-0.003068214605285986,0.002904418313101036
-0.6786916380543185,0.51,0.125,38.0,-0.0010754153835526314,0.001202795038794537,-0.0021313922463761484,0.0022697888398153293
-0.6786916380543185,0.57,0.125,42.0,-0.0009085367906974765,0.0009270210685184516,-0.0017235766813324073,0.0019567031289206074
-0.6786916380543185,0.63,0.125,42.0,-0.0007398167774701853,0.0008013544037377288,-0.0014562874762368088,0.0015649252582888831
-0.6786916380543185,0.69,0.125,48.0,-0.0005698108509346392,0.0005506638986688538,-0.0011275590140858406,0.0011032330278126954
-0.6786916380543185,0.75,0.125,83.0,-0.0005067640382064503,0.0004466289375215781,-0.0010209754338844949,0.0008636714513869486
-0.6786916380543185,0.81,0.125,147.0,-0.0002782278002757623,0.0002982550574925591,-0.0005619876427325753,0.000575333513623209
-0.6786916380543185,0.87,0.125,24.0,-0.000628310874467378,0.0004750647645382641,-0.0013660521831352428,0.0008597326920092844
-0.8622467393414444,0.27,0.125,8.0,-0.0035436132152756455,0.003279227565745335,-0.00692780542771565,0.0062172581101715895
-0.8622467393414444,0.33,0.125,15.0,-0.0015013521241159214,0.0016629031779089953,-0.0028347872205824326,0.003570973562944857
-0.8622467393414444,0.39,0.125,18.0,-0.0020399302367642954,0.001501383855659044,-0.004321680816142645,0.002763279901281396
-0.8622467393414444,0.45,0.125,42.0,-0.0017895621967906317,0.0016229600057712122,-0.0036835750474536627,0.0032019619653112985
-0.8622467393414444,0.51,0.125,34.0,-0.0012727952923652984,0.0012122339670473034,-0.0024028372804941484,0.0024814556435877907
-0.8622467393414444,0.57,0.125,42.0,-0.0011697463717355075,0.0012013186067803016,-0.00231714635738266,0.0023168079944802006
-0.8622467393414444,0.63,0.125,43.0,-0.0008097978511629098,0.0007929903837845784,-0.0015960756810287507,0.0015560040724684654
-0.8622467393414444,0.69,0.125,47.0,-0.0007339106431553621,0.0007514368473905868,-0.0014699439113703445,0.0014279140228828356
-0.8622467393414444,0.75,0.125,78.0,-0.0005582454775488743,0.0005423059167431013,-0.0010879271673146771,0.001051304386584149
-0.8622467393414444,0.81,0.125,148.0,-0.00042314961155266484,0.00041806542131719355,-0.000862026955196377,0.0008131345993544481
-0.8622467393414444,0.87,0.125,22.0,-0.0010252217965391526,0.0008911376448334225,-0.0020049683129682696,0.0016716472545050224
-1.0954451150103266,0.27,0.125,7.0,-0.001982039893568298,0.0020364610674011843,-0.003734449769411593,0.004009770816974194
-1.0954451150103266,0.33,0.125,16.0,-0.0019849490470803624,0.002030768361823528,-0.003815525908137261,0.004110246187862688
-1.0954451150103266,0.39,0.125,16.0,-0.0020369209485194832,0.0015388208259711938,-0.004423188082211175,0.0028169492138858192
-1.0954451150103266,0.45,0.125,39.0,-0.001910785033948868,0.001887042902909382,-0.003826943086423265,0.003558433571116189
-1.0954451150103266,0.51,0.125,40.0,-0.0012891549156068198,0.0013396195068130742,-0.002445519407910355,0.002740701192722749
-1.0954451150103266,0.57,0.125,40.0,-0.0013081791299394553,0.001400575968269411,-0.002668532084141092,0.0027788736646158574
-1.0954451150103266,0.63,0.125,42.0,-0.0009705402139486207,0.000986332068376482,-0.0019645106215516513,0.002071037175148026
-1.0954451150103266,0.69,0.125,50.0,-0.0009497703143408874,0.0009699150060206299,-0.0018565112952148393,0.0019030593296641839
-1.0954451150103266,0.75,0.125,86.0,-0.0005964553744322949,0.0005864361123263131,-0.0011751374742370478,0.001146642989780597
-1.0954451150103266,0.81,0.125,142.0,-0.000580562848572366,0.000572602008914684,-0.0011429334911042712,0.0011319959523173908
-1.0954451150103266,0.87,0.125,19.0,-0.001307216526975015,0.001157662743581486,-0.0027720285828153795,0.002071344803266832
-1.391713004234164,0.27,0.125,8.0,-0.0017817347046684248,0.0014811286551011382,-0.0034198284483364094,0.00288270432600804
-1.391713004234164,0.33,0.125,15.0,-0.0032374563694522337,0.003006683051505682,-0.006241550709624142,0.006134527946595666
-1.391713004234164,0.39,0.125,20.0,-0.0021207301087720087,0.0023510164181887337,-0.0039037227836788285,0.0047639949500316026
-1.391713004234164,0.45,0.125,32.0,-0.001737409716302255,0.0018232670404159893,-0.0034436219656897617,0.0035366687131270294
-1.391713004234164,0.51,0.125,42.0,-0.0014354879437762666,0.0015517190806572626,-0.002771705386808924,0.003129478147257376
-1.391713004234164,0.57,0.125,38.0,-0.0016313135474198565,0.0016896363133082951,-0.0032489001066868966,0.003423996325956482
-1.391713004234164,0.63,0.125,41.0,-0.0012336348018883835,0.001260489911522501,-0.002320538278727938,0.0025014809138628733
-1.391713004234164,0.69,0.125,62.0,-0.0009699621884270084,0.0010339962163995171,-0.001953202788175262,0.0019351616758747456
-1.391713004234164,0.75,0.125,117.0,-0.0006816931221467811,0.0006321103117151303,-0.0012779334033016345,0.0012522587788825197
-1.391713004234164,0.81,0.125,109.0,-0.0007186979128880497,0.000677543904928632,-0.0014191648165727704,0.00131332359288019
-1.391713004234164,0.87,0.125,14.0,-0.0015079705228125267,0.0009696134895775967,-0.0029627874496644903,0.0018129514796638914
-1.7681078308849842,0.27,0.125,7.0,-0.0029485665076973222,0.0029861076301287742,-0.00563250121913328,0.0056831658602547455
-1.7681078308849842,0.33,0.125,16.0,-0.003817025578140989,0.003950106609365124,-0.008034904317811236,0.007644834333102975
-1.7681078308849842,0.39,0.125,19.0,-0.002205710808037764,0.0023720710616632903,-0.004332340953149791,0.004472766584924417
-1.7681078308849842,0.45,0.125,40.0,-0.0016450723729277837,0.001933899494376827,-0.0032130168831608387,0.003805766165298695
-1.7681078308849842,0.51,0.125,32.0,-0.0019404854948173787,0.0019558740091086243,-0.003897218644544042,0.0038380368657274294
-1.7681078308849842,0.57,0.125,40.0,-0.0019306729264795788,0.0019247055118608732,-0.003755834117616211,0.0039031507203476775
-1.7681078308849842,0.63,0.125,47.0,-0.001578922714793457,0.001633348796185788,-0.0030030159919643674,0.0031940403980534092
-1.7681078308849842,0.69,0.125,67.0,-0.0012379224073225715,0.0011928040606752539,-0.0023266064443741644,0.0024778693506287753
-1.7681078308849842,0.75,0.125,135.0,-0.0007512023444740282,0.0007454548859445845,-0.001521667793959018,0.001400143243365575
-1.7681078308849842,0.81,0.125,87.0,-0.0008644038722447202,0.0007990471844867167,-0.0016925575129922619,0.0016117418925198047
-1.7681078308849842,0.87,0.125,7.0,-0.0009715327229689993,0.0007596685075797868,-0.002003350808171251,0.0013885426150753246
-2.2463002732069244,0.27,0.125,12.0,-0.002262018623803601,0.0021930073813763375,-0.0042432417847578195,0.004191578736730663
-2.2463002732069244,0.33,0.125,21.0,-0.0015018933362075592,0.0016807914845537032,-0.002917081387314986,0.0033997347060691426
-2.2463002732069244,0.39,0.125,27.0,-0.0014787190503055534,0.001329207928801889,-0.003014632393713709,0.0026008069610769773
-2.2463002732069244,0.45,0.125,38.0,-0.0014511542824561863,0.0016557903613573016,-0.0028882648326231026,0.003250680833002537
-2.2463002732069244,0.51,0.125,52.0,-0.0012623221416441794,0.0013187418525869954,-0.0024212636609755598,0.002647699411194378
-2.2463002732069244,0.57,0.125,46.0,-0.0012547843190645696,0.0012461899549464622,-0.002535987537280249,0.002347236622938214
-2.2463002732069244,0.63,0.125,51.0,-0.0010554797911780144,0.001059183426484102,-0.002145591266877621,0.0020183505910516993
-2.2463002732069244,0.69,0.125,76.0,-0.0010354747700414327,0.000998056362621799,-0.0020804166705971207,0.0019806877045831024
-2.2463002732069244,0.75,0.125,116.0,-0.000789820118137122,0.0007703351968290347,-0.0015481032254971152,0.0015338961755584943
-2.2463002732069244,0.81,0.125,54.0,-0.000890479207448297,0.0008632691987956592,-0.0018019861999578675,0.0016993748682068049
-2.853821938497883,0.21,0.125,9.0,-0.002098239940378354,0.0016685066175015132,-0.0043423759461619854,0.0030885667629686614
-2.853821938497883,0.27,0.125,17.0,-0.001806252700090362,0.0016968368981906587,-0.0036374632284709744,0.0034234406825102014
-2.853821938497883,0.33,0.125,27.0,-0.0013149855964029323,0.0012570943594022337,-0.0025736353836916938,0.0024971300549814493
-2.853821938497883,0.39,0.125,35.0,-0.0011247678053945282,0.001200256298813627,-0.0022076217039773373,0.0023290525009495803
-2.853821938497883,0.45,0.125,58.0,-0.0010501988423054416,0.0010864513099142013,-0.0020727502773031686,0.002109123704956611
-2.853821938497883,0.51,0.125,43.0,-0.0011625948419663223,0.0011658621316372358,-0.0022864020960210534,0.002258407546046973
-2.853821938497883,0.57,0.125,42.0,-0.001333253089423705,0.0012516118085369146,-0.002911748975526841,0.002352817995633455
-2.853821938497883,0.63,0.125,42.0,-0.0018204076081319244,0.00164061619780394,-0.0036186437378419698,0.003111719678993964
-2.853821938497883,0.69,0.125,73.0,-0.001219150347245206,0.0011532260555145,-0.002474901447004283,0.0022164549532810497
-2.853821938497883,0.75,0.125,117.0,-0.0009127113648049274,0.0008165398497245714,-0.0018372576693993195,0.0016067724513136865
-2.853821938497883,0.81,0.125,35.0,-0.001001526118734964,0.0010398834953279966,-0.0020567917030069184,0.0020384227878579744
-3.625650476828122,0.21,0.125,13.0,-0.0024286748840924846,0.0015508421531399952,-0.005029794091038424,0.0030350279658593834
-3.625650476828122,0.27,0.125,23.0,-0.001911337880415234,0.0020763713909101185,-0.0037736517831690316,0.004193079806759458
-3.625650476828122,0.33,0.125,35.0,-0.00148730152184431,0.0015776313006137259,-0.002849297549404082,0.003120755288897244
-3.625650476828122,0.39,0.125,46.0,-0.0013462248352123134,0.0013445388367040085,-0.002766800469899283,0.002597489785020347
-3.625650476828122,0.45,0.125,41.0,-0.001499619749356542,0.0014955672276778134,-0.0030765496047372226,0.0030352663525566865
-3.625650476828122,0.51,0.125,49.0,-0.0015734586832845164,0.0014555479172528615,-0.003113576534126672,0.0027997003736564786
-3.625650476828122,0.57,0.125,40.0,-0.0021221194452560907,0.0017239624701116851,-0.004094608381987668,0.0033804229953105025
-3.625650476828122,0.63,0.125,41.0,-0.002249591241817775,0.0022864466628309717,-0.004502776194073761,0.004264657517035916
-3.625650476828122,0.69,0.125,61.0,-0.0014534418305337353,0.0014917305077138108,-0.0030136769953156214,0.0027574026839102925
-3.625650476828122,0.75,0.125,125.0,-0.0009050869193593971,0.0008887187845080476,-0.0017109668724242478,0.0017107664518005267
-3.625650476828122,0.81,0.125,24.0,-0.0014492112705391887,0.0014596608012730544,-0.0027379612740356715,0.0029263024360484495
-4.606223395648536,0.21,0.125,13.0,-0.0024838798035170025,0.0025743067637580136,-0.004837558783103735,0.005050145969459663
-4.606223395648536,0.27,0.125,33.0,-0.001961737208576265,0.0020081337862794236,-0.0037221664257817326,0.0039057853167201663
-4.606223395648536,0.33,0.125,47.0,-0.0018512285968052225,0.0017407424559960818,-0.0036157000017259786,0.0032402354197607645
-4.606223395648536,0.39,0.125,50.0,-0.00167664802155349,0.001767643219867356,-0.003162719917394944,0.0034750809686404076
-4.606223395648536,0.45,0.125,54.0,-0.0017072705601062007,0.0015412359322767295,-0.003179884915791671,0.0031147741783851086
-4.606223395648536,0.51,0.125,44.0,-0.0023112059111019207,0.0023069719348245967,-0.004914713017251684,0.004200148245625333
-4.606223395648536,0.57,0.125,42.0,-0.0025024344757327323,0.0024155485544974952,-0.005206388169379933,0.004614708553078134
-4.606223395648536,0.63,0.125,46.0,-0.0024003087243187633,0.00222754472570357,-0.005112276424831559,0.004250204205674557
-4.606223395648536,0.69,0.125,101.0,-0.001322893653712065,0.001325007916004752,-0.0027050500400526557,0.0026326104474079697
-4.606223395648536,0.75,0.125,56.0,-0.0015613312906439685,0.0015593363446651434,-0.0030251916482021374,0.0030873216191365863
-4.606223395648536,0.81,0.125,10.0,-0.002601766792553592,0.0020822290694801353,-0.005042022288499164,0.004170932143903416
-5.851996519306439,0.15,0.125,10.0,-0.001922825724645973,0.001818701147452711,-0.003927693583019453,0.0034763493114037354
-5.851996519306439,0.21,0.125,27.0,-0.0016675537794089534,0.0015789013518652834,-0.0033313264289419886,0.003142878695345522
-5.851996519306439,0.27,0.125,36.0,-0.0019788616446658625,0.001917915548543025,-0.003817966114520958,0.0037527199747874147
-5.851996519306439,0.33,0.125,59.0,-0.001384690793924657,0.0014375040516696007,-0.002679414842234048,0.0029201690844954217
-5.851996519306439,0.39,0.125,49.0,-0.0018073163487583044,0.001760471163587818,-0.0035472217158184992,0.003434801535736365
-5.851996519306439,0.45,0.125,50.0,-0.0023053002750403223,0.0021011850568160855,-0.004485675317525817,0.0041799649702425265
-5.851996519306439,0.51,0.125,41.0,-0.0031215066343569286,0.002704434470803745,-0.006362528934035884,0.005328926526757865
-5.851996519306439,0.57,0.125,50.0,-0.002492373349258705,0.0023510693581677124,-0.005269722846609737,0.004240606644848123
-5.851996519306439,0.63,0.125,61.0,-0.0019944341276176463,0.0020128374534930864,-0.003921880367751571,0.003713434405169563
-5.851996519306439,0.69,0.125,81.0,-0.0016993492905095834,0.0017078056216131934,-0.003496373428563041,0.0033552293482880095
-5.851996519306439,0.75,0.125,30.0,-0.0027060026716615383,0.002873465062345113,-0.005437608745028949,0.005799431678764185
-5.851996519306439,0.81,0.125,6.0,-0.005499381421438279,0.004258965544392202,-0.011278793138493856,0.007941848316890729
-7.434694395049624,0.15,0.125,11.0,-0.003165150663767915,0.0036573566583464074,-0.005961304686848283,0.0075400387182596815
-7.434694395049624,0.21,0.125,28.0,-0.0016466766297751376,0.0015522793455760963,-0.0032039782286198658,0.003004201660946086
-7.434694395049624,0.27,0.125,52.0,-0.0020144772823937973,0.0019822700265651693,-0.00389837406449073,0.00405119489867273
-7.434694395049624,0.33,0.125,57.0,-0.0017035842238356178,0.0017545065923899534,-0.0035016673907770357,0.003388003596688896
-7.434694395049624,0.39,0.125,65.0,-0.0016278893773268397,0.0016218121847469953,-0.0032023638103444415,0.0032353455708938827
-7.434694395049624,0.45,0.125,50.0,-0.002075187448517299,0.00199130431347364,-0.004137876060629141,0.0038869733123090082
-7.434694395049624,0.51,0.125,51.0,-0.0024006952653022884,0.002012541236385639,-0.004560752119333187,0.004091730267637529
-7.434694395049624,0.57,0.125,50.0,-0.002049534782168801,0.0020748747794789154,-0.004058274292795118,0.0040652804219200615
-7.434694395049624,0.63,0.125,67.0,-0.002371787410489079,0.0021260789845365556,-0.004641494981548714,0.004179369210960492
-7.434694395049624,0.69,0.125,59.0,-0.002230142567466863,0.0021657828002830427,-0.0043230856429503015,0.004378975949452686
-7.434694395049624,0.75,0.125,7.0,-0.003877214248446162,0.004663795367380962,-0.007023577464990304,0.009555700044452912
-9.445439785451793,0.15,0.125,16.0,-0.00194311461586784,0.00187480047483428,-0.0037542054649912686,0.003789888244950769
-9.445439785451793,0.21,0.125,36.0,-0.0020455829406721454,0.0023231172077451726,-0.0038585568501751464,0.004750467860649302
-9.445439785451793,0.27,0.125,61.0,-0.0019038886700233544,0.002041336371005186,-0.003957074924695603,0.0038229963334693445
-9.445439785451793,0.33,0.125,71.0,-0.0018557001814847143,0.0018750331894215099,-0.003558051283979465,0.003795772712755311
-9.445439785451793,0.39,0.125,59.0,-0.0015543271279668202,0.0014613137802820587,-0.0029404823708665553,0.0028705640464600493
-9.445439785451793,0.45,0.125,61.0,-0.0020483976715308886,0.001946032260979211,-0.004090650279990656,0.0037177211223464518
-9.445439785451793,0.51,0.125,40.0,-0.00255558988486543,0.003329085640238945,-0.005284478682986939,0.006448631402690563
-9.445439785451793,0.57,0.125,56.0,-0.0025833288053269884,0.0024890439371686255,-0.005033945562062498,0.004808543502976993
-9.445439785451793,0.63,0.125,59.0,-0.0029101763768070426,0.0028848294285124198,-0.005957978332805231,0.005797091980386925
-9.445439785451793,0.69,0.125,31.0,-0.003679616235224392,0.003784370324289407,-0.007264230983774285,0.007693260625244089
-9.445439785451793,0.75,0.125,6.0,-0.006656646259776948,0.0057058746326899,-0.012362520892466847,0.01100822751611045
-11.999999999999996,0.15,0.125,17.0,-0.0017626199365215459,0.0016026418652581938,-0.003713021802397661,0.003060470424668712
-11.999999999999996,0.21,0.125,35.0,-0.0023305985769859956,0.002505172683990752,-0.004549990453772648,0.005077645804191791
-11.999999999999996,0.27,0.125,61.0,-0.0027989912432118914,0.0029972224584131207,-0.005568678638029084,0.005950399259367337
-11.999999999999996,0.33,0.125,84.0,-0.002150599941937556,0.0020061386867667123,-0.004161336378813994,0.0040311818218004645
-11.999999999999996,0.39,0.125,69.0,-0.002519671583443985,0.002210196959547145,-0.004870276106787853,0.004441308668111298
-11.999999999999996,0.45,0.125,65.0,-0.002212948427990961,0.0021831890890109933,-0.0043796923584445875,0.0040009779334469146
-11.999999999999996,0.51,0.125,48.0,-0.002841820332440765,0.002986603238356094,-0.0055388194357871125,0.0061841812194706166
-11.999999999999996,0.57,0.125,45.0,-0.005197585671182664,0.004547189265540615,-0.01034201197854229,0.00873196131627453
-11.999999999999996,0.63,0.125,40.0,-0.005411561358478733,0.0046587638326186995,-0.010599303162385183,0.009241099348221687
-11.999999999999996,0.69,0.125,23.0,-0.007354889664061697,0.007958956272486998,-0.012975460534055556,0.016562512774867116
-11.999999999999996,0.75,0.125,7.0,-0.01673356089235206,0.01423840310682339,-0.032860333964842996,0.026144653750325347
-0.0999999999999992,0.27,0.5,9.0,-0.00019135140903643556,0.000130479555018696,-0.0003897675886826698,0.0002298682201939963
-0.0999999999999992,0.33,0.5,18.0,-7.569849902476223e-05,5.2026317472764535e-05,-0.0001576693338264838,9.702051733031657e-05
-0.0999999999999992,0.39,0.5,29.0,-3.8301511045985265e-05,3.4070065061200504e-05,-7.805590291185247e-05,6.471031070989037e-05
-0.0999999999999992,0.45,0.5,33.0,-0.00011371552859439722,0.00014878624839878118,-0.00020713711949830094,0.00030629576512259277
-0.0999999999999992,0.51,0.5,45.0,-8.17514946942872e-05,0.00011410516840184792,-0.0001471080791123063,0.0002322043819366043
-0.0999999999999992,0.57,0.5,35.0,-9.56837496533851e-05,0.00013003189062831731,-0.00017242180381729814,0.0002624005739339901
-0.0999999999999992,0.63,0.5,45.0,-8.265073556601583e-05,0.00010196728803244445,-0.00014441748921775817,0.00021481119099183669
-0.0999999999999992,0.69,0.5,58.0,-7.923049908502576e-05,9.186859325071382e-05,-0.00014434884977914005,0.00019375373051931178
-0.0999999999999992,0.75,0.5,102.0,-4.8754966157459925e-05,5.664745434031991e-05,-9.004145660816244e-05,0.00012012422815986035
-0.0999999999999992,0.81,0.5,112.0,-7.234016570290294e-05,7.430495179718138e-05,-0.000142122244587515,0.00014472973465052178
-0.0999999999999992,0.87,0.5,11.0,-8.993073546587576e-06,6.009621699996208e-06,-1.9005781634723568e-05,1.1403017384322564e-05
-0.1270454343320614,0.27,0.5,9.0,-0.00029381689985669764,0.00024283491560235979,-0.0005944584838387399,0.0004498218760221113
-0.1270454343320614,0.33,0.5,18.0,-0.00010204523102255523,7.74292617721172e-05,-0.00021308333495990072,0.00014939010892075466
-0.1270454343320614,0.39,0.5,31.0,-5.806655345052219e-05,5.4094247543011264e-05,-0.00010641884845105369,0.00011127654617445341
-0.1270454343320614,0.45,0.5,31.0,-0.00015029532325229892,0.00018371274192079015,-0.00027139326564863854,0.0004034277755154753
-0.1270454343320614,0.51,0.5,45.0,-9.242127510888777e-05,0.00013099275531136165,-0.00017217546527745044,0.0002698726867064713
-0.1270454343320614,0.57,0.5,37.0,-0.00010285428793924061,0.00014224093646473794,-0.00018750864836105353,0.0002992486281213357
-0.1270454343320614,0.63,0.5,43.0,-9.081975834336777e-05,0.0001203870228039549,-0.0001716623968552047,0.0002488614853082617
-0.1270454343320614,0.69,0.5,59.0,-8.013451503264529e-05,9.29940087291953e-05,-0.0001517313180788632,0.00019064731166273266
-0.1270454343320614,0.75,0.5,105.0,-5.0000558875057285e-05,5.895403124564479e-05,-9.732044271418036e-05,0.00012133353520836695
-0.1270454343320614,0.81,0.5,108.0,-7.330167131206718e-05,7.739798359988278e-05,-0.00014239208790480467,0.00014744058359436385
-0.1270454343320614,0.87,0.5,11.0,-1.3556051054676016e-05,8.893438624730578e-06,-2.9478982021920045e-05,1.5391248714115247e-05
-0.1614054238462062,0.27,0.5,8.0,-0.0005336711053480353,0.0004763629085172416,-0.001056560284719843,0.0009488782013060693
-0.1614054238462062,0.33,0.5,19.0,-0.0001477685257525328,0.00013097405442084794,-0.0002999906463312452,0.0002638681601572487
-0.1614054238462062,0.39,0.5,32.0,-0.00010504165513095792,0.0001573329865410454,-0.00019555840353045113,0.000328478951970286
-0.1614054238462062,0.45,0.5,31.0,-0.00017861532363017265,0.00024431445838581745,-0.00033412311444820013,0.0005178384729302248
-0.1614054238462062,0.51,0.5,43.0,-0.00013122023838764286,0.00017061361874326972,-0.00024569497687070143,0.0003506971984996885
-0.1614054238462062,0.57,0.5,37.0,-0.00012739516486211401,0.000178938951343359,-0.0002471136912140214,0.0003903430331858822
-0.1614054238462062,0.63,0.5,43.0,-0.00011286790759490251,0.00014759484955377116,-0.00021337552209922168,0.0003021148509188639
-0.1614054238462062,0.69,0.5,61.0,-9.546508377940383e-05,0.00010987547619962952,-0.0001801728770536846,0.00022579011314539417
-0.1614054238462062,0.75,0.5,107.0,-5.675861620713794e-05,6.223932209346088e-05,-0.00010361049786651928,0.0001322103763396678
-0.1614054238462062,0.81,0.5,105.0,-7.561699396956576e-05,8.21885101140417e-05,-0.00015539464714814225,0.00016085508571666714
-0.1614054238462062,0.87,0.5,10.0,-1.0513017752800092e-05,9.468082910042879e-06,-2.0546476598014847e-05,1.8324645396118424e-05
-0.2050582217609121,0.27,0.5,8.0,-0.0008812421782860569,0.0007764370126887008,-0.0017876712407752554,0.0014825746995650313
-0.2050582217609121,0.33,0.5,21.0,-0.00023113468390617995,0.00021273237700215569,-0.00045296010384155046,0.00040362833305758575
-0.2050582217609121,0.39,0.5,32.0,-0.00016897303607665392,0.00023166348133430632,-0.0003133843252426833,0.0004837536204666623
-0.2050582217609121,0.45,0.5,29.0,-0.0003072587278244207,0.00037729273939022693,-0.0005540188356463833,0.000804490198767849
-0.2050582217609121,0.51,0.5,48.0,-0.0001747364031932157,0.00021621346586703802,-0.0003265476203186117,0.0004594092641682215
-0.2050582217609121,0.57,0.5,33.0,-0.00021235981017249131,0.00027300274452489855,-0.000398105270471121,0.0005704270688246265
-0.2050582217609121,0.63,0.5,45.0,-0.00014433003556228545,0.00019195754154569864,-0.00027454952486141655,0.00040350558892507247
-0.2050582217609121,0.69,0.5,59.0,-0.00012821039136246803,0.00014880481027213646,-0.0002469629168183079,0.00030240758601583236
-0.2050582217609121,0.75,0.5,107.0,-6.661006564421969e-05,8.445349457594563e-05,-0.00013538187149761315,0.00015935783191727557
-0.2050582217609121,0.81,0.5,104.0,-9.333316172211421e-05,9.621816543814316e-05,-0.00018786715201796005,0.0001975529910069932
-0.2050582217609121,0.87,0.5,10.0,-1.944410573814185e-05,2.0688678963103766e-05,-3.444838068287264e-05,4.21131461806562e-05
-0.2605171084697358,0.27,0.5,9.0,-0.001233713855921798,0.0011547314690779512,-0.002280786348371752,0.0022791777541610217
-0.2605171084697358,0.33,0.5,20.0,-0.0003805589535230509,0.00033263601675959293,-0.000723571575770943,0.0006400018580731726
-0.2605171084697358,0.39,0.5,32.0,-0.00025058302979459634,0.0002924590703077939,-0.00048826092889369326,0.0006066748469849472
-0.2605171084697358,0.45,0.5,31.0,-0.0004151577247941431,0.00046386671865716205,-0.0007651090542359629,0.0010132872966821926
-0.2605171084697358,0.51,0.5,47.0,-0.00023743173959469554,0.0002889866433107503,-0.00044848942216417444,0.0005912287893695873
-0.2605171084697358,0.57,0.5,39.0,-0.0002514891602658781,0.00032411287346702336,-0.00048205105489718586,0.0006847371072352618
-0.2605171084697358,0.63,0.5,42.0,-0.00019234528961998315,0.00022554561034457489,-0.00034174834952361557,0.00047655692439206837
-0.2605171084697358,0.69,0.5,58.0,-0.00016138644651367571,0.0001794360707932546,-0.00031019449186032083,0.0003584475290598645
-0.2605171084697358,0.75,0.5,107.0,-6.953567972880223e-05,8.843320739259905e-05,-0.00013791709113137172,0.00017012081116108842
-0.2605171084697358,0.81,0.5,101.0,-0.00010434548245912922,0.00011174776109467785,-0.00020299186164019674,0.00021414859305289753
-0.2605171084697358,0.87,0.5,10.0,-2.7195407459112887e-05,3.0394985130321523e-05,-5.289386679121602e-05,5.823630317884906e-05
-0.3309750919646877,0.27,0.5,9.0,-0.0016228167971953644,0.0015254143303967936,-0.0032654002803977856,0.002839099083726068
-0.3309750919646877,0.33,0.5,20.0,-0.0005581013387284477,0.0005634419187847663,-0.0011427733708093853,0.001088825351522781
-0.3309750919646877,0.39,0.5,31.0,-0.00038315517391310146,0.00043533546616173185,-0.0007303765239743104,0.0008633669301755061
-0.3309750919646877,0.45,0.5,34.0,-0.0005571739102639606,0.000658748853365914,-0.0010488980857274765,0.0013112612765569362
-0.3309750919646877,0.51,0.5,46.0,-0.0003462566012730685,0.000389744587965323,-0.0006649202584430184,0.000794353916624715
-0.3309750919646877,0.57,0.5,42.0,-0.00034317752236609733,0.00041783467150712737,-0.0006471451436031063,0.0008542199516618918
-0.3309750919646877,0.63,0.5,42.0,-0.00022380163223516158,0.0002810788958637741,-0.00042517283977317995,0.0005801676284734023
-0.3309750919646877,0.69,0.5,54.0,-0.0002123947275025692,0.00022231372206028518,-0.0004054438888515454,0.00048244985817019894
-0.3309750919646877,0.75,0.5,110.0,-8.831918150960644e-05,0.00010201035665998079,-0.0001742036767026405,0.00020148432092632952
-0.3309750919646877,0.81,0.5,98.0,-0.00011936385784730422,0.0001168906418461134,-0.00022933617979674828,0.0002332738512502183
-0.3309750919646877,0.87,0.5,10.0,-3.9340743606326145e-05,4.300934044201283e-05,-7.436465386462498e-05,8.809075984238926e-05
-0.4204887431174507,0.27,0.5,10.0,-0.0015234397911785377,0.001428139966135857,-0.002928420126988174,0.0027829310945250694
-0.4204887431174507,0.33,0.5,19.0,-0.0008936723619584425,0.000997956869559028,-0.0018233943928251328,0.0019244017823718124
-0.4204887431174507,0.39,0.5,31.0,-0.000500144673108731,0.0006214248880108389,-0.0009615271570827527,0.0012611435214543343
-0.4204887431174507,0.45,0.5,38.0,-0.0007342873076214417,0.0008304568277478206,-0.0013359310864302545,0.0017603372360565977
-0.4204887431174507,0.51,0.5,45.0,-0.0004920973821014976,0.0005606138468634034,-0.000947025329287237,0.0011113673994348138
-0.4204887431174507,0.57,0.5,44.0,-0.00042935195258633,0.0005404766482139938,-0.000852509629903786,0.001096530280936998
-0.4204887431174507,0.63,0.5,42.0,-0.0003067758588165439,0.0003866719962321804,-0.0005700954379276462,0.0007856035948973122
-0.4204887431174507,0.69,0.5,55.0,-0.0002724976747033113,0.00031385905329295327,-0.0005350537424689688,0.0005847674595127311
-0.4204887431174507,0.75,0.5,104.0,-0.00011745431141054188,0.00013359006921305703,-0.0002228274845710693,0.00026707739139758926
-0.4204887431174507,0.81,0.5,97.0,-0.00014275521566173337,0.00014054140750600937,-0.00027649956192897366,0.00027683366691279656
-0.4204887431174507,0.87,0.5,10.0,-6.42804746882498e-05,6.54274332994302e-05,-0.00012184774878479773,0.0001325571379734241
-0.534211750010973,0.21,0.5,5.0,-0.0025962699788300682,0.0024793707989916756,-0.004780994822825324,0.004780994822825324
-0.534211750010973,0.27,0.5,11.0,-0.0023382302552834547,0.0022512651664729523,-0.00465423236826935,0.004319310062411147
-0.534211750010973,0.33,0.5,23.0,-0.001124706809082123,0.0012189637392096273,-0.002294918471514195,0.002339405586938025
-0.534211750010973,0.39,0.5,26.0,-0.000902876417922093,0.0010303427541755394,-0.0017719896016237938,0.002107641331074929
-0.534211750010973,0.45,0.5,43.0,-0.000834546137450032,0.000997738340028135,-0.0016126050524047422,0.0020674962188482874
-0.534211750010973,0.51,0.5,43.0,-0.0007060966266182855,0.0008196895233643324,-0.0013939966448122086,0.001614307378763151
-0.534211750010973,0.57,0.5,42.0,-0.0006097756869060498,0.0007096369626583553,-0.001125754570682652,0.0015401821470569605
-0.534211750010973,0.63,0.5,48.0,-0.00041220445858657133,0.0004757866570101363,-0.0007608679630983215,0.0010052042868834063
-0.534211750010973,0.69,0.5,52.0,-0.00038460026535836156,0.00039246679567188407,-0.0007233701639926708,0.0007955878021021053
-0.534211750010973,0.75,0.5,101.0,-0.00015717144861487716,0.00018043339546435248,-0.0002945553392313934,0.0003599037664976489
-0.534211750010973,0.81,0.5,98.0,-0.00018571618515849205,0.0001835736320219168,-0.00036842615843810507,0.0003594060784724531
-0.534211750010973,0.87,0.5,7.0,-0.00010584656283257093,7.146172805024991e-05,-0.00023326771676037054,0.00013533389867127966
-0.6786916380543213,0.21,0.5,6.0,-0.0027554072250669894,0.002567459783708518,-0.005448461569992533,0.004786217114106687
-0.6786916380543213,0.27,0.5,11.0,-0.0034598170976713858,0.002899203653952788,-0.006950712725025266,0.00559533671333867
-0.6786916380543213,0.33,0.5,24.0,-0.0017314127661045686,0.001804606219212094,-0.003459649851343963,0.003563283601000531
-0.6786916380543213,0.39,0.5,26.0,-0.001232758693718754,0.0013319660671821533,-0.0024880357366670524,0.002709555271518524
-0.6786916380543213,0.45,0.5,43.0,-0.0010848182697297325,0.0011733547802975826,-0.0020885435795043403,0.002389437668382314
-0.6786916380543213,0.51,0.5,48.0,-0.000835328696361036,0.0009829747881853488,-0.0016644942335862997,0.0018371081910990154
-0.6786916380543213,0.57,0.5,42.0,-0.000681144149498844,0.0007555337877401027,-0.0013667631294699612,0.0015273556430491625
-0.6786916380543213,0.63,0.5,45.0,-0.000542133310148132,0.0006154064808620736,-0.0010758593953869488,0.0012616818972477563
-0.6786916380543213,0.69,0.5,53.0,-0.00046480997658788164,0.0004964759989271485,-0.0009282498941884237,0.000983075268851678
-0.6786916380543213,0.75,0.5,95.0,-0.00020919245923650158,0.00023253480479218586,-0.00039608761188248374,0.0004848803295750069
-0.6786916380543213,0.81,0.5,101.0,-0.00025330316966033404,0.0002379281190513763,-0.0004982785316935595,0.0004850660061624759
-0.6786916380543213,0.87,0.5,5.0,-0.0002259709400481258,0.00015211587189198906,-0.0005115055142772996,0.0003234955215426716
-0.8622467393414548,0.21,0.5,9.0,-0.0036960031311462885,0.0031181092542206675,-0.00737637515202759,0.006047300408977177
-0.8622467393414548,0.27,0.5,11.0,-0.004200362423243971,0.004584684362556371,-0.007942355977253448,0.008969149782060308
-0.8622467393414548,0.33,0.5,24.0,-0.002172347054814835,0.00208742511346691,-0.004364989970529938,0.0038824602916732375
-0.8622467393414548,0.39,0.5,30.0,-0.0016688696909301698,0.0016591499215046436,-0.0032495413141922585,0.003220928837288252
-0.8622467393414548,0.45,0.5,44.0,-0.001218705955032097,0.0013128017709644667,-0.0024046972061969635,0.00260124340018554
-0.8622467393414548,0.51,0.5,49.0,-0.0009659598020594026,0.0010787867507870473,-0.0018988207373411543,0.0021159365162678307
-0.8622467393414548,0.57,0.5,36.0,-0.0009849591084267809,0.0008937742827910209,-0.0018867207017599554,0.001743292618994796
-0.8622467393414548,0.63,0.5,47.0,-0.0006924677594502787,0.0007679889984702822,-0.0013913092411349315,0.0014239687552420456
-0.8622467393414548,0.69,0.5,51.0,-0.0005980392034798637,0.0006397445171974251,-0.0011766193396727878,0.0012898195366715828
-0.8622467393414548,0.75,0.5,97.0,-0.000305284183832964,0.00033915175573171624,-0.0006074832887264171,0.0006879590385448568
-0.8622467393414548,0.81,0.5,98.0,-0.00035764152436024415,0.0003714870275035122,-0.0007300480943539784,0.0007298225300669363
-1.0954451150103353,0.21,0.5,9.0,-0.0038295854927910644,0.0035916698471000455,-0.007563735994166138,0.0066911314829315605
-1.0954451150103353,0.27,0.5,12.0,-0.004521101509222036,0.004680365427719913,-0.008928507153376428,0.008881582997460615
-1.0954451150103353,0.33,0.5,26.0,-0.002299068009798092,0.00208616245260694,-0.004683325543941061,0.004070098063280501
-1.0954451150103353,0.39,0.5,31.0,-0.002079194572718999,0.002087940198043871,-0.0041041953309442535,0.004050045768767581
-1.0954451150103353,0.45,0.5,44.0,-0.001428198143643607,0.0014266626922118863,-0.002833805683450826,0.0028805544977298313
-1.0954451150103353,0.51,0.5,46.0,-0.0012522344892886357,0.0013143460067826553,-0.002389183638095456,0.002632768073229768
-1.0954451150103353,0.57,0.5,41.0,-0.0010894013000882906,0.0011103708414185616,-0.002292945895172179,0.0020366428614515793
-1.0954451150103353,0.63,0.5,45.0,-0.0009650603443865906,0.0009538813034585035,-0.001859180054482429,0.0018991699744022857
-1.0954451150103353,0.69,0.5,53.0,-0.0007588341426990108,0.0008170238215511401,-0.001492199291430613,0.001569387095086312
-1.0954451150103353,0.75,0.5,94.0,-0.0004644161463206177,0.00048229962861669824,-0.0009073534888850704,0.0009664914333251619
-1.0954451150103353,0.81,0.5,96.0,-0.0005545416128936835,0.0005492247930329514,-0.0011051114135181964,0.0010684897791213672
-1.3917130042341646,0.21,0.5,9.0,-0.0029460980248803533,0.0031744820664839886,-0.0054220431083036435,0.006464935410763599
-1.3917130042341646,0.27,0.5,17.0,-0.0031629623544630757,0.003164218233513287,-0.006001760731551662,0.006589476993702702
-1.3917130042341646,0.33,0.5,27.0,-0.002044224723907374,0.001760212453682452,-0.004106932899546405,0.003314638877821787
-1.3917130042341646,0.39,0.5,34.0,-0.0015416907742676306,0.001894021850714289,-0.00321124826584564,0.0034545101630449235
-1.3917130042341646,0.45,0.5,47.0,-0.0014042633659474312,0.0014276835973075868,-0.002751020917112591,0.00270184722613277
-1.3917130042341646,0.51,0.5,40.0,-0.0013363408331762588,0.0014496859334631152,-0.0025637093424197995,0.0029004886290479154
-1.3917130042341646,0.57,0.5,42.0,-0.0012726668219556387,0.0012812061457848846,-0.0025136710747810883,0.002449441320038388
-1.3917130042341646,0.63,0.5,49.0,-0.0009925605095056338,0.001033231158393463,-0.0019385932899342244,0.0020439596625839093
-1.3917130042341646,0.69,0.5,51.0,-0.0009482167264045936,0.0010054228330922388,-0.0018427825872401775,0.0020568836170546017
-1.3917130042341646,0.75,0.5,107.0,-0.0005327652475069474,0.0005392727495919484,-0.001040482138191253,0.0010546782638447794
-1.3917130042341646,0.81,0.5,75.0,-0.0007508774771975144,0.0007045810237033119,-0.0015277690666879856,0.0012774674095978173
-1.7681078308849825,0.21,0.5,9.0,-0.0033596930825642423,0.0038804652431988387,-0.006883701795700177,0.0072379591151658556
-1.7681078308849825,0.27,0.5,22.0,-0.0019303461290533439,0.0018913929217462529,-0.0038553378638835466,0.003951608851925045
-1.7681078308849825,0.33,0.5,24.0,-0.002148404689585268,0.0016461229821911503,-0.004577551517805733,0.00304300760985443
-1.7681078308849825,0.39,0.5,45.0,-0.001317659469315542,0.0013613138354345608,-0.002563259020149169,0.0027065256008658232
-1.7681078308849825,0.45,0.5,42.0,-0.0015067516283408492,0.0014040121062748555,-0.00299069445028512,0.002695896756322567
-1.7681078308849825,0.51,0.5,43.0,-0.0014799774090753592,0.001538998728417909,-0.002948798949544592,0.003099692561869373
-1.7681078308849825,0.57,0.5,43.0,-0.0010194528413770474,0.001071319675957311,-0.0020046580580192594,0.002054130427769704
-1.7681078308849825,0.63,0.5,49.0,-0.0011330095687712128,0.0012012704886308673,-0.0022350378187082484,0.0024009970578160074
-1.7681078308849825,0.69,0.5,57.0,-0.0008234684108303834,0.0008492442554447301,-0.0015978496698496663,0.001610987530536887
-1.7681078308849825,0.75,0.5,114.0,-0.0006077219281491281,0.000623760303698045,-0.0012687322921237914,0.0011751796416813636
-1.7681078308849825,0.81,0.5,50.0,-0.0008758402357343639,0.0007223893828414985,-0.0017854096267603536,0.001358524070506979
-2.246300273206928,0.21,0.5,11.0,-0.003875187498053027,0.0033722542334531855,-0.00849603249902524,0.005936586594039722
-2.246300273206928,0.27,0.5,27.0,-0.001580041107596481,0.0014222222842457215,-0.0033620048870097396,0.002744893699078623
-2.246300273206928,0.33,0.5,25.0,-0.002236498082085748,0.001840234524858613,-0.004557820803964952,0.0034956817144470285
-2.246300273206928,0.39,0.5,49.0,-0.0014119598604845067,0.0013341535332191806,-0.0027530621836116716,0.002556855277005453
-2.246300273206928,0.45,0.5,47.0,-0.001350912636004497,0.001258995509880895,-0.0027073404581712296,0.0024100834472364926
-2.246300273206928,0.51,0.5,40.0,-0.0013384628129815429,0.0014547018885058267,-0.002607670521283426,0.0028776914048238215
-2.246300273206928,0.57,0.5,44.0,-0.0012028358148609619,0.0012078670738552657,-0.0022976278067984362,0.002492355111554282
-2.246300273206928,0.63,0.5,45.0,-0.001296154112040037,0.0013153590176361288,-0.002596237088339868,0.002584649882056476
-2.246300273206928,0.69,0.5,66.0,-0.0009356228642276406,0.0009021667453607892,-0.0018005730404770195,0.0018005526484581274
-2.246300273206928,0.75,0.5,101.0,-0.0007424875632878988,0.0007164353700719382,-0.0014798383832346428,0.0014073506959840457
-2.246300273206928,0.81,0.5,43.0,-0.0011802496901614876,0.0009925069736868455,-0.002522795325057883,0.0017567687247388392
-2.8538219384978776,0.21,0.5,15.0,-0.0023500464821079796,0.0021419289706053855,-0.004451966411805666,0.004264998552416599
-2.8538219384978776,0.27,0.5,31.0,-0.0017186689799756612,0.0015818380065859854,-0.003298282744348736,0.0030004833738035974
-2.8538219384978776,0.33,0.5,32.0,-0.0017122141525906236,0.0016729938499476704,-0.003453688341768328,0.0032373050117111774
-2.8538219384978776,0.39,0.5,47.0,-0.0015236845599167716,0.0014345564214905387,-0.002924117020652988,0.00278041908827858
-2.8538219384978776,0.45,0.5,47.0,-0.0012639906722675877,0.0010955656426999878,-0.0024083525785109625,0.0022253614320276883
-2.8538219384978776,0.51,0.5,41.0,-0.0012015192185176116,0.001069383640592866,-0.0023728339500535623,0.002092603512933509
-2.8538219384978776,0.57,0.5,51.0,-0.0009561222306956796,0.0009174638163251089,-0.0019444793294217172,0.001766974329620522
-2.8538219384978776,0.63,0.5,41.0,-0.0012925730005592204,0.0014696815517537332,-0.002501084008739794,0.0029611714088705874
-2.8538219384978776,0.69,0.5,57.0,-0.0008343058632729151,0.0008219449323187907,-0.0016466605865671164,0.0015643603356999948
-2.8538219384978776,0.75,0.5,107.0,-0.0007660521363321198,0.0007260718549956393,-0.0014780204430026116,0.0014634714754523485
-2.8538219384978776,0.81,0.5,29.0,-0.0014110779626778345,0.0010751100963023322,-0.0028676992697710614,0.002027549808617546
-3.625650476828127,0.21,0.5,16.0,-0.00195820316691873,0.0020347250669011754,-0.003716406101050722,0.004151772050666181
-3.625650476828127,0.27,0.5,31.0,-0.0018970873246969327,0.001773619664809138,-0.0037094641627655337,0.003614341095873376
-3.625650476828127,0.33,0.5,42.0,-0.0015570605907983019,0.0014170621982505902,-0.0032183309558739014,0.0027107524325476425
-3.625650476828127,0.39,0.5,43.0,-0.0014231194254582598,0.0013244215150613411,-0.002762259298826923,0.00265287980897311
-3.625650476828127,0.45,0.5,55.0,-0.0011676737473755928,0.001080578460698533,-0.0022773114674026957,0.0021804622915278246
-3.625650476828127,0.51,0.5,44.0,-0.000983434896287941,0.0008118953951106396,-0.00200010178310702,0.0016215669320944481
-3.625650476828127,0.57,0.5,42.0,-0.0012607775948516033,0.0012817762350481054,-0.002525219532942127,0.0025779163267015508
-3.625650476828127,0.63,0.5,47.0,-0.001168588303445038,0.0012670477484628723,-0.002148372225656152,0.002667340905342618
-3.625650476828127,0.69,0.5,59.0,-0.00092558165953733,0.0009275406730749745,-0.0017307241124685175,0.0017761641220690688
-3.625650476828127,0.75,0.5,99.0,-0.0008496412952634163,0.0008102455463368561,-0.0016164638467481927,0.0016169125409237416
-3.625650476828127,0.81,0.5,18.0,-0.0017037961442628485,0.001534018237284379,-0.0033850076321620725,0.00285842261115451
-4.60622339564853,0.15,0.5,5.0,-0.005514596431252318,0.0033668384248406458,-0.010646607928365626,0.0067564274800423485
-4.60622339564853,0.21,0.5,16.0,-0.0018577198769980498,0.0019944093329939618,-0.0034789394211821294,0.00402977225328978
-4.60622339564853,0.27,0.5,29.0,-0.001675425022355271,0.0017856769582037441,-0.00340480793622485,0.0034566582923285212
-4.60622339564853,0.33,0.5,51.0,-0.0012905401012478681,0.001300444221508181,-0.002551336322266623,0.0025717540800579866
-4.60622339564853,0.39,0.5,47.0,-0.0012254580501813584,0.00116801285601056,-0.002480465707831439,0.002247193415566765
-4.60622339564853,0.45,0.5,52.0,-0.001099658535379914,0.0011154820774150142,-0.002206861544510824,0.002206091772212467
-4.60622339564853,0.51,0.5,52.0,-0.0010207115229025922,0.001000440055739455,-0.002022995369457636,0.001924261391759406
-4.60622339564853,0.57,0.5,34.0,-0.00151171526490361,0.00190594420009416,-0.002905954881829815,0.0036566579138399957
-4.60622339564853,0.63,0.5,57.0,-0.001452280707680154,0.0015146558696217606,-0.002821866369434414,0.0029347165286983693
-4.60622339564853,0.69,0.5,73.0,-0.0011638636702888477,0.001207312785924915,-0.002307902269278224,0.002320247097412472
-4.60622339564853,0.75,0.5,72.0,-0.0012035925917717547,0.0011489824877318714,-0.0023252344741594155,0.002319742751914353
-4.60622339564853,0.81,0.5,10.0,-0.002896857110118282,0.0032546361148214622,-0.005738260470180041,0.0062599884686238005
-5.851996519306435,0.15,0.5,9.0,-0.0010717244428662255,0.0009798654314524897,-0.0021215474234263783,0.0018313674212574237
-5.851996519306435,0.21,0.5,22.0,-0.002158533519982138,0.002213741111098483,-0.0042982619114502576,0.004278504368216054
-5.851996519306435,0.27,0.5,42.0,-0.001716689431995651,0.0017808283377403317,-0.00347034367682049,0.003396400839377389
-5.851996519306435,0.33,0.5,55.0,-0.0012296678147058755,0.001376666785441182,-0.0024882080234404206,0.002585621279658076
-5.851996519306435,0.39,0.5,48.0,-0.0012421058258500332,0.001201438113878986,-0.0025124714562136646,0.002319068642842649
-5.851996519306435,0.45,0.5,57.0,-0.0013598914116708964,0.0013236774285359015,-0.002628239182418497,0.002652071444852573
-5.851996519306435,0.51,0.5,45.0,-0.0019043779621794766,0.0019165457399803185,-0.003924127258946892,0.003556897713384903
-5.851996519306435,0.57,0.5,49.0,-0.0019320757757656537,0.0018141246474790433,-0.0037360579604342214,0.0035292099711911524
-5.851996519306435,0.63,0.5,47.0,-0.0018609186991890355,0.0017794464020943579,-0.003984217812497356,0.0032003150523100873
-5.851996519306435,0.69,0.5,76.0,-0.001626771456995826,0.0016317056035466877,-0.0033317241361931365,0.003116734773370841
-5.851996519306435,0.75,0.5,41.0,-0.002518420777225035,0.0023682535244630245,-0.005044945099846737,0.004559298048287981
-5.851996519306435,0.81,0.5,8.0,-0.004795187816475158,0.004152102597608532,-0.008997916620994653,0.00828318162828108
-7.434694395049627,0.15,0.5,9.0,-0.00146267293828873,0.0015467116830327388,-0.0027416162320462387,0.0031547310990915115
-7.434694395049627,0.21,0.5,25.0,-0.0017416751629843762,0.0016671801620557589,-0.0036285224302271464,0.0031420325903014513
-7.434694395049627,0.27,0.5,46.0,-0.001943055650903879,0.0017230930976196992,-0.003492348984606935,0.0036638221115302366
-7.434694395049627,0.33,0.5,57.0,-0.0016221402844160072,0.0017416545951042203,-0.003158430025399265,0.0035814066677575633
-7.434694395049627,0.39,0.5,63.0,-0.0013019381902937127,0.0013198956873905537,-0.0025810177277020593,0.0025138857802764238
-7.434694395049627,0.45,0.5,57.0,-0.002018320668785783,0.001867750875795517,-0.003965753171709741,0.00372865154528679
-7.434694395049627,0.51,0.5,55.0,-0.0019906931935168323,0.001969156345742836,-0.0038357960932476204,0.0038562926225802203
-7.434694395049627,0.57,0.5,37.0,-0.0028090802027201925,0.002724051343366956,-0.005736981849678766,0.0053176266472333405
-7.434694395049627,0.63,0.5,60.0,-0.0019399759181769635,0.0020370723004217144,-0.003992789868040256,0.003938386844234831
-7.434694395049627,0.69,0.5,59.0,-0.002903196380819296,0.0027085165262162726,-0.005598320948875036,0.005242413140951384
-7.434694395049627,0.75,0.5,25.0,-0.003960466513182849,0.0035475274714167363,-0.008438007081036439,0.006584893678632205
-7.434694395049627,0.81,0.5,5.0,-0.009347495929647209,0.00826342587216713,-0.017513249322036108,0.014333744523719183
-9.445439785451788,0.15,0.5,12.0,-0.00148044308941712,0.001346237463110918,-0.003142784631909822,0.0024430630566025686
-9.445439785451788,0.21,0.5,22.0,-0.001940311268092057,0.0018630901743737472,-0.003793147211810652,0.0037351982862792836
-9.445439785451788,0.27,0.5,57.0,-0.0016695372291522642,0.0016918177982661361,-0.003449672885422128,0.0032413394756156443
-9.445439785451788,0.33,0.5,67.0,-0.0014379815869389819,0.0014886991961758124,-0.0027666713998336623,0.0029542807390673356
-9.445439785451788,0.39,0.5,60.0,-0.0020229162803685526,0.0017715665675339914,-0.003981751390751225,0.0034384171454564334
-9.445439785451788,0.45,0.5,55.0,-0.002106545951121981,0.001961616401485675,-0.004201095204732491,0.0037511428785887567
-9.445439785451788,0.51,0.5,53.0,-0.0024588069560978797,0.0023092385014456163,-0.004857405760126083,0.004421993917710233
-9.445439785451788,0.57,0.5,46.0,-0.0030979113772864604,0.003236033502967221,-0.006488655298323697,0.006144433713454227
-9.445439785451788,0.63,0.5,49.0,-0.0042768580609836605,0.0038415578346428165,-0.008679254300699567,0.007202475800964607
-9.445439785451788,0.69,0.5,50.0,-0.0043846090128640235,0.004167528541054454,-0.008469554074436919,0.008036996363648984
-9.445439785451788,0.75,0.5,19.0,-0.0065132206754798605,0.006375718608639917,-0.013052138961148043,0.012429875785140616
-9.445439785451788,0.81,0.5,6.0,-0.009915864878639971,0.00925784659300688,-0.017974714942622965,0.01898377539661685
-12.00000000000001,0.15,0.5,7.0,-0.004757231984428979,0.008014898990966855,-0.008107865136452596,0.017983551308111485
-12.00000000000001,0.21,0.5,24.0,-0.00252346424718982,0.002609613294829274,-0.004798721213469868,0.005458325868260262
-12.00000000000001,0.27,0.5,60.0,-0.0020085256302327385,0.0022489359869853837,-0.004129631661403302,0.004354674979336418
-12.00000000000001,0.33,0.5,66.0,-0.002182815459447324,0.002282286605589862,-0.004177726000398423,0.00457687237247092
-12.00000000000001,0.39,0.5,79.0,-0.002416391178547269,0.002457753999963287,-0.004637862962285548,0.0046526141970413765
-12.00000000000001,0.45,0.5,64.0,-0.0031666591189687633,0.00312538219109141,-0.006260426848944622,0.006077603244864477
-12.00000000000001,0.51,0.5,47.0,-0.004086108057031955,0.0037710483359558043,-0.008027844401714009,0.0073663709360003195
-12.00000000000001,0.57,0.5,45.0,-0.004985676159151928,0.004301305820893811,-0.009658658762862319,0.008616289851914443
-12.00000000000001,0.63,0.5,38.0,-0.007942009909328791,0.00653257560770265,-0.01604140747703898,0.01235439714802875
-12.00000000000001,0.69,0.5,38.0,-0.009680787393770391,0.009662949265484303,-0.020118544521674515,0.01865197858238749
-12.00000000000001,0.75,0.5,13.0,-0.011342134037321363,0.016148838941546995,-0.02043366847414196,0.0345394634315454
-12.00000000000001,0.81,0.5,8.0,-0.005432901140982549,0.007359445046342539,-0.010088502363954366,0.015461179076818377
-12.00000000000001,0.87,0.5,6.0,-0.017642068423673916,0.015507661793047045,-0.03484039930906858,0.02864138001539271
-12.00000000000001,0.93,0.5,5.0,-0.005896703034052458,0.00531476889703093,-0.009351007671374801,0.010336325165868087
-0.1000000000000085,0.21,1.0,10.0,-8.175214474085084e-05,8.408435802727474e-05,-0.00016205053562939645,0.0001540500899046003
-0.1000000000000085,0.27,1.0,20.0,-6.74578358558649e-05,6.0357009900146246e-05,-0.00013662126878747087,0.0001076869377297112
-0.1000000000000085,0.33,1.0,30.0,-6.024352514672389e-05,4.7600338523837466e-05,-0.00012413649151662466,9.108524898261855e-05
-0.1000000000000085,0.39,1.0,47.0,-2.829244236012684e-05,2.438757931776217e-05,-5.649293322176679e-05,4.6287832483892726e-05
-0.1000000000000085,0.45,1.0,41.0,-5.965837158586591e-05,7.109031756135032e-05,-0.00010877916922995169,0.0001589723624647347
-0.1000000000000085,0.51,1.0,49.0,-6.672037151252677e-05,8.136231289247256e-05,-0.00011930640698775287,0.00017087899282109317
-0.1000000000000085,0.57,1.0,38.0,-6.871859362970556e-05,9.25360064911615e-05,-0.00012587675464888594,0.00019150737161096376
-0.1000000000000085,0.63,1.0,48.0,-7.307551100144723e-05,8.459092523906944e-05,-0.00014042655063011092,0.00016861133376378998
-0.1000000000000085,0.69,1.0,55.0,-5.173236182342242e-05,6.5707619355636e-05,-9.61791168937532e-05,0.0001348426115319905
-0.1000000000000085,0.75,1.0,94.0,-4.2968922605834645e-05,5.185687124618294e-05,-8.365481765068985e-05,0.00010392662793991443
-0.1000000000000085,0.81,1.0,60.0,-7.536605992925945e-05,7.336675947644605e-05,-0.0001546033564246056,0.00013821432516105135
-0.1000000000000085,0.87,1.0,5.0,-5.7712799299114494e-06,2.3429479365066844e-06,-1.0792318179486675e-05,5.7399275185776536e-06
-0.1270454343320629,0.21,1.0,10.0,-0.00013121004556617823,0.00012464378480835824,-0.0002689692470767726,0.00023043477127023047
-0.1270454343320629,0.27,1.0,20.0,-0.00010842983603189054,0.00010154306197830821,-0.00021797714684719408,0.00018819193656881305
-0.1270454343320629,0.33,1.0,30.0,-8.342527124196524e-05,7.097289534476954e-05,-0.0001727782152677472,0.00013396668897543151
-0.1270454343320629,0.39,1.0,47.0,-3.945658615686572e-05,3.257682922706371e-05,-7.75690500751092e-05,6.365830726441761e-05
-0.1270454343320629,0.45,1.0,42.0,-6.457935540894016e-05,8.303947348558759e-05,-0.00012562164688242756,0.00016592373413073987
-0.1270454343320629,0.51,1.0,48.0,-7.408150111926265e-05,9.300120938913637e-05,-0.00014326352514638417,0.00019313917548893165
-0.1270454343320629,0.57,1.0,37.0,-7.646957748129437e-05,0.00010640117027141515,-0.00014149511350536616,0.0002179517889039779
-0.1270454343320629,0.63,1.0,49.0,-7.93429468467206e-05,9.002085180256647e-05,-0.00014626915924382774,0.00018467760331936862
-0.1270454343320629,0.69,1.0,56.0,-5.3346506780246633e-05,6.829749308573485e-05,-9.916585830061122e-05,0.00014017971681927696
-0.1270454343320629,0.75,1.0,93.0,-4.408428118948541e-05,5.304506616121006e-05,-8.594027895302488e-05,0.00010761111471968918
-0.1270454343320629,0.81,1.0,60.0,-7.597254328426127e-05,7.381859081107025e-05,-0.00015713233647970945,0.00014130860875958287
-0.1270454343320629,0.87,1.0,5.0,-6.887151563494964e-06,3.029547363020402e-06,-1.2238764791261413e-05,6.497378042791258e-06
-0.1614054238462024,0.21,1.0,11.0,-0.00019564340332023375,0.00017926355766621226,-0.0003899606318361151,0.0003442882953782891
-0.1614054238462024,0.27,1.0,20.0,-0.00019020500162790307,0.00017330993345300528,-0.00037902197956908373,0.0003353474855402238
-0.1614054238462024,0.33,1.0,31.0,-0.0001279665940467964,0.00010712955699179977,-0.0002600438625126652,0.00020377131088294252
-0.1614054238462024,0.39,1.0,47.0,-5.866759676066164e-05,5.247413109307771e-05,-0.00012518711799968578,9.482260558938655e-05
-0.1614054238462024,0.45,1.0,41.0,-8.958652954217287e-05,0.00010151265307694608,-0.00017010786775538633,0.0002058967894143583
-0.1614054238462024,0.51,1.0,48.0,-9.375007564524251e-05,0.00011060222382291021,-0.0001812349644930178,0.0002282580007407626
-0.1614054238462024,0.57,1.0,38.0,-9.045192653430465e-05,0.00012027041772474028,-0.0001675750667937352,0.0002522937710130377
-0.1614054238462024,0.63,1.0,48.0,-9.311130202286112e-05,0.00010997371766972563,-0.00017798511167890584,0.00021908468823571053
-0.1614054238462024,0.69,1.0,56.0,-5.826917742370823e-05,7.720725080682364e-05,-0.00011010347345931586,0.00015623857179985324
-0.1614054238462024,0.75,1.0,93.0,-4.803973662222947e-05,5.6977538844466985e-05,-9.20862207244902e-05,0.00011695813519733399
-0.1614054238462024,0.81,1.0,60.0,-8.124997324234462e-05,7.447421542467328e-05,-0.00015604395200721934,0.0001487278057638133
-0.1614054238462024,0.87,1.0,5.0,-8.262387685986627e-06,5.736514916065982e-06,-2.047721409721425e-05,7.520517549997063e-06
-0.2050582217609077,0.21,1.0,12.0,-0.0002994901190261664,0.00026439134445020143,-0.0005808437265089797,0.000509172823522526
-0.2050582217609077,0.27,1.0,20.0,-0.0003037551041437512,0.00031393756795041286,-0.0006580486310876048,0.0005606325082172935
-0.2050582217609077,0.33,1.0,32.0,-0.0002154335957034992,0.00019416441568051478,-0.00042550633147525374,0.0003650153307800553
-0.2050582217609077,0.39,1.0,47.0,-0.00010502424729917424,9.049439476340091e-05,-0.0002239542923527743,0.000176913531740599
-0.2050582217609077,0.45,1.0,39.0,-0.00013213381323026274,0.00015038978016505695,-0.00025353744558278814,0.0002930973886349501
-0.2050582217609077,0.51,1.0,50.0,-0.00012928108302535262,0.00015617424199755684,-0.00024178077759902944,0.00030988746537559945
-0.2050582217609077,0.57,1.0,36.0,-0.0001242238387393112,0.0001616708783126364,-0.0002351278219493011,0.0003443223233252294
-0.2050582217609077,0.63,1.0,52.0,-0.00012549000370420068,0.00013000707082942673,-0.00022951307318784203,0.00028436744338201426
-0.2050582217609077,0.69,1.0,53.0,-6.981238675062308e-05,9.008745882788861e-05,-0.0001282924763763512,0.00019058410816409345
-0.2050582217609077,0.75,1.0,90.0,-5.655239871730138e-05,6.737992645584949e-05,-0.00010811367233812942,0.00013695229347892413
-0.2050582217609077,0.81,1.0,62.0,-8.963974213516898e-05,8.818128205558862e-05,-0.00018203782114860397,0.00016054631282495297
-0.2050582217609077,0.87,1.0,5.0,-2.2294621451246542e-05,1.38808110219379e-05,-5.022678018478115e-05,1.9224359805658464e-05
-0.2605171084697463,0.21,1.0,12.0,-0.0005046077614493821,0.00044449869034093577,-0.0009825093795062258,0.0008382512530271144
-0.2605171084697463,0.27,1.0,20.0,-0.000550808893121775,0.0004998749931411177,-0.0011044949070446424,0.0009561352419869156
-0.2605171084697463,0.33,1.0,33.0,-0.00036480489221948524,0.00030406878415402655,-0.0007217046700231896,0.0005982197752373771
-0.2605171084697463,0.39,1.0,47.0,-0.00017130018033912296,0.00016175245318019363,-0.0003581874273482135,0.00029179839664383395
-0.2605171084697463,0.45,1.0,40.0,-0.0002009353783363448,0.00019631775357354194,-0.0003884183506420002,0.0004048346253275784
-0.2605171084697463,0.51,1.0,51.0,-0.00017734740967661195,0.00019987339301031978,-0.000329004603692544,0.00041790135325043767
-0.2605171084697463,0.57,1.0,34.0,-0.0001974780569028167,0.00023707244838130635,-0.00035163835491759497,0.0005096859105901494
-0.2605171084697463,0.63,1.0,51.0,-0.0001692584719690593,0.00017739467591774836,-0.0003103864231961576,0.0003650347602779666
-0.2605171084697463,0.69,1.0,55.0,-8.70607318073408e-05,0.00011527544214036985,-0.00016129407040554796,0.0002445348248753984
-0.2605171084697463,0.75,1.0,88.0,-7.559781129082144e-05,8.140330018057759e-05,-0.00013618469143101327,0.00017186697182572055
-0.2605171084697463,0.81,1.0,62.0,-0.0001074933445982254,0.00010510092177948786,-0.00021936183170772082,0.00019699274219535213
-0.2605171084697463,0.87,1.0,5.0,-3.114352039319543e-05,2.3610012346208988e-05,-8.219251466461416e-05,3.114352039319526e-05
-0.3309750919646957,0.21,1.0,12.0,-0.0008559725555128327,0.0007068319659212962,-0.0016755638781930894,0.0013519406240076297
-0.3309750919646957,0.27,1.0,23.0,-0.0008188145865863709,0.0007307965198982693,-0.0015811109283765232,0.0014606458213610072
-0.3309750919646957,0.33,1.0,31.0,-0.0006016802271851388,0.0005139920440837058,-0.001169180799852391,0.0009911778058540495
-0.3309750919646957,0.39,1.0,46.0,-0.0002829348601757741,0.00026563109111114587,-0.0005871508552683994,0.0005000593431519298
-0.3309750919646957,0.45,1.0,42.0,-0.0003023371015691358,0.0002882239610327477,-0.0006290091581975752,0.000526850705482036
-0.3309750919646957,0.51,1.0,49.0,-0.0002723705546031851,0.0002942351735322174,-0.0005078305040191187,0.0006132751187901444
-0.3309750919646957,0.57,1.0,36.0,-0.00025481316020639134,0.00031330298084347323,-0.0004768010679379523,0.0006301629070165813
-0.3309750919646957,0.63,1.0,49.0,-0.00022505786298630763,0.00024761117638337314,-0.0004261881797701146,0.00048083868233007843
-0.3309750919646957,0.69,1.0,55.0,-0.00011445350565381133,0.00014430760082918438,-0.00020908453676487404,0.0003059222481293396
-0.3309750919646957,0.75,1.0,86.0,-9.007285700926604e-05,0.0001024306376935038,-0.00017164245631185604,0.0002040881880072273
-0.3309750919646957,0.81,1.0,64.0,-0.0001244943472785219,0.00012406841896832706,-0.0002503421753717465,0.00022835182591077145
-0.3309750919646957,0.87,1.0,5.0,-5.671959075539421e-05,3.798605998341911e-05,-0.00013638400794064874,5.6719590755394036e-05
-0.420488743117451,0.21,1.0,12.0,-0.0014193840559655845,0.00119337024462014,-0.0028795116635845757,0.0022250640401680097
-0.420488743117451,0.27,1.0,24.0,-0.0011835733719100365,0.0011836032395736535,-0.0023282714711546824,0.0022031924707882878
-0.420488743117451,0.33,1.0,32.0,-0.0009464676275046129,0.000772541214219734,-0.0018676458873986318,0.0014607172843458475
-0.420488743117451,0.39,1.0,45.0,-0.0004351112897978369,0.00038185837367898457,-0.000894621052272079,0.0007392756689324936
-0.420488743117451,0.45,1.0,43.0,-0.0004707011404379967,0.0004038346613151266,-0.0009291469848964033,0.0007901202478481741
-0.420488743117451,0.51,1.0,47.0,-0.00040440222257470947,0.00044197033547353683,-0.0007728847905932007,0.0008778373481790764
-0.420488743117451,0.57,1.0,37.0,-0.000376530529973681,0.00040687356951132734,-0.0006783731268297935,0.0008828191190538377
-0.420488743117451,0.63,1.0,49.0,-0.0003040298565692398,0.0003349009380127037,-0.0005774004356899573,0.0006762548761914366
-0.420488743117451,0.69,1.0,56.0,-0.00015123056949375776,0.0001744230757001786,-0.0002659770614754972,0.00039298346657112284
-0.420488743117451,0.75,1.0,82.0,-0.00011824132310847073,0.00012720236297113444,-0.00022326559758254817,0.00026489198250013735
-0.420488743117451,0.81,1.0,65.0,-0.00014858348438490776,0.00013502164612597307,-0.0002912461319815029,0.0002720606781144275
-0.420488743117451,0.87,1.0,6.0,-7.919938295558593e-05,4.689199480530556e-05,-0.0001358036336572832,8.715584907559304e-05
-0.5342117500109833,0.21,1.0,12.0,-0.00242680061141947,0.0019006207340496867,-0.0051426464742779735,0.0035042286222271546
-0.5342117500109833,0.27,1.0,26.0,-0.0017324509789573852,0.0017209142442471742,-0.003459578812531271,0.0031786963386733215
-0.5342117500109833,0.33,1.0,29.0,-0.0012244334169201944,0.0011240804437201064,-0.002530193422792266,0.002179517389349237
-0.5342117500109833,0.39,1.0,47.0,-0.0006048242669902065,0.0005407213920788301,-0.001190880628893078,0.0010592042125700802
-0.5342117500109833,0.45,1.0,45.0,-0.0006525519683566746,0.0006168776597244664,-0.0013994797376105247,0.0011394652269998296
-0.5342117500109833,0.51,1.0,44.0,-0.0006317647054802421,0.0006424424607781396,-0.0012463012512340054,0.0013075320348016656
-0.5342117500109833,0.57,1.0,38.0,-0.0005453699019250324,0.0005675391647166179,-0.001022892492507958,0.0011767818389941762
-0.5342117500109833,0.63,1.0,47.0,-0.00042952676594583546,0.0004604332682061848,-0.0008151330079298449,0.0009425303384922227
-0.5342117500109833,0.69,1.0,55.0,-0.00020275372827618346,0.00025526808459104506,-0.0003646669936280166,0.0005322492789311578
-0.5342117500109833,0.75,1.0,87.0,-0.00014973393992038725,0.00016463061936357687,-0.0002779264045792264,0.00032802579448011783
-0.5342117500109833,0.81,1.0,61.0,-0.00018443971200267616,0.00017164911359313136,-0.00035996748006516654,0.0003378628529408071
-0.5342117500109833,0.87,1.0,6.0,-0.00011180298920802441,9.467204347239177e-05,-0.0002262340734410783,0.0001918450365235118
-0.6786916380543062,0.21,1.0,12.0,-0.003553902985860076,0.0025369843223377103,-0.007174923516542417,0.004730464460577843
-0.6786916380543062,0.27,1.0,28.0,-0.002253107932805909,0.0021401439636550335,-0.0044588272258968345,0.004030866551936429
-0.6786916380543062,0.33,1.0,29.0,-0.0017783176433008151,0.0015903572909357923,-0.00375873190641361,0.003016952334976578
-0.6786916380543062,0.39,1.0,46.0,-0.0007991787586753976,0.000761847465107564,-0.0016698674328836241,0.0014670916776229424
-0.6786916380543062,0.45,1.0,48.0,-0.0008620636475496114,0.000843608296241819,-0.0019089411594754627,0.0015261823794963868
-0.6786916380543062,0.51,1.0,44.0,-0.0008146111719414646,0.0007829930947139779,-0.0015786945482240615,0.0015587629090798975
-0.6786916380543062,0.57,1.0,38.0,-0.0006923883012626158,0.0007701094453116518,-0.0013149404900923683,0.001571390756639836
-0.6786916380543062,0.63,1.0,43.0,-0.0005945882190276171,0.0006211257460197002,-0.0011257630512431377,0.0012260277188798011
-0.6786916380543062,0.69,1.0,57.0,-0.00025487682734317836,0.0003137858102222239,-0.00047632796186193214,0.0006432722687311417
-0.6786916380543062,0.75,1.0,87.0,-0.000188009675115918,0.00020149387190658075,-0.0003562373184160501,0.0003999750015467611
-0.6786916380543062,0.81,1.0,59.0,-0.00022159266337346293,0.00020888310856336632,-0.0004363299045035213,0.00040759859137821935
-0.6786916380543062,0.87,1.0,6.0,-0.00016810307623018236,0.00018276111608017676,-0.0003057379358648027,0.0003568232717229651
-0.8622467393414557,0.21,1.0,12.0,-0.004055931962274537,0.0032061999820261556,-0.008291467890864941,0.00578330903124541
-0.8622467393414557,0.27,1.0,29.0,-0.0026773756863010807,0.0025149556998971456,-0.005215654444851741,0.004947935574106985
-0.8622467393414557,0.33,1.0,29.0,-0.0022546259669589145,0.002133089927096846,-0.004626866368623707,0.003935438966797888
-0.8622467393414557,0.39,1.0,45.0,-0.0010779133922015525,0.00102015128940111,-0.002182188181113818,0.0019287808765115742
-0.8622467393414557,0.45,1.0,51.0,-0.0011185912055130891,0.001014161302173319,-0.002326777667715099,0.001927866350789505
-0.8622467393414557,0.51,1.0,42.0,-0.0010802268766694728,0.001031736084773656,-0.002167902117479094,0.0019803465158698148
-0.8622467393414557,0.57,1.0,38.0,-0.0009397954758049849,0.0009589825258132285,-0.0018154015831239204,0.0020606549030233582
-0.8622467393414557,0.63,1.0,45.0,-0.0007345607942528936,0.000760280996427562,-0.0014272212659781206,0.001529977815145499
-0.8622467393414557,0.69,1.0,55.0,-0.00032550689236574633,0.00041083959480906943,-0.000644649883994553,0.0008385665210811729
-0.8622467393414557,0.75,1.0,85.0,-0.0002315629591251349,0.00026859525219958733,-0.000479823035605088,0.0005048901318962554
-0.8622467393414557,0.81,1.0,60.0,-0.0002654981178736209,0.0002534073810242717,-0.0005193140907699805,0.0004872827367481479
-0.8622467393414557,0.87,1.0,6.0,-0.00023960577099592847,0.00028686396718911406,-0.0004481914289122258,0.000578115259195914
-1.0954451150103266,0.21,1.0,12.0,-0.004086909838916324,0.003151962781982983,-0.008813589948760012,0.005900649394305492
-1.0954451150103266,0.27,1.0,29.0,-0.00285322403496718,0.0026615962199028603,-0.005685865751385898,0.005265518571968064
-1.0954451150103266,0.33,1.0,33.0,-0.002389490586453969,0.002356170058415762,-0.004902784426484705,0.004364205612228323
-1.0954451150103266,0.39,1.0,41.0,-0.0012769091749603614,0.0011822249837263688,-0.0025366709811597064,0.0023744668181705252
-1.0954451150103266,0.45,1.0,50.0,-0.00140752115703906,0.0012511850371565675,-0.00300812322060605,0.002340154243344524
-1.0954451150103266,0.51,1.0,45.0,-0.0014242623065760572,0.0013675496327967616,-0.002864158826700046,0.00263065864498423
-1.0954451150103266,0.57,1.0,41.0,-0.0011328969785462267,0.0012556246804662195,-0.0022513880421277353,0.0025864233370956587
-1.0954451150103266,0.63,1.0,47.0,-0.0009336993270697647,0.0009216567822640956,-0.0017676038568038763,0.001928822027810438
-1.0954451150103266,0.69,1.0,54.0,-0.0004528543100016612,0.0005612748317439731,-0.0009272377462101494,0.001110244508407299
-1.0954451150103266,0.75,1.0,83.0,-0.0003338068513004863,0.0003422210881739412,-0.000647886549277166,0.000683838365037307
-1.0954451150103266,0.81,1.0,56.0,-0.0003537939612798275,0.0003564722745824822,-0.0007166305136574642,0.000662993651807394
-1.0954451150103266,0.87,1.0,6.0,-0.00032015084555914175,0.00037946016968902024,-0.0005995083009728841,0.0008349589524839218
-1.3917130042341563,0.21,1.0,13.0,-0.0030509901604948487,0.0028614057850809196,-0.006296527473990959,0.005360047843502541
-1.3917130042341563,0.27,1.0,29.0,-0.002386142537785424,0.002346952819561203,-0.004787704237182148,0.00460952166915158
-1.3917130042341563,0.33,1.0,35.0,-0.0022819643978238663,0.0020038174861051776,-0.004704371604313832,0.003851312473760652
-1.3917130042341563,0.39,1.0,44.0,-0.0014573468780896708,0.0014383337143671624,-0.0027253473415820646,0.0028037203680717467
-1.3917130042341563,0.45,1.0,50.0,-0.0017340589968684761,0.0015252623623041733,-0.0034528348363720676,0.002978896687371543
-1.3917130042341563,0.51,1.0,41.0,-0.0019286320055349273,0.0018113670175554115,-0.0036106763939821413,0.0037660790020719107
-1.3917130042341563,0.57,1.0,47.0,-0.001447188652697736,0.0016239881625720882,-0.002797861619648797,0.003285916921578562
-1.3917130042341563,0.63,1.0,47.0,-0.0011365931389136833,0.0012701243768242362,-0.0021602927496029217,0.0025926459119521446
-1.3917130042341563,0.69,1.0,51.0,-0.0007056823855160028,0.0008305072208648152,-0.0013367296621120046,0.0017372321114312275
-1.3917130042341563,0.75,1.0,86.0,-0.00044522662113310476,0.00045130101125438407,-0.0008588760648582514,0.0008868802264622159
-1.3917130042341563,0.81,1.0,49.0,-0.0005115232568979354,0.0004877135157880574,-0.001108211146113294,0.0008721756159757617
-1.3917130042341563,0.87,1.0,6.0,-0.00033245066813366203,0.000354194579437639,-0.000655886810272584,0.0009705606929523717
-1.7681078308849831,0.21,1.0,12.0,-0.0031514907330738055,0.002348130116480244,-0.00636606797943513,0.0042974194987389506
-1.7681078308849831,0.27,1.0,29.0,-0.002065668136742646,0.0018710957283823472,-0.004167839470180545,0.003742783704733682
-1.7681078308849831,0.33,1.0,42.0,-0.0018525570120813439,0.0015128294850561136,-0.0037478444826206177,0.002882076017015254
-1.7681078308849831,0.39,1.0,37.0,-0.0016893201347763255,0.0017368874287367224,-0.0033658107727780593,0.0032997317787251314
-1.7681078308849831,0.45,1.0,53.0,-0.0018681925426582654,0.0016192741245231559,-0.003478964710608874,0.003199693754586475
-1.7681078308849831,0.51,1.0,42.0,-0.002006073569352193,0.001938729288697969,-0.0037843314858702253,0.003899558699958934
-1.7681078308849831,0.57,1.0,50.0,-0.0016904858383013624,0.0017853028013095202,-0.003185892630312768,0.003616911973895452
-1.7681078308849831,0.63,1.0,49.0,-0.0011043628495189005,0.0013580484812366898,-0.0021327158553250732,0.002579698064932223
-1.7681078308849831,0.69,1.0,48.0,-0.0008149581742346685,0.0008947118394008992,-0.0015958081915543867,0.0017494624934527823
-1.7681078308849831,0.75,1.0,83.0,-0.0005730296383807718,0.0005594459569140892,-0.0011418993652633049,0.0011271222424057727
-1.7681078308849831,0.81,1.0,45.0,-0.0006503350891760531,0.0005382239087005518,-0.0013687809896331016,0.0009795814639362614
-1.7681078308849831,0.87,1.0,6.0,-0.00040475838347853177,0.0005013486633872651,-0.00072243790184362,0.0010734821964350865
-2.2463002732069097,0.21,1.0,12.0,-0.003356232734063461,0.002672799267470694,-0.007033670518782065,0.005040750947267431
-2.2463002732069097,0.27,1.0,33.0,-0.0016848523049234248,0.0015224438779016336,-0.003243200977037399,0.0031387975550160744
-2.2463002732069097,0.33,1.0,41.0,-0.0018024303158436401,0.0015674831617238831,-0.0036939046496716767,0.0030284895605978313
-2.2463002732069097,0.39,1.0,40.0,-0.001526725952511067,0.0015232158366066328,-0.0030711036082794194,0.0029835648572923775
-2.2463002732069097,0.45,1.0,54.0,-0.0016643376375734124,0.0015042617376560168,-0.0032143248444981985,0.0030318960220939183
-2.2463002732069097,0.51,1.0,40.0,-0.0018732470071729512,0.0018829523787362273,-0.0037127817750081727,0.0036741811442107617
-2.2463002732069097,0.57,1.0,56.0,-0.0015107137350034573,0.0016359968638331723,-0.00291698744502073,0.0032694513784146135
-2.2463002732069097,0.63,1.0,44.0,-0.0012389914857537272,0.0014051338507652408,-0.0023362213646210923,0.0028868171262992712
-2.2463002732069097,0.69,1.0,62.0,-0.0007922839192116758,0.0008130431181434741,-0.0015449078140955242,0.001588787876749536
-2.2463002732069097,0.75,1.0,66.0,-0.0007341691751419166,0.000664796489813813,-0.0014483572737591548,0.0012727108478724038
-2.2463002732069097,0.81,1.0,41.0,-0.0008129237201130141,0.0006086151460382048,-0.0016612709323276065,0.00116032189458508
-2.2463002732069097,0.87,1.0,7.0,-0.001814622446673345,0.0014513294457143004,-0.0048785460069272705,0.0017319269217986083
-2.8538219384978847,0.15,1.0,5.0,-0.004222322901996844,0.004327564288256802,-0.007459097377553814,0.008656138916618894
-2.8538219384978847,0.21,1.0,12.0,-0.0026844951708627704,0.00226429518895703,-0.0051372748638468,0.00447131516561545
-2.8538219384978847,0.27,1.0,33.0,-0.0016464402348414684,0.0015335935959317026,-0.00326313710242998,0.003029273826231
-2.8538219384978847,0.33,1.0,44.0,-0.0013726693807860658,0.0012627098333671016,-0.0028302808733972704,0.0023377059533179548
-2.8538219384978847,0.39,1.0,42.0,-0.001426987041432523,0.0012279558844462072,-0.0028222388764948658,0.0024134075256766
-2.8538219384978847,0.45,1.0,56.0,-0.0012235795176132847,0.0012645266390960627,-0.0025133607857996012,0.002329439963469111
-2.8538219384978847,0.51,1.0,42.0,-0.0015532501239459416,0.0016317753052012402,-0.00301131731547507,0.0033442690009685794
-2.8538219384978847,0.57,1.0,53.0,-0.0013280506344414814,0.001515373634409365,-0.00270469178298867,0.0028953955645190424
-2.8538219384978847,0.63,1.0,50.0,-0.0011335397994674495,0.0012612699842711843,-0.0021544735318801533,0.002476599407999394
-2.8538219384978847,0.69,1.0,56.0,-0.0008723632782690367,0.0008462720971536097,-0.0017447194334242607,0.0016158499980586005
-2.8538219384978847,0.75,1.0,67.0,-0.0007104661582958442,0.0006957509045169989,-0.0014820607881506679,0.0012582282262286948
-2.8538219384978847,0.81,1.0,31.0,-0.0008601924263549203,0.0006573953500479663,-0.0018118515984126365,0.0012636385753682002
-2.8538219384978847,0.87,1.0,9.0,-0.0021362893535691197,0.001526653547239365,-0.005529505244231796,0.0019331656644854297
-3.625650476828114,0.21,1.0,16.0,-0.0018977621989720239,0.001954941156974329,-0.003962908147365629,0.0035590331911777642
-3.625650476828114,0.27,1.0,32.0,-0.0014736712076300986,0.0015517130753337867,-0.002996660547483483,0.0030623648788710555
-3.625650476828114,0.33,1.0,52.0,-0.0011824692249608028,0.0011644039453045493,-0.002244324719109534,0.002252508317314621
-3.625650476828114,0.39,1.0,47.0,-0.001077307730619412,0.001088556361295112,-0.002192867919746539,0.0020818892999677364
-3.625650476828114,0.45,1.0,53.0,-0.000997204265675407,0.0009574104730437796,-0.0019344788139064807,0.0019051350843965371
-3.625650476828114,0.51,1.0,50.0,-0.0010763303614173723,0.0011223877297659886,-0.002217550377205653,0.002133723319166338
-3.625650476828114,0.57,1.0,47.0,-0.0011306364921456296,0.001147426017232805,-0.0021941996143721135,0.002377587544962727
-3.625650476828114,0.63,1.0,46.0,-0.001193105115669778,0.001351741257461178,-0.0023272828299079245,0.0026591591367568115
-3.625650476828114,0.69,1.0,55.0,-0.0009523132829637375,0.0008706760181473405,-0.0018878245966461905,0.001737804644370825
-3.625650476828114,0.75,1.0,64.0,-0.0008246281595682995,0.000797569399566087,-0.001581109396424771,0.0015828675208153775
-3.625650476828114,0.81,1.0,24.0,-0.0011688443828246887,0.0009724758879868663,-0.0024009301193439617,0.0018650383746822653
-3.625650476828114,0.87,1.0,10.0,-0.002978720754083262,0.0015859299287304756,-0.006798243663022114,0.002760985791282644
-4.60622339564852,0.15,1.0,5.0,-0.0024594833358590135,0.0021386776929471114,-0.006935969475720815,0.002459483335859015
-4.60622339564852,0.21,1.0,15.0,-0.0017093200858812076,0.001539796755795768,-0.003399384733381381,0.0030522331278174946
-4.60622339564852,0.27,1.0,36.0,-0.0015496835143145671,0.0014489398065515107,-0.0030243791942441167,0.002902192897591325
-4.60622339564852,0.33,1.0,52.0,-0.0011946641870758006,0.0011763479440464358,-0.0022864210959959224,0.0023317700762247877
-4.60622339564852,0.39,1.0,49.0,-0.0010770626766770308,0.0009954091716824565,-0.0020762625260018447,0.0019529697535679506
-4.60622339564852,0.45,1.0,54.0,-0.0008405843578120279,0.0008106896538502746,-0.0016230003242386209,0.0016218540850057917
-4.60622339564852,0.51,1.0,55.0,-0.0008931268272501125,0.0008340020287576054,-0.001659871918059241,0.0016692022750260569
-4.60622339564852,0.57,1.0,48.0,-0.000934998743772408,0.001087497011745213,-0.0018808456105175722,0.0021614300883534125
-4.60622339564852,0.63,1.0,44.0,-0.0011360909600682883,0.0011947029362859348,-0.0022403181882474097,0.002371651182727101
-4.60622339564852,0.69,1.0,52.0,-0.0010598649250330747,0.0009560120421679471,-0.002064223179932113,0.0018989120499691182
-4.60622339564852,0.75,1.0,58.0,-0.0012909226614200688,0.0012170807666382285,-0.002532817899604425,0.002338862564062402
-4.60622339564852,0.81,1.0,22.0,-0.0017613734365975325,0.001793389729010754,-0.0038501939096802023,0.0031912498566958763
-4.60622339564852,0.87,1.0,9.0,-0.0042627357862258025,0.0028820138221618613,-0.008879400995205454,0.005220066838290413
-5.851996519306423,0.15,1.0,5.0,-0.0027363742995070604,0.0027363742995070604,-0.005466246332996571,0.005467284142432405
-5.851996519306423,0.21,1.0,18.0,-0.0013751936239491,0.0011211878147364418,-0.002702354720166411,0.002302973001100922
-5.851996519306423,0.27,1.0,39.0,-0.0017175624267370538,0.0017096210437058616,-0.003366054921774173,0.003216193241534447
-5.851996519306423,0.33,1.0,53.0,-0.0012568823487192759,0.0012301187095241468,-0.0024301632403469597,0.0023672005396676997
-5.851996519306423,0.39,1.0,53.0,-0.0013337786533084031,0.0012902451633614062,-0.0025809390688541116,0.0025511834876484093
-5.851996519306423,0.45,1.0,54.0,-0.0012611911383045198,0.0014664252562303693,-0.002600974857786144,0.0028975610626360043
-5.851996519306423,0.51,1.0,58.0,-0.0012789886474681514,0.0012029692818018173,-0.0025476976973896007,0.002422475613208709
-5.851996519306423,0.57,1.0,45.0,-0.0014689943025105122,0.0014548046080142458,-0.002809623997541363,0.002935071341018097
-5.851996519306423,0.63,1.0,42.0,-0.0014322245157843932,0.0014329501972183258,-0.0028929116395686807,0.002813156891318303
-5.851996519306423,0.69,1.0,54.0,-0.0016886617905647978,0.0015313107616101698,-0.0034271494429906502,0.0028874242553078304
-5.851996519306423,0.75,1.0,47.0,-0.0025430742370462518,0.002314457530227303,-0.005035979348272169,0.004555889749771689
-5.851996519306423,0.81,1.0,18.0,-0.003515737807349245,0.0035322221783394346,-0.007019438806457492,0.006660484181638093
-5.851996519306423,0.87,1.0,12.0,-0.004980688580978447,0.004173219042278463,-0.009684207501379306,0.008268761896864627
-7.434694395049647,0.21,1.0,20.0,-0.0013128409745774405,0.0013428286383827684,-0.002688214702018849,0.002575984784543248
-7.434694395049647,0.27,1.0,45.0,-0.001350113075543096,0.0013582452873727462,-0.0026862550269305687,0.0026229008779752538
-7.434694395049647,0.33,1.0,50.0,-0.0019624906360718357,0.002017329560679726,-0.003754618082923496,0.003962771949791085
-7.434694395049647,0.39,1.0,69.0,-0.0013692001307536587,0.00135778523348932,-0.0026610532910856266,0.0026243159972713383
-7.434694395049647,0.45,1.0,50.0,-0.001652347230181261,0.0016499838021950997,-0.0032676881778897528,0.003224728671071734
-7.434694395049647,0.51,1.0,61.0,-0.0020203043144922926,0.0022011525147147587,-0.004055347004047784,0.004115510930675183
-7.434694395049647,0.57,1.0,49.0,-0.0021752100202633933,0.0023823584021867693,-0.004263050159502349,0.0047493870530700665
-7.434694395049647,0.63,1.0,43.0,-0.00256673114596992,0.002413755110228125,-0.005069225963422027,0.004823236601401229
-7.434694395049647,0.69,1.0,38.0,-0.004263150265580599,0.0034278223202501234,-0.008518979440568841,0.006558425923321489
-7.434694395049647,0.75,1.0,32.0,-0.006441690759849316,0.00630374175362876,-0.012946550083586387,0.012251100276592528
-7.434694395049647,0.81,1.0,20.0,-0.004646991044365345,0.003413767288648086,-0.010074523990564103,0.006165688086370129
-7.434694395049647,0.87,1.0,15.0,-0.0031923047108261948,0.0027194897660715355,-0.0064357094490227525,0.005058086467871929
-7.434694395049647,0.93,1.0,5.0,-0.003480576490580179,0.002175286975977508,-0.006659887166551348,0.00461067306167111
-9.44543978545178,0.21,1.0,25.0,-0.0010951822872499245,0.0013174995632395348,-0.0022237628447988045,0.0026302939449300723
-9.44543978545178,0.27,1.0,45.0,-0.001878829321040219,0.0017817663205237121,-0.0036107891645935425,0.003601726573858825
-9.44543978545178,0.33,1.0,47.0,-0.0022126318603895405,0.002137188597596954,-0.004276291440789832,0.004209899706894776
-9.44543978545178,0.39,1.0,63.0,-0.0020045799545878405,0.0020027963290486558,-0.0038415141870663584,0.0039045478139132536
-9.44543978545178,0.45,1.0,64.0,-0.002391480920732299,0.0022473787877475334,-0.004826904330008242,0.004412562231160224
-9.44543978545178,0.51,1.0,56.0,-0.003592884734132509,0.0031644480407377914,-0.007268153996563218,0.006150896838268716
-9.44543978545178,0.57,1.0,42.0,-0.003923158314037881,0.004022466809888489,-0.007870165408570072,0.007807219292470679
-9.44543978545178,0.63,1.0,46.0,-0.004810328731145561,0.004167905012893187,-0.009254644282452882,0.007915687111129449
-9.44543978545178,0.69,1.0,35.0,-0.0055207878723793425,0.00451042218249315,-0.010703367851866648,0.008660847623482041
-9.44543978545178,0.75,1.0,35.0,-0.00819397116607613,0.008141807873427944,-0.01572433336464724,0.01591408027666629
-9.44543978545178,0.81,1.0,17.0,-0.007569820676332276,0.008275688531242182,-0.01530214994253658,0.016869133218233856
-9.44543978545178,0.87,1.0,15.0,-0.00545796538577911,0.004807169800385229,-0.011309432066432682,0.00960936441252207
-9.44543978545178,0.93,1.0,8.0,-0.007288128867591936,0.006614408137112088,-0.014915208586341905,0.012432325366012442
-11.999999999999996,0.21,1.0,21.0,-0.0019526431023828596,0.0018705228589401522,-0.0038146893471498796,0.00354901995892974
-11.999999999999996,0.27,1.0,44.0,-0.0021321262039513257,0.0019479502388522602,-0.004368441668858998,0.003824733045688193
-11.999999999999996,0.33,1.0,53.0,-0.0024674668742604546,0.0024114989758614843,-0.004979127601857615,0.0045975343157744035
-11.999999999999996,0.39,1.0,71.0,-0.002589983583580068,0.002642722435332821,-0.005121908097859491,0.005084667721672802
-11.999999999999996,0.45,1.0,66.0,-0.003525447019163669,0.003389040773680857,-0.007155172938722696,0.006372623032977313
-11.999999999999996,0.51,1.0,59.0,-0.005137921842650414,0.0046665223238939735,-0.010627121621428455,0.008843231598787627
-11.999999999999996,0.57,1.0,52.0,-0.0062992833705549,0.006073291396216554,-0.013085246503785251,0.011608948823864531
-11.999999999999996,0.63,1.0,31.0,-0.010683687607667757,0.008255956537877194,-0.021255642313563593,0.01602122066648164
-11.999999999999996,0.69,1.0,33.0,-0.012305268767809357,0.010585033554846487,-0.02599749909776575,0.01996555695588825
-11.999999999999996,0.75,1.0,20.0,-0.02066808788448295,0.01724727028719118,-0.03953114887163895,0.03492566466648378
-11.999999999999996,0.81,1.0,18.0,-0.008009941905215963,0.013818274806632093,-0.013370204748839303,0.03243405664700461
-11.999999999999996,0.87,1.0,14.0,-0.00538108904165368,0.004127374222729193,-0.010967955407107773,0.007342026695746676
-11.999999999999996,0.93,1.0,16.0,-0.006940545736059757,0.007966488352089693,-0.01335418607469405,0.015402183478226653
-0.0999999999999969,0.21,2.0,10.0,-7.966369876387407e-05,7.178011986622512e-05,-0.00016851478099056712,0.0001362050423360546
-0.0999999999999969,0.27,2.0,19.0,-4.405597809990591e-05,3.561587437006504e-05,-8.989587305974297e-05,6.492528718547171e-05
-0.0999999999999969,0.33,2.0,43.0,-2.8300582738512437e-05,2.7869472228466732e-05,-6.0235503712560833e-05,5.247200622088708e-05
-0.0999999999999969,0.39,2.0,48.0,-1.8098542601487425e-05,1.707285352950444e-05,-3.8863379876799935e-05,3.0545132124167685e-05
-0.0999999999999969,0.45,2.0,51.0,-1.6419942919091924e-05,1.2924700314769674e-05,-3.1509854286831975e-05,2.6024567086274322e-05
-0.0999999999999969,0.51,2.0,45.0,-1.2527825375250423e-05,1.0743517911400683e-05,-2.355305743325692e-05,2.1234800938747678e-05
-0.0999999999999969,0.57,2.0,50.0,-2.0588028784819716e-05,2.5796096560851496e-05,-3.705907236894847e-05,5.377358209416718e-05
-0.0999999999999969,0.63,2.0,40.0,-2.0257594285397822e-05,2.8939885551649986e-05,-3.634267922671246e-05,6.48241924378312e-05
-0.0999999999999969,0.69,2.0,55.0,-2.52412752166674e-05,3.141551070038748e-05,-4.79343653747249e-05,6.333817509743034e-05
-0.0999999999999969,0.75,2.0,40.0,-3.283567083673487e-05,4.076053659155762e-05,-6.303617992729309e-05,8.160397195638656e-05
-0.0999999999999969,0.81,2.0,38.0,-3.942692521507056e-05,4.251901771769884e-05,-7.734684624195233e-05,8.653116575835157e-05
-0.0999999999999969,0.87,2.0,27.0,-4.153322307634918e-05,2.1070246570878112e-05,-0.00010225437251855044,4.14014780103692e-05
-0.0999999999999969,0.93,2.0,34.0,-9.117367127295029e-07,6.43507820250081e-07,-2.0598844669769027e-06,1.1698810769116444e-06
-0.1270454343320518,0.21,2.0,10.0,-0.00011530811298810607,0.00010434884373050279,-0.00023375764755282773,0.0001927238528433613
-0.1270454343320518,0.27,2.0,19.0,-5.9033580964517185e-05,4.977240126323741e-05,-0.00011892508281760801,9.283107795423e-05
-0.1270454343320518,0.33,2.0,43.0,-4.080734090246904e-05,3.9685940468466454e-05,-8.189595722205765e-05,7.523123261879568e-05
-0.1270454343320518,0.39,2.0,48.0,-2.6561387514442625e-05,2.2690024400783726e-05,-5.260802527501567e-05,4.367397698789721e-05
-0.1270454343320518,0.45,2.0,51.0,-2.1202579127428685e-05,1.8018451621667316e-05,-4.3227610294770976e-05,3.5270545215751316e-05
-0.1270454343320518,0.51,2.0,45.0,-1.6008354548430464e-05,1.455639147808169e-05,-3.3100801600383244e-05,2.72418027726836e-05
-0.1270454343320518,0.57,2.0,50.0,-2.0788461507841974e-05,2.543589933851385e-05,-3.942455813322771e-05,5.2501289652194995e-05
-0.1270454343320518,0.63,2.0,41.0,-2.0108985852971342e-05,2.8668394852393224e-05,-3.706046796967479e-05,6.369107425775432e-05
-0.1270454343320518,0.69,2.0,54.0,-2.63076787320777e-05,3.112086138723707e-05,-4.978076589231922e-05,6.801077936036519e-05
-0.1270454343320518,0.75,2.0,40.0,-3.46562311306509e-05,4.0009855657275715e-05,-6.306944107157964e-05,8.534427109114078e-05
-0.1270454343320518,0.81,2.0,38.0,-4.077078374265348e-05,4.325415609195361e-05,-7.910512122313511e-05,8.8579621189904e-05
-0.1270454343320518,0.87,2.0,27.0,-4.160172350811921e-05,2.1440697779057755e-05,-0.00010272747686002228,4.144852541597323e-05
-0.1270454343320518,0.93,2.0,34.0,-1.3060695614977173e-06,9.607422078855508e-07,-2.863276998283709e-06,1.7486092546154202e-06
-0.1614054238462532,0.21,2.0,10.0,-0.00017340476156694356,0.0001523053744138081,-0.0003437703995194283,0.0002967734663634155
-0.1614054238462532,0.27,2.0,19.0,-8.814142110225167e-05,7.356953444655498e-05,-0.0001728318001412486,0.00014280884871316308
-0.1614054238462532,0.33,2.0,43.0,-6.480248905390091e-05,5.8550921786551894e-05,-0.00012816191762153356,0.00011578792219351615
-0.1614054238462532,0.39,2.0,48.0,-4.161277854756659e-05,3.5856465495177516e-05,-8.374626577039371e-05,6.952317349592957e-05
-0.1614054238462532,0.45,2.0,51.0,-3.181284798399776e-05,2.787437704629391e-05,-6.672396784031462e-05,5.313428005381034e-05
-0.1614054238462532,0.51,2.0,45.0,-2.5685776535170132e-05,2.1484901630624612e-05,-4.936219470818835e-05,4.4163753376099776e-05
-0.1614054238462532,0.57,2.0,50.0,-2.421607965268266e-05,2.6231676822503238e-05,-4.470587224007125e-05,5.1731190898349154e-05
-0.1614054238462532,0.63,2.0,41.0,-2.265530474880052e-05,3.266803495175665e-05,-4.10309962481625e-05,6.71523485419632e-05
-0.1614054238462532,0.69,2.0,54.0,-2.8566747873946776e-05,3.2475963960032405e-05,-5.23620818549124e-05,6.831406436489545e-05
-0.1614054238462532,0.75,2.0,40.0,-3.341480759169632e-05,4.197461991418011e-05,-6.451019409311149e-05,8.51731404955357e-05
-0.1614054238462532,0.81,2.0,37.0,-4.006436301516572e-05,4.497899060584537e-05,-7.857662709914239e-05,8.854494218087273e-05
-0.1614054238462532,0.87,2.0,28.0,-4.126305793587822e-05,2.1522740322625636e-05,-9.334655758036694e-05,4.110889827022914e-05
-0.1614054238462532,0.93,2.0,34.0,-2.1243264732066192e-06,1.4851291286726045e-06,-4.177789893729546e-06,3.003323531193514e-06
-0.205058221760839,0.21,2.0,10.0,-0.00030559390017080736,0.0002597715738569818,-0.0005818473113939104,0.0005229734363833608
-0.205058221760839,0.27,2.0,19.0,-0.00013990342779974073,0.0001295651612447822,-0.00027630241854869334,0.00024914066568586143
-0.205058221760839,0.33,2.0,43.0,-0.0001128396543990423,9.790828003874169e-05,-0.00022384932285337758,0.00019449370495911385
-0.205058221760839,0.39,2.0,48.0,-7.057259765146929e-05,6.195175043139812e-05,-0.0001435673164765513,0.00011941960429151466
-0.205058221760839,0.45,2.0,51.0,-5.60906088539678e-05,4.609462000255936e-05,-0.00011499088036686033,8.745604345947626e-05
-0.205058221760839,0.51,2.0,45.0,-4.417131292062373e-05,3.944834853147956e-05,-8.750105934691939e-05,7.387824510813167e-05
-0.205058221760839,0.57,2.0,50.0,-3.252062387039327e-05,3.118399834369936e-05,-6.581218237250687e-05,6.129422960299238e-05
-0.205058221760839,0.63,2.0,41.0,-2.9280452660848672e-05,3.852773733880891e-05,-5.5317642657379745e-05,7.947971018421188e-05
-0.205058221760839,0.69,2.0,54.0,-3.160148295654388e-05,3.976708384645747e-05,-6.001246700418871e-05,7.866068964532034e-05
-0.205058221760839,0.75,2.0,40.0,-4.01623120747032e-05,4.7267001158358464e-05,-7.380864364534677e-05,9.619631108206083e-05
-0.205058221760839,0.81,2.0,37.0,-4.62058308853941e-05,4.957514918029933e-05,-8.975870384474773e-05,9.78026851944319e-05
-0.205058221760839,0.87,2.0,28.0,-4.723434870059831e-05,2.4231854947964822e-05,-0.00010086953658661165,4.60656065718429e-05
-0.205058221760839,0.93,2.0,34.0,-3.2458774374808025e-06,2.5924836805399397e-06,-6.580517141729622e-06,5.091860850216973e-06
-0.2605171084697784,0.21,2.0,10.0,-0.0004991423568426439,0.00045357966099710884,-0.0010204224968544393,0.0008215364036876393
-0.2605171084697784,0.27,2.0,19.0,-0.0002233953741040042,0.00021979642741796375,-0.00047778117187616357,0.0004121835375753873
-0.2605171084697784,0.33,2.0,43.0,-0.0001838239520247522,0.00017380640741467335,-0.0003680770314188486,0.0003339915794692162
-0.2605171084697784,0.39,2.0,48.0,-0.0001226407173771992,0.00010881947212845748,-0.00024782387274497654,0.00020859866368309242
-0.2605171084697784,0.45,2.0,52.0,-9.118829933446571e-05,7.703166853486484e-05,-0.00019035000243029307,0.00014630171275345835
-0.2605171084697784,0.51,2.0,45.0,-7.470968665276026e-05,7.041878141587455e-05,-0.00014941945307933387,0.00012846327315632928
-0.2605171084697784,0.57,2.0,50.0,-5.4160176337453553e-05,4.396593627286234e-05,-0.00010868617005977268,8.741889680754815e-05
-0.2605171084697784,0.63,2.0,41.0,-4.463670841928749e-05,5.027111335030881e-05,-8.195341130544251e-05,0.00010849727729448176
-0.2605171084697784,0.69,2.0,53.0,-4.6009010639601924e-05,5.4848427698043276e-05,-8.632236981263836e-05,0.00010947818507364965
-0.2605171084697784,0.75,2.0,40.0,-5.268887912384319e-05,6.563183246170032e-05,-0.00010092456513158198,0.00012961300897481942
-0.2605171084697784,0.81,2.0,38.0,-5.96904217453391e-05,6.897867790440259e-05,-0.00011397989077432641,0.0001310200489200283
-0.2605171084697784,0.87,2.0,27.0,-5.5401846555891367e-05,2.746535715604446e-05,-0.00013227368875894847,3.768115944336486e-05
-0.2605171084697784,0.93,2.0,34.0,-6.962215248033e-06,5.20979603202066e-06,-1.4744805809080716e-05,9.543169623476921e-06
-0.3309750919646702,0.21,2.0,10.0,-0.0008233975314211562,0.0007092252233223484,-0.0015831520802818378,0.0013562582831775586
-0.3309750919646702,0.27,2.0,19.0,-0.000386811819878887,0.0003577973417594752,-0.0007433775945676827,0.0006999874132282024
-0.3309750919646702,0.33,2.0,43.0,-0.00031339166536006885,0.0002735485321398837,-0.0006112122044478649,0.0005441597426349724
-0.3309750919646702,0.39,2.0,48.0,-0.00021483851458125886,0.00017926336691541543,-0.0004307182426041681,0.00035820873541349106
-0.3309750919646702,0.45,2.0,52.0,-0.0001483978390076047,0.00012914717721507934,-0.0003021088981919364,0.0002440722694329676
-0.3309750919646702,0.51,2.0,45.0,-0.00012810481286240204,0.00011213853557002509,-0.00025794631094499577,0.000210630907411815
-0.3309750919646702,0.57,2.0,50.0,-7.883114358348308e-05,6.727741976972492e-05,-0.0001668954891001864,0.00012224789144406277
-0.3309750919646702,0.63,2.0,41.0,-6.757020302391612e-05,6.595298003698566e-05,-0.00012762026377051333,0.00013841154999358292
-0.3309750919646702,0.69,2.0,53.0,-5.877100092689541e-05,6.890276897136477e-05,-0.00011600040965855462,0.00013288226823193988
-0.3309750919646702,0.75,2.0,40.0,-6.800962876596703e-05,7.838205018031995e-05,-0.0001226029170748815,0.00016495937732826448
-0.3309750919646702,0.81,2.0,38.0,-7.201954108605308e-05,7.792860434319043e-05,-0.0001328527843536186,0.00015421805999004434
-0.3309750919646702,0.87,2.0,27.0,-6.314894098119592e-05,2.9323578814772506e-05,-0.00015541045162983892,4.9074370497992845e-05
-0.3309750919646702,0.93,2.0,34.0,-1.2522258864887169e-05,8.62389898419365e-06,-2.7075026619772485e-05,1.627773215705045e-05
-0.4204887431174353,0.21,2.0,10.0,-0.0012579350384458409,0.0011283228744137042,-0.002595835385755674,0.002189053098697233
-0.4204887431174353,0.27,2.0,19.0,-0.0006099911697533178,0.0006087158656216561,-0.0011803557440720654,0.0011741404299282121
-0.4204887431174353,0.33,2.0,41.0,-0.0005223937773042691,0.0004711068122108117,-0.0010254029500079372,0.000903088585622994
-0.4204887431174353,0.39,2.0,50.0,-0.00034288175539163353,0.00030550813497296105,-0.0006743726480403729,0.0006056526216803415
-0.4204887431174353,0.45,2.0,52.0,-0.00025308502021873706,0.00019840765793371117,-0.0005063083356420238,0.0003812886168111664
-0.4204887431174353,0.51,2.0,45.0,-0.00020439173693414056,0.00017902441212278036,-0.00041339579628026134,0.00034768454065779735
-0.4204887431174353,0.57,2.0,51.0,-0.00012030075111484561,9.840115023056382e-05,-0.0002570489746418995,0.000181288138130511
-0.4204887431174353,0.63,2.0,40.0,-9.865111891354529e-05,8.820767466994395e-05,-0.0001891569630202446,0.00017563197201262703
-0.4204887431174353,0.69,2.0,53.0,-7.104286137156246e-05,8.19225289172631e-05,-0.00013779129758839708,0.00016430443171925585
-0.4204887431174353,0.75,2.0,40.0,-7.928255697546142e-05,9.284060022685621e-05,-0.0001474795016003185,0.00020016036822691538
-0.4204887431174353,0.81,2.0,38.0,-7.979619083937897e-05,9.35668526278749e-05,-0.00015513438523740916,0.00018432401848304293
-0.4204887431174353,0.87,2.0,27.0,-6.89823676850334e-05,3.623394183790329e-05,-0.00016660560734147245,6.233324672275514e-05
-0.4204887431174353,0.93,2.0,34.0,-1.9147420559192155e-05,1.3697116278091e-05,-4.108016284454005e-05,2.4491599682443873e-05
-0.5342117500110048,0.21,2.0,10.0,-0.002026059151780013,0.001650788241598581,-0.003845550560883962,0.00328865593464024
-0.5342117500110048,0.27,2.0,19.0,-0.0009733718558898499,0.0009470721588208165,-0.0019860473693617195,0.001835864000135082
-0.5342117500110048,0.33,2.0,41.0,-0.0007771462239213652,0.0007555828562766817,-0.0015839073616907306,0.001418157775934119
-0.5342117500110048,0.39,2.0,50.0,-0.000523627470487267,0.0005098879059690334,-0.0010990364383723853,0.0009575882957311211
-0.5342117500110048,0.45,2.0,53.0,-0.0003682800869036045,0.0003080397515448158,-0.0007449570259772968,0.0005948570138923781
-0.5342117500110048,0.51,2.0,44.0,-0.0003194727431890163,0.00028564821851902476,-0.0006652135299471643,0.0005449674808140366
-0.5342117500110048,0.57,2.0,53.0,-0.0001784804228799501,0.0001457184120755409,-0.0003683025518026564,0.0002709635052374068
-0.5342117500110048,0.63,2.0,39.0,-0.0001444242590917607,0.00013383332758224172,-0.0003020838442247523,0.00025141068463070703
-0.5342117500110048,0.69,2.0,52.0,-8.772802163263753e-05,0.00010243910926024831,-0.00018062357952534122,0.0002115620487309636
-0.5342117500110048,0.75,2.0,42.0,-9.56743940003147e-05,0.00011341030858529372,-0.00017808212928037187,0.000234110112343856
-0.5342117500110048,0.81,2.0,36.0,-0.00010159493337647878,0.00011279896562964711,-0.00018817207968889458,0.00022786454466494838
-0.5342117500110048,0.87,2.0,27.0,-8.307386930700799e-05,4.569101938706377e-05,-0.00018396201871522427,8.201725243225382e-05
-0.5342117500110048,0.93,2.0,34.0,-3.091499631237778e-05,1.8554047747084436e-05,-6.590487005584146e-05,3.3989059612932886e-05
-0.678691638054321,0.21,2.0,10.0,-0.002606266028792428,0.002441423025541486,-0.0053491030626913365,0.004714602412305463
-0.678691638054321,0.27,2.0,19.0,-0.001416026110013144,0.001483491239981628,-0.00289411135371915,0.002664722161905715
-0.678691638054321,0.33,2.0,42.0,-0.001116607053511325,0.0011543939436140533,-0.0023298869374757023,0.00214000727258437
-0.678691638054321,0.39,2.0,50.0,-0.0008402077931774984,0.000756330621842002,-0.0016515404095431552,0.0014786466870694906
-0.678691638054321,0.45,2.0,53.0,-0.0005488627758325195,0.0004485948910883882,-0.001124708706309847,0.0008773909573009265
-0.678691638054321,0.51,2.0,47.0,-0.00048793247780031494,0.00043009699642796985,-0.0009831838484551582,0.0008343137696679366
-0.678691638054321,0.57,2.0,50.0,-0.00028408263616493107,0.00023792216753106108,-0.0005785743867754303,0.0004516396015592349
-0.678691638054321,0.63,2.0,39.0,-0.0002239772109488715,0.00018951080138834896,-0.00047399023261029716,0.00034735192782749287
-0.678691638054321,0.69,2.0,52.0,-0.000116724638526462,0.00013917600937062304,-0.0002274084121688368,0.00027626331232326356
-0.678691638054321,0.75,2.0,42.0,-0.00012545563324565723,0.00014639461388533975,-0.00023550529918140478,0.00029502413466147713
-0.678691638054321,0.81,2.0,34.0,-0.00012992349138431418,0.00014695685794429713,-0.0002457628451181749,0.0003107275781853798
-0.678691638054321,0.87,2.0,28.0,-0.00010966493909543012,7.264578806577566e-05,-0.00023169934449792558,0.00013018743183694368
-0.678691638054321,0.93,2.0,34.0,-5.945427044262045e-05,3.422120543610511e-05,-0.00013738203207617797,6.13245952630651e-05
-0.862246739341456,0.21,2.0,10.0,-0.0035301898055387485,0.003106533928646027,-0.007248138886519448,0.0060612467275179835
-0.862246739341456,0.27,2.0,19.0,-0.0020866350596939,0.002042660536893937,-0.00425008344009287,0.003767696845291319
-0.862246739341456,0.33,2.0,42.0,-0.0016965266129328432,0.001549273217541579,-0.0033190365999898348,0.0032489831328683934
-0.862246739341456,0.39,2.0,50.0,-0.0011804014530770594,0.001141404828099741,-0.002430565071883855,0.0021140037845031167
-0.862246739341456,0.45,2.0,54.0,-0.0008169747573188375,0.000687598427860739,-0.0016933991912937664,0.001287640584697009
-0.862246739341456,0.51,2.0,47.0,-0.0007464072365833179,0.000746833589844233,-0.0015370697826439853,0.0013464410185433573
-0.862246739341456,0.57,2.0,50.0,-0.00039726965537880456,0.0003433524046525604,-0.0007820866289550242,0.0006481441838997052
-0.862246739341456,0.63,2.0,38.0,-0.00035522521950073657,0.000297955584508661,-0.000746408652552706,0.0005421298226369824
-0.862246739341456,0.69,2.0,52.0,-0.0001608475102944926,0.00018977784657595078,-0.00031581694427667255,0.0003742265546576016
-0.862246739341456,0.75,2.0,42.0,-0.00017006978242757923,0.0002007516229862651,-0.00034139795330185956,0.00039232068714238426
-0.862246739341456,0.81,2.0,34.0,-0.0001779492163385337,0.00018928306029599988,-0.0003330815885148533,0.00038997948824122565
-0.862246739341456,0.87,2.0,28.0,-0.0001609728919369174,0.00011610865973616376,-0.00034871772427658154,0.00020732750388982837
-0.862246739341456,0.93,2.0,34.0,-0.00010893251162721375,6.361803990217554e-05,-0.00024294364952345541,0.00011013594712264885
-1.0954451150103393,0.21,2.0,10.0,-0.004232780711040874,0.0038149065570147844,-0.008226375219285152,0.007707453852882122
-1.0954451150103393,0.27,2.0,20.0,-0.002617894967055277,0.0025080578620608877,-0.005329736198634604,0.004751034042182265
-1.0954451150103393,0.33,2.0,43.0,-0.002251020218215489,0.0021028112528181965,-0.004628037723523755,0.004251326582789841
-1.0954451150103393,0.39,2.0,48.0,-0.0016872730295533272,0.0016502438421812445,-0.003381397058580083,0.003209488025770931
-1.0954451150103393,0.45,2.0,54.0,-0.0012429987684865966,0.000978518991000086,-0.002458836643151774,0.0019220104090623218
-1.0954451150103393,0.51,2.0,49.0,-0.0011852321081835305,0.0010138631245811516,-0.0022107054856635375,0.0020572531205396566
-1.0954451150103393,0.57,2.0,49.0,-0.0005975073709370041,0.0005417564404590787,-0.00127468996703349,0.0010513471207794836
-1.0954451150103393,0.63,2.0,37.0,-0.0005832959382092444,0.0004523269868116863,-0.0012573886514932722,0.000833990737312558
-1.0954451150103393,0.69,2.0,52.0,-0.0002477625050027711,0.0002638099781001448,-0.0004810960981770928,0.0005171759365954389
-1.0954451150103393,0.75,2.0,44.0,-0.00024885317779043325,0.00027583262015095695,-0.00047247474375731015,0.0005486526422373225
-1.0954451150103393,0.81,2.0,32.0,-0.0002792046950997155,0.0002824602727806265,-0.0005409256624659142,0.00056487866264391
-1.0954451150103393,0.87,2.0,28.0,-0.00024999503959569536,0.000188869996018644,-0.0005528607682409348,0.00033998348932081377
-1.0954451150103393,0.93,2.0,34.0,-0.00018673166675033996,0.00010496430502794144,-0.0003988227804317645,0.0001917150906368579
-1.3917130042341714,0.21,2.0,10.0,-0.0035044532303253047,0.0037114404616233674,-0.007326196116698358,0.006921592066935888
-1.3917130042341714,0.27,2.0,20.0,-0.0028571005091706154,0.002689024943106403,-0.005863980384540738,0.005252365533508559
-1.3917130042341714,0.33,2.0,43.0,-0.0026738248746813894,0.0025059101202232112,-0.005359528249651205,0.004902415735552384
-1.3917130042341714,0.39,2.0,47.0,-0.0021466797455981126,0.0020127523928105307,-0.004300565572225162,0.003915779169131238
-1.3917130042341714,0.45,2.0,56.0,-0.0015931976517971635,0.0014761027988046639,-0.00328154287519292,0.00276616177534219
-1.3917130042341714,0.51,2.0,50.0,-0.0015458233293207072,0.0014435399595739708,-0.003202788941203038,0.0026859869633227753
-1.3917130042341714,0.57,2.0,50.0,-0.0008692729954159623,0.0007586484784527823,-0.0017673181542797812,0.0014571438513406008
-1.3917130042341714,0.63,2.0,34.0,-0.0009192598966609196,0.0007211206490104591,-0.0019894040532058236,0.001291957630097611
-1.3917130042341714,0.69,2.0,55.0,-0.0003154113581969754,0.0003111405689416743,-0.0006123071991514696,0.0006268541845813638
-1.3917130042341714,0.75,2.0,42.0,-0.0003788101086969775,0.0003669760524121863,-0.0007687418090500763,0.000732564767390172
-1.3917130042341714,0.81,2.0,30.0,-0.0004673724584562279,0.00036092185036283727,-0.0009473855295469121,0.0007285235322031871
-1.3917130042341714,0.87,2.0,29.0,-0.0004388473194585141,0.00031310016893831193,-0.0009204555015449081,0.0005762668284195696
-1.3917130042341714,0.93,2.0,34.0,-0.0002955455022953944,0.0001858261008142274,-0.0006542686610391552,0.0003265713270680147
-1.768107830884992,0.21,2.0,10.0,-0.0027349984866593016,0.0029140710398905026,-0.005218442414875833,0.005714315228125865
-1.768107830884992,0.27,2.0,20.0,-0.0028895364172625538,0.003495927393348351,-0.005558903143175529,0.006939772107430485
-1.768107830884992,0.33,2.0,43.0,-0.0025138705455548154,0.0023188219942220684,-0.004745970004176203,0.004611693704579836
-1.768107830884992,0.39,2.0,48.0,-0.002356394215990176,0.002178472334388688,-0.004819310122879315,0.004141000029722482
-1.768107830884992,0.45,2.0,57.0,-0.0018586611191037067,0.0016375091623308624,-0.0038241690287838226,0.003032191996683849
-1.768107830884992,0.51,2.0,49.0,-0.0020002004635816454,0.0017884986743103937,-0.003882294141634898,0.003539525473437611
-1.768107830884992,0.57,2.0,50.0,-0.0011459969350294562,0.0010323616206609288,-0.0023835537569604,0.001983923916530516
-1.768107830884992,0.63,2.0,37.0,-0.0011928088544293997,0.0009348176821372842,-0.0025191304379860112,0.0016578140177989688
-1.768107830884992,0.69,2.0,51.0,-0.0004360945231588697,0.0004431653845126,-0.0008625051484431463,0.0008395596258658513
-1.768107830884992,0.75,2.0,40.0,-0.0006128933965060183,0.0005722199884177817,-0.0013339544486732037,0.0010306589628134404
-1.768107830884992,0.81,2.0,32.0,-0.0007129180457395733,0.0005281341500320167,-0.0015449299109187341,0.0009418423969205518
-1.768107830884992,0.87,2.0,29.0,-0.0007219141116417668,0.000519691445714421,-0.0015839068513405006,0.0009511443589269404
-1.768107830884992,0.93,2.0,34.0,-0.000507292919638162,0.0003086002630485701,-0.001126705522585093,0.0005720885061211195
-2.2463002732069,0.21,2.0,10.0,-0.0020428492423140666,0.0022731030402106224,-0.003738646547669336,0.0045712657958155555
-2.2463002732069,0.27,2.0,20.0,-0.002473011180918629,0.003116287385362662,-0.004933525164764365,0.0062215415890970165
-2.2463002732069,0.33,2.0,43.0,-0.0019964267286237706,0.0018405631019199219,-0.00382158794879696,0.0036214216953693594
-2.2463002732069,0.39,2.0,51.0,-0.002139519889626431,0.0019830890252843054,-0.004158530328028188,0.0038572823572324473
-2.2463002732069,0.45,2.0,59.0,-0.001864412070540409,0.0016436810546607593,-0.0037241111686591253,0.003140586320348235
-2.2463002732069,0.51,2.0,45.0,-0.0023157112622926856,0.002220227355530345,-0.0045089573626841415,0.004232164306573803
-2.2463002732069,0.57,2.0,51.0,-0.0013283648145469749,0.0011850351938834654,-0.0025936423927279155,0.0022428859152691044
-2.2463002732069,0.63,2.0,38.0,-0.0014409831385168333,0.0011820421914941388,-0.002917512662320189,0.0022630760842469746
-2.2463002732069,0.69,2.0,48.0,-0.0005906163793196113,0.0005604180399801516,-0.0011936194029023243,0.0011021739521734606
-2.2463002732069,0.75,2.0,40.0,-0.0009170435351380597,0.0007562183229077684,-0.001924276054869891,0.001371229286862208
-2.2463002732069,0.81,2.0,33.0,-0.0011144052048564395,0.0007588424981175002,-0.002360494930758321,0.0013910215843330018
-2.2463002732069,0.87,2.0,28.0,-0.0011690351219017898,0.0008146877592928094,-0.002482648957573341,0.0015155008270213942
-2.2463002732069,0.93,2.0,34.0,-0.000808123153689532,0.0005065288319423966,-0.0017111452708222523,0.000974725615587555
-2.8538219384978536,0.21,2.0,10.0,-0.0018393164625305524,0.002078555941741073,-0.0034556291374723313,0.004205157537121277
-2.8538219384978536,0.27,2.0,22.0,-0.002375682060541249,0.002378982514855782,-0.004507544227741392,0.0049166030573392265
-2.8538219384978536,0.33,2.0,43.0,-0.001483464161966723,0.0014323040333165304,-0.0029648789653343045,0.0028095814913622315
-2.8538219384978536,0.39,2.0,48.0,-0.0017890194282804098,0.0016586351576200807,-0.003563546586365067,0.00330413976469844
-2.8538219384978536,0.45,2.0,62.0,-0.0015074210077042063,0.0013664480277204387,-0.003008467092789591,0.0025824652260252627
-2.8538219384978536,0.51,2.0,47.0,-0.0019104784941415738,0.0018563558237521987,-0.00404735622591266,0.0034685358694243637
-2.8538219384978536,0.57,2.0,48.0,-0.0012989117396534637,0.0012329735993742595,-0.002671064707088078,0.002350125380850421
-2.8538219384978536,0.63,2.0,39.0,-0.0014838184582138465,0.001151618041314185,-0.0029457131335398888,0.0023277865504251287
-2.8538219384978536,0.69,2.0,49.0,-0.0007009930620871243,0.0006852072424469032,-0.0014214658104259234,0.0013257968942707182
-2.8538219384978536,0.75,2.0,37.0,-0.0012744362162405798,0.0010077802902443878,-0.002806386484307393,0.0017939370390673431
-2.8538219384978536,0.81,2.0,32.0,-0.0015767925696202336,0.0012184519139555891,-0.0035117655560475895,0.00209916981277306
-2.8538219384978536,0.87,2.0,29.0,-0.001640411252444612,0.0011790556553003663,-0.003406510771668727,0.0021567329745856806
-2.8538219384978536,0.93,2.0,34.0,-0.0011076152902472463,0.0007842364950458384,-0.0023907678800299467,0.001435039794817545
-3.625650476828135,0.21,2.0,11.0,-0.0015885835928041762,0.0016605937025153232,-0.0029687813823139134,0.0034170334607351413
-3.625650476828135,0.27,2.0,21.0,-0.001770246591250697,0.0017670299303675565,-0.003455493721842809,0.003428940588015076
-3.625650476828135,0.33,2.0,47.0,-0.001165656349362763,0.0013211379608637842,-0.002306127844035323,0.002567164600061076
-3.625650476828135,0.39,2.0,50.0,-0.0014299631459917732,0.0013487063821109272,-0.00276482548371859,0.002604841669892706
-3.625650476828135,0.45,2.0,60.0,-0.0010944670591012998,0.0010243957530670868,-0.0022471819353217766,0.001860449327940411
-3.625650476828135,0.51,2.0,47.0,-0.0014911693398280456,0.0013745906947705752,-0.002964649812616651,0.0026771815554076316
-3.625650476828135,0.57,2.0,48.0,-0.0009974803443893617,0.0008758061522731626,-0.001985874077206923,0.0016932838139337963
-3.625650476828135,0.63,2.0,38.0,-0.001134253602787324,0.0009965717058459617,-0.0024851016138286042,0.0018149801974539268
-3.625650476828135,0.69,2.0,46.0,-0.0006354097423906049,0.0006104987772069964,-0.0012657366849957205,0.001228110365243321
-3.625650476828135,0.75,2.0,37.0,-0.0011931375309491724,0.0009656194960883049,-0.00257495100421735,0.0017649213060324826
-3.625650476828135,0.81,2.0,31.0,-0.0022863888719967048,0.0016909578864829546,-0.004937581694683961,0.00311104318399239
-3.625650476828135,0.87,2.0,29.0,-0.0019032842587020141,0.0013160808506413523,-0.003943518194548282,0.002487949600022469
-3.625650476828135,0.93,2.0,35.0,-0.0013485806415918231,0.0011824525606480146,-0.00280540699916418,0.0021747698628346306
-4.6062233956485175,0.21,2.0,9.0,-0.002067093254293945,0.001905554656386539,-0.0041831160660107435,0.003456130123804156
-4.6062233956485175,0.27,2.0,22.0,-0.0016578546521406816,0.0016821374843287963,-0.0033627915381014726,0.0032818563950074526
-4.6062233956485175,0.33,2.0,49.0,-0.0012401056098597257,0.0013215289349069765,-0.0025741759343352187,0.0025068700281675356
-4.6062233956485175,0.39,2.0,55.0,-0.00119305382877156,0.0011963812964771636,-0.002408614373548566,0.002358035961444804
-4.6062233956485175,0.45,2.0,58.0,-0.0010991718071498503,0.0010152778617150452,-0.0020919274418575414,0.002035559196138919
-4.6062233956485175,0.51,2.0,51.0,-0.0010799979307077124,0.0010956673834349026,-0.0022628756560819697,0.002030657777932036
-4.6062233956485175,0.57,2.0,46.0,-0.0010908294132938097,0.0009535731571791307,-0.0022868748804782736,0.0017893000900902228
-4.6062233956485175,0.63,2.0,38.0,-0.001370358901966546,0.0011627634089751634,-0.0029227567026986804,0.0021008558928521485
-4.6062233956485175,0.69,2.0,44.0,-0.0008058146265620639,0.0008072279933565321,-0.0015394620250931165,0.0015631376109629604
-4.6062233956485175,0.75,2.0,33.0,-0.001739309534680404,0.0013524398166401795,-0.0036112264760622885,0.002501260521171655
-4.6062233956485175,0.81,2.0,31.0,-0.0026936440172538227,0.0022297702652248302,-0.005462772304505942,0.004172926962717095
-4.6062233956485175,0.87,2.0,26.0,-0.0027181129459208876,0.0021457934085996767,-0.005759916291484408,0.004016095629845743
-4.6062233956485175,0.93,2.0,38.0,-0.0015446594231773142,0.0014680390721686705,-0.003242006997337828,0.0027310757050598876
-5.85199651930643,0.21,2.0,9.0,-0.002414143783080531,0.0023438647797924825,-0.004826932856633208,0.004416473664603196
-5.85199651930643,0.27,2.0,23.0,-0.0017730645082341934,0.001623577011765488,-0.0033838449515639097,0.0032323216064032052
-5.85199651930643,0.33,2.0,50.0,-0.001376820965650436,0.0013919721533606274,-0.0027522690935401694,0.0027142598156417227
-5.85199651930643,0.39,2.0,59.0,-0.0013364682398042153,0.0014045436490098839,-0.0026559128060586563,0.002683851345664999
-5.85199651930643,0.45,2.0,57.0,-0.0012581026833031561,0.0012465566854261572,-0.0024459728424955523,0.002540067633524779
-5.85199651930643,0.51,2.0,54.0,-0.0012056392805907285,0.0011994677472386653,-0.0024750562477128873,0.0022899098238548447
-5.85199651930643,0.57,2.0,46.0,-0.0012861148743062685,0.0012454351709920446,-0.0026620604502541204,0.0022977565115334295
-5.85199651930643,0.63,2.0,34.0,-0.0020018645503077186,0.001981746124681235,-0.004031658499917842,0.003873556549840042
-5.85199651930643,0.69,2.0,42.0,-0.001223766298228224,0.0011295968574193667,-0.0024301104767251503,0.0021758189428244088
-5.85199651930643,0.75,2.0,31.0,-0.0021697387151890695,0.001875909121851508,-0.004552693056933085,0.0034012586751039024
-5.85199651930643,0.81,2.0,28.0,-0.0032758615522756594,0.0030752385452531574,-0.006772146217340058,0.00584353554450129
-5.85199651930643,0.87,2.0,22.0,-0.0034205716704356955,0.0031074511147726725,-0.007185118444292895,0.005743995720477826
-5.85199651930643,0.93,2.0,43.0,-0.002074628070814694,0.0019589877769783165,-0.003991633707694616,0.003963639846800919
-7.43469439504961,0.21,2.0,11.0,-0.0015363336812358028,0.0014003771500331115,-0.002993216902382523,0.002701892639006744
-7.43469439504961,0.27,2.0,19.0,-0.0018853355492489676,0.0015529220208633323,-0.0038738899606755796,0.0029982219123828925
-7.43469439504961,0.33,2.0,49.0,-0.0012241671245514492,0.001276046864800994,-0.002444485223452355,0.002404198459293131
-7.43469439504961,0.39,2.0,51.0,-0.0015962391438436227,0.0015960643508456606,-0.003164878204883189,0.003136328304333664
-7.43469439504961,0.45,2.0,65.0,-0.001300868345740061,0.0013931174986372655,-0.00266916964570868,0.002772453599756197
-7.43469439504961,0.51,2.0,52.0,-0.0014596741309949048,0.001513295091049725,-0.0027831581498475237,0.0030424703452566226
-7.43469439504961,0.57,2.0,49.0,-0.0015101910809033666,0.0014132130081136406,-0.002874952255545797,0.0028530591358920374
-7.43469439504961,0.63,2.0,37.0,-0.0020658339123310323,0.0020439469358213293,-0.004063706138057503,0.003971023245357382
-7.43469439504961,0.69,2.0,36.0,-0.0020604364437826423,0.0020321548807521227,-0.003983926294290733,0.003940291133131882
-7.43469439504961,0.75,2.0,33.0,-0.0035076219014464802,0.0030271082437056777,-0.0077410369482992895,0.005558772159788701
-7.43469439504961,0.81,2.0,28.0,-0.004984055333738979,0.004636280165611624,-0.009771351803908672,0.00934233238103407
-7.43469439504961,0.87,2.0,21.0,-0.0039308607551148895,0.004714574249026011,-0.007380966530286359,0.009760716489474023
-7.43469439504961,0.93,2.0,37.0,-0.002327396878282741,0.002254867760321152,-0.004807707545139404,0.004236682628258294
-7.43469439504961,0.99,2.0,12.0,-0.0032861449742904356,0.002680888875809734,-0.006646902827836387,0.005065328395262246
-9.445439785451777,0.21,2.0,6.0,-0.001930202102034188,0.0029559325546686574,-0.0030929855522471295,0.006526794973660229
-9.445439785451777,0.27,2.0,23.0,-0.001827484390966051,0.0012700986490299974,-0.0037743598292599148,0.0023655437571232342
-9.445439785451777,0.33,2.0,45.0,-0.0015992915420737495,0.0015410511253266862,-0.0033306053821533107,0.0029573019217721446
-9.445439785451777,0.39,2.0,57.0,-0.0019374937823669744,0.0019008348469652884,-0.0037906084679712854,0.003677411536029488
-9.445439785451777,0.45,2.0,63.0,-0.0018568250619832862,0.001898680199280491,-0.00374380898163912,0.003736438399597663
-9.445439785451777,0.51,2.0,54.0,-0.002005880669175051,0.0019810490995746896,-0.003866365416023185,0.0040292038214960945
-9.445439785451777,0.57,2.0,48.0,-0.0022086078499232256,0.0021255709770753076,-0.004341607098716965,0.004007816153723381
-9.445439785451777,0.63,2.0,37.0,-0.003199553176206676,0.002883007774681601,-0.006305298953205388,0.005770297711795393
-9.445439785451777,0.69,2.0,35.0,-0.0033803284774645195,0.003473789256243641,-0.006814855394361031,0.006606264472336067
-9.445439785451777,0.75,2.0,32.0,-0.005678114752239864,0.004602536622277334,-0.011793692565227143,0.00861895172440003
-9.445439785451777,0.81,2.0,27.0,-0.007377803950850379,0.006399890988686134,-0.013964476829029281,0.01299015647945716
-9.445439785451777,0.87,2.0,22.0,-0.004303173516873065,0.006572133340179013,-0.007889902546019227,0.014293720277836585
-9.445439785451777,0.93,2.0,34.0,-0.003139751055854938,0.002821230193344661,-0.00649232282019497,0.005602075039393244
-9.445439785451777,0.99,2.0,17.0,-0.0047931151883060154,0.003853563622908143,-0.009540959133737505,0.007594651119299024
-12.000000000000009,0.27,2.0,20.0,-0.0020793090941929964,0.0018246045096491172,-0.004493831793680609,0.0033526871559714155
-12.000000000000009,0.33,2.0,47.0,-0.002029124600504385,0.0020003869318706673,-0.004135061182102966,0.0037877223786403416
-12.000000000000009,0.39,2.0,52.0,-0.0026694521961851715,0.0026537026532691293,-0.00539689155998069,0.005142224955417021
-12.000000000000009,0.45,2.0,66.0,-0.0026735831266235274,0.0026453121351226595,-0.005192383797381099,0.005228265956449525
-12.000000000000009,0.51,2.0,61.0,-0.0028056784920726394,0.0027379213873096418,-0.005286451825633554,0.005470524496881033
-12.000000000000009,0.57,2.0,53.0,-0.0032894482154673444,0.0030741869019564336,-0.006542548768616114,0.005818506026005299
-12.000000000000009,0.63,2.0,37.0,-0.005309934688831259,0.00429049918212042,-0.010288313647121416,0.008914299157702721
-12.000000000000009,0.69,2.0,28.0,-0.008394338514175252,0.007082739573788741,-0.0166288828498509,0.013497532615371005
-12.000000000000009,0.75,2.0,29.0,-0.011461924365104365,0.009663291244349441,-0.023726074632224675,0.01793152143995022
-12.000000000000009,0.81,2.0,25.0,-0.013192132388867276,0.012098742342897663,-0.02685500179904321,0.022698719026375217
-12.000000000000009,0.87,2.0,18.0,-0.009659317531338594,0.01538288985881417,-0.01719837107493336,0.035868333133599356
-12.000000000000009,0.93,2.0,33.0,-0.005145948751736306,0.005258425460021517,-0.009963286733676599,0.010326354061830217
-12.000000000000009,0.99,2.0,28.0,-0.005228816715091456,0.005086948962556074,-0.01023947189478728,0.0100493081173909
-0.0999999999988488,0.27,3.0,7.0,-2.681559676825139e-05,3.108844723991625e-05,-4.798261214351529e-05,6.355984308410125e-05
-0.0999999999988488,0.33,3.0,24.0,-1.5480486507821534e-05,1.3399197451647607e-05,-3.146530690431482e-05,2.5312523103687097e-05
-0.0999999999988488,0.39,3.0,31.0,-1.1204786221139247e-05,1.0711977790530079e-05,-2.1387456682225643e-05,2.1350383868529303e-05
-0.0999999999988488,0.45,3.0,39.0,-9.82174336901215e-06,9.244310185777368e-06,-2.0096574002172394e-05,1.701097319880552e-05
-0.0999999999988488,0.51,3.0,58.0,-6.302163380587094e-06,5.78017947230152e-06,-1.244808890454324e-05,1.1592850793347784e-05
-0.0999999999988488,0.57,3.0,52.0,-4.162930013813205e-06,3.971843016494976e-06,-7.974432341603128e-06,7.636711163322578e-06
-0.0999999999988488,0.63,3.0,48.0,-4.011725021812664e-06,3.5750509716486993e-06,-8.373316770357365e-06,6.676095395146546e-06
-0.0999999999988488,0.69,3.0,55.0,-1.0107502175358234e-05,1.3720110307208389e-05,-1.8440268034120502e-05,2.9466693692788537e-05
-0.0999999999988488,0.75,3.0,42.0,-6.872554158513457e-06,1.2559459054014942e-05,-1.2739419618417619e-05,2.7774681208633327e-05
-0.0999999999988488,0.81,3.0,37.0,-1.8477641711617918e-05,2.033487173464771e-05,-3.345109429444903e-05,4.291122960794054e-05
-0.0999999999988488,0.87,3.0,41.0,-2.0444236133226697e-05,2.120031342144341e-05,-4.143446624311202e-05,4.125167054070362e-05
-0.0999999999988488,0.93,3.0,49.0,-1.1160844179085347e-05,5.504494905830073e-06,-2.3642796915723842e-05,5.976435093417638e-06
-0.0999999999988488,0.99,3.0,17.0,-7.191073257123115e-08,8.770117302969711e-08,-1.3982379020980932e-07,1.8060613155340347e-07
-0.1270454343323782,0.27,3.0,7.0,-3.60376493266606e-05,3.896842107532967e-05,-6.596627131389661e-05,8.42825330242507e-05
-0.1270454343323782,0.33,3.0,24.0,-2.179361583025389e-05,1.9009179759450493e-05,-4.352055908725708e-05,3.477329033707376e-05
-0.1270454343323782,0.39,3.0,31.0,-1.4368474784104281e-05,1.4376787947431192e-05,-2.8699734535833024e-05,2.7209365346879912e-05
-0.1270454343323782,0.45,3.0,39.0,-1.3903506252938898e-05,1.217609992577871e-05,-2.8906133867025423e-05,2.2577092575161954e-05
-0.1270454343323782,0.51,3.0,58.0,-8.045511372303049e-06,7.599260488270657e-06,-1.6229026110472433e-05,1.4299202013990197e-05
-0.1270454343323782,0.57,3.0,52.0,-5.396862533977609e-06,4.9405027917287965e-06,-1.07057583317218e-05,9.477182991915557e-06
-0.1270454343323782,0.63,3.0,48.0,-4.962193131238546e-06,4.345974686640541e-06,-1.0026953900636106e-05,8.236239354830071e-06
-0.1270454343323782,0.69,3.0,55.0,-1.0514070634338466e-05,1.4658914370643057e-05,-1.9318725442784424e-05,2.9667466423731173e-05
-0.1270454343323782,0.75,3.0,42.0,-7.4742166250225624e-06,1.2955762048972602e-05,-1.2914113882123043e-05,2.941752464626817e-05
-0.1270454343323782,0.81,3.0,37.0,-1.7927473400232477e-05,2.2717943360059427e-05,-3.364693624223724e-05,4.641742602262814e-05
-0.1270454343323782,0.87,3.0,41.0,-2.1119306180768973e-05,2.261521952301718e-05,-4.249881046975777e-05,4.31765095075584e-05
-0.1270454343323782,0.93,3.0,49.0,-1.1316264311452224e-05,5.683056833581002e-06,-2.4529198512341136e-05,6.3187697395986e-06
-0.1270454343323782,0.99,3.0,17.0,-4.505030262562042e-08,5.69223933217602e-08,-8.07707731417372e-08,1.1460410576091259e-07
-0.1614054238468478,0.27,3.0,7.0,-5.3030931798548855e-05,5.356917275150301e-05,-9.132533154760598e-05,0.00011596583500189145
-0.1614054238468478,0.33,3.0,24.0,-3.125202418310596e-05,2.8243799711660727e-05,-6.573017494124932e-05,5.2415953522175706e-05
-0.1614054238468478,0.39,3.0,31.0,-2.1896122407423934e-05,2.013370025876292e-05,-4.243924259413331e-05,4.068985396990304e-05
-0.1614054238468478,0.45,3.0,39.0,-2.130676907733873e-05,1.7499651042878895e-05,-4.2594420397361466e-05,3.428907238942159e-05
-0.1614054238468478,0.51,3.0,58.0,-1.1316875785969854e-05,1.0567298293464096e-05,-2.2391655242000177e-05,1.9971816724415676e-05
-0.1614054238468478,0.57,3.0,52.0,-8.060650568384146e-06,7.098149049205456e-06,-1.564159515130047e-05,1.3681484998956855e-05
-0.1614054238468478,0.63,3.0,48.0,-7.057300144193005e-06,5.592924197111138e-06,-1.4471483398682225e-05,1.0522297351019474e-05
-0.1614054238468478,0.69,3.0,55.0,-1.1147949131792707e-05,1.5561865603311978e-05,-2.0975430109726282e-05,3.22682274171823e-05
-0.1614054238468478,0.75,3.0,42.0,-7.896921859601762e-06,1.3785396485919789e-05,-1.368074268048506e-05,3.268785799933585e-05
-0.1614054238468478,0.81,3.0,37.0,-1.9542257667684203e-05,2.4020957142324993e-05,-3.625262823719243e-05,4.774795358131269e-05
-0.1614054238468478,0.87,3.0,41.0,-2.278140090784261e-05,2.3783252147203415e-05,-4.579532554466491e-05,4.634363013889547e-05
-0.1614054238468478,0.93,3.0,49.0,-1.2193383789991051e-05,6.040479476275631e-06,-3.18341135024824e-05,6.820230893471579e-06
-0.1614054238468478,0.99,3.0,17.0,-1.5367208689212326e-07,1.2389410999409942e-07,-3.06578701807083e-07,2.45420415380804e-07
-0.2050582217603373,0.27,3.0,7.0,-7.093639449608413e-05,8.494531635614406e-05,-0.00013058775429315112,0.0001699977989769572
-0.2050582217603373,0.33,3.0,24.0,-5.639474392887577e-05,4.519777343106056e-05,-0.00011157811079076698,8.763719873858367e-05
-0.2050582217603373,0.39,3.0,31.0,-3.615502586958332e-05,3.6229037778802366e-05,-7.413626761179975e-05,6.748660588930845e-05
-0.2050582217603373,0.45,3.0,39.0,-3.524586168072364e-05,2.9983079600416696e-05,-7.18208109175789e-05,5.813326768361169e-05
-0.2050582217603373,0.51,3.0,58.0,-1.8045014672248314e-05,1.7280774135579117e-05,-3.6420793091990214e-05,3.313372554394916e-05
-0.2050582217603373,0.57,3.0,52.0,-1.3394654799715078e-05,1.1752348141047717e-05,-2.6900097458665334e-05,2.296289135598787e-05
-0.2050582217603373,0.63,3.0,48.0,-1.1643904565260286e-05,9.659372175839304e-06,-2.3530331873486225e-05,1.773691337761014e-05
-0.2050582217603373,0.69,3.0,55.0,-1.3711577705526249e-05,1.9075723105491764e-05,-2.6931890805299832e-05,3.8404061483479414e-05
-0.2050582217603373,0.75,3.0,42.0,-9.592921242910586e-06,1.639678216651131e-05,-1.6847023506376055e-05,3.7291630698393975e-05
-0.2050582217603373,0.81,3.0,37.0,-2.308000960523831e-05,2.8240513421188062e-05,-4.232947499106318e-05,5.831075619141127e-05
-0.2050582217603373,0.87,3.0,41.0,-2.800379276094033e-05,2.686204321071374e-05,-5.3089423546464495e-05,5.264775811901159e-05
-0.2050582217603373,0.93,3.0,49.0,-1.3441766869709135e-05,6.9456685358205676e-06,-3.190761647100918e-05,8.216427895618847e-06
-0.2050582217603373,0.99,3.0,17.0,-5.054073572496998e-07,4.0945222543112476e-07,-1.0398722529499404e-06,8.047516226203361e-07
-0.2605171084699756,0.27,3.0,7.0,-0.00014814442604600092,0.00012248440449399593,-0.00028140591555311393,0.00025748354159925235
-0.2605171084699756,0.33,3.0,24.0,-9.395722024935175e-05,8.439001579825089e-05,-0.00020291565212355456,0.00016087081723483175
-0.2605171084699756,0.39,3.0,31.0,-6.85518926074447e-05,6.488673498938164e-05,-0.0001343942830815659,0.00012627786308894197
-0.2605171084699756,0.45,3.0,39.0,-6.800628073482856e-05,5.526523757350116e-05,-0.0001329342506694507,0.00011016500332979057
-0.2605171084699756,0.51,3.0,58.0,-3.393921131704637e-05,3.087427553664945e-05,-6.583260587796125e-05,6.231768955331991e-05
-0.2605171084699756,0.57,3.0,52.0,-2.3963104699817332e-05,2.197357410289966e-05,-4.9231371334778786e-05,4.368505332351236e-05
-0.2605171084699756,0.63,3.0,48.0,-2.0634891652586803e-05,1.7012193029574237e-05,-4.3239141242383665e-05,3.239788081572336e-05
-0.2605171084699756,0.69,3.0,55.0,-2.215624132199055e-05,2.7025194896357116e-05,-4.062979663228489e-05,5.987879739927237e-05
-0.2605171084699756,0.75,3.0,42.0,-1.3844068733138676e-05,2.33993581637287e-05,-2.4224300398179097e-05,5.432016245954985e-05
-0.2605171084699756,0.81,3.0,37.0,-3.526662342402058e-05,4.06273593922003e-05,-6.311646541134545e-05,8.575474925752356e-05
-0.2605171084699756,0.87,3.0,41.0,-4.014839487248581e-05,3.971918901511603e-05,-7.612243932387516e-05,8.077959211438841e-05
-0.2605171084699756,0.93,3.0,49.0,-1.9904369621767192e-05,9.513895213661749e-06,-4.494822643985226e-05,1.1997774513656306e-05
-0.2605171084699756,0.99,3.0,17.0,-5.937451493452293e-07,4.963507966501188e-07,-1.2193542535898747e-06,9.151224178843458e-07
-0.3309750919644821,0.27,3.0,7.0,-0.00030210977609281193,0.00023701406873756684,-0.0006121678139747574,0.00043135101515001656
-0.3309750919644821,0.33,3.0,24.0,-0.0001608307892686606,0.00014214035641353737,-0.00031918976906721144,0.00027384338835755094
-0.3309750919644821,0.39,3.0,31.0,-0.00012151079354868757,0.00011064676192075554,-0.0002358572394228275,0.00021615744471631564
-0.3309750919644821,0.45,3.0,39.0,-0.00011218540738344838,9.831601262922054e-05,-0.00023765809063290322,0.0001929650765267197
-0.3309750919644821,0.51,3.0,58.0,-5.7513382892733615e-05,5.593030025526924e-05,-0.00011741126336004981,0.00010501912025002128
-0.3309750919644821,0.57,3.0,52.0,-4.3585973425335364e-05,3.7674323395312e-05,-8.520904842377942e-05,7.574181059152843e-05
-0.3309750919644821,0.63,3.0,48.0,-3.644122288991956e-05,2.9652172107166108e-05,-7.521528810966153e-05,5.640819631428877e-05
-0.3309750919644821,0.69,3.0,55.0,-3.234549607264952e-05,3.9085534623357116e-05,-6.080295284768001e-05,8.041357559252422e-05
-0.3309750919644821,0.75,3.0,42.0,-1.9280937604655345e-05,3.24188276261083e-05,-3.330369267179091e-05,7.596577087124638e-05
-0.3309750919644821,0.81,3.0,37.0,-4.740423283055031e-05,5.7278003881809475e-05,-8.940515203007046e-05,0.0001196368267939001
-0.3309750919644821,0.87,3.0,41.0,-5.1322952492237495e-05,5.588799967635688e-05,-0.00010399330743530011,0.00010818293097238776
-0.3309750919644821,0.93,3.0,49.0,-2.5268486701011686e-05,1.2584407065867998e-05,-6.015743606544204e-05,1.6896870389875285e-05
-0.3309750919644821,0.99,3.0,17.0,-1.0229092022786905e-06,7.967159903127677e-07,-2.0446784745283806e-06,1.5160208937460118e-06
-0.4204887431176252,0.27,3.0,7.0,-0.0005745458642293998,0.00050435863013181,-0.0011070352729907354,0.0009599064837011258
-0.4204887431176252,0.33,3.0,24.0,-0.00026054811920616695,0.0002449296624375592,-0.0005165776824957882,0.0004994701632659886
-0.4204887431176252,0.39,3.0,31.0,-0.00020206682067826226,0.00020298026271689393,-0.0004097195470727158,0.0003796804721915205
-0.4204887431176252,0.45,3.0,39.0,-0.00019631466019901956,0.00016863353424662967,-0.0003915331324478951,0.0003222808246771464
-0.4204887431176252,0.51,3.0,58.0,-9.807167675739898e-05,9.156612918001882e-05,-0.00020081090768101992,0.00017336879946475945
-0.4204887431176252,0.57,3.0,52.0,-7.385537234087911e-05,6.299418099724664e-05,-0.00015050397753863282,0.0001245501740544794
-0.4204887431176252,0.63,3.0,48.0,-6.35621027163203e-05,5.0303485442008554e-05,-0.0001232991733850566,9.626623875468423e-05
-0.4204887431176252,0.69,3.0,55.0,-4.711020889786534e-05,5.202003300523924e-05,-8.886078203625136e-05,0.0001076470373168684
-0.4204887431176252,0.75,3.0,42.0,-2.48715505466499e-05,4.401729772266306e-05,-4.572129087609175e-05,0.00010064850147460449
-0.4204887431176252,0.81,3.0,37.0,-6.270049439903323e-05,7.286055673900161e-05,-0.0001185232289038087,0.0001596954885256123
-0.4204887431176252,0.87,3.0,41.0,-6.914477342423887e-05,7.190290115021062e-05,-0.0001360825993080921,0.00014019722730717376
-0.4204887431176252,0.93,3.0,49.0,-3.234799306136191e-05,1.5537164952650352e-05,-8.004416368080876e-05,2.334216409696762e-05
-0.4204887431176252,0.99,3.0,17.0,-1.7132315104920092e-06,1.3949508828206937e-06,-3.536721835230276e-06,2.54301691489411e-06
-0.5342117500110911,0.27,3.0,7.0,-0.0009766876950803663,0.0009700633479732586,-0.0019696282873185823,0.001720796577611578
-0.5342117500110911,0.33,3.0,24.0,-0.0004446156845381732,0.00044321899149763757,-0.0008463299558275091,0.0009535028774752129
-0.5342117500110911,0.39,3.0,31.0,-0.0003546743548717795,0.0003183721957806514,-0.0007087625983757049,0.0006207812159643912
-0.5342117500110911,0.45,3.0,39.0,-0.00031753743460673776,0.0002841058264837123,-0.0006513915233678868,0.0005270482796245888
-0.5342117500110911,0.51,3.0,58.0,-0.00016357817824409258,0.0001518112956411842,-0.0003329009258646878,0.00029183484167846156
-0.5342117500110911,0.57,3.0,52.0,-0.00012107722679487348,0.00010513295144069573,-0.00024669304757526234,0.00020345807191585454
-0.5342117500110911,0.63,3.0,48.0,-0.00010226473966733101,7.984582679486592e-05,-0.00021435074139384582,0.00015214110536506596
-0.5342117500110911,0.69,3.0,55.0,-6.89256579946395e-05,7.234288160940056e-05,-0.00013803060961557376,0.00014511321843308221
-0.5342117500110911,0.75,3.0,42.0,-3.50381486923355e-05,5.768247560381009e-05,-6.152124966525618e-05,0.00013109099613915355
-0.5342117500110911,0.81,3.0,37.0,-8.834959412531225e-05,9.769309003444579e-05,-0.00015795313095901364,0.0002046886991412622
-0.5342117500110911,0.87,3.0,41.0,-9.401083476591609e-05,9.471831543980702e-05,-0.000176144760713503,0.0001901869835209677
-0.5342117500110911,0.93,3.0,49.0,-4.5083326102779534e-05,2.0048516601944086e-05,-0.00010603569379597061,3.335861306956462e-05
-0.5342117500110911,0.99,3.0,17.0,-2.586595607998593e-06,2.0511148525401146e-06,-5.452583273776079e-06,3.844889664560573e-06
-0.6786916380543364,0.27,3.0,7.0,-0.001516680238176415,0.0012590314497681015,-0.0029209536243107203,0.002485420469285159
-0.6786916380543364,0.33,3.0,24.0,-0.0006712087017928354,0.0007337822378615792,-0.0013158647783518087,0.001507456679371896
-0.6786916380543364,0.39,3.0,31.0,-0.0005659359414162759,0.0005355508543864832,-0.0011653207811771207,0.0010216139423785831
-0.6786916380543364,0.45,3.0,39.0,-0.0005058869611776825,0.0004443639620364333,-0.0010169099266680263,0.0008619698525173291
-0.6786916380543364,0.51,3.0,58.0,-0.00026741290225079043,0.00023707625215660584,-0.0005383863255033073,0.0004674411110254477
-0.6786916380543364,0.57,3.0,52.0,-0.00018829950807038387,0.00017659502005831196,-0.00037165010553620733,0.0003258631339282412
-0.6786916380543364,0.63,3.0,48.0,-0.0001664417994304279,0.00013411699594811615,-0.0003339656594103549,0.00025612531656677107
-0.6786916380543364,0.69,3.0,55.0,-0.00010223175360553707,9.917870484274856e-05,-0.00019941307096707427,0.00019910415888525686
-0.6786916380543364,0.75,3.0,42.0,-4.726942793685873e-05,8.275662301166886e-05,-8.695920121739773e-05,0.0001761540001159005
-0.6786916380543364,0.81,3.0,37.0,-0.00011614522190336915,0.0001405656370560083,-0.0002192306559724885,0.00027964099892664285
-0.6786916380543364,0.87,3.0,42.0,-0.00012453488545668018,0.00013162464557731952,-0.0002502998313858377,0.00025394032214888767
-0.6786916380543364,0.93,3.0,48.0,-5.8608803380948896e-05,2.8564384387342258e-05,-0.0001414690897313456,4.8426222369000126e-05
-0.6786916380543364,0.99,3.0,17.0,-4.525872312804005e-06,3.3663757192307756e-06,-9.042248144798521e-06,6.592737923230159e-06
-0.8622467393414354,0.27,3.0,7.0,-0.0020039351018255524,0.0016435271011775285,-0.003810857369262677,0.0032345695654786427
-0.8622467393414354,0.33,3.0,24.0,-0.001014033064741412,0.0010841323933516674,-0.0020043463191237775,0.0021735629900078383
-0.8622467393414354,0.39,3.0,31.0,-0.0009213431557319367,0.0008120802461190915,-0.0018233878012870737,0.001590859940194268
-0.8622467393414354,0.45,3.0,39.0,-0.000795859431016231,0.0007185480679292449,-0.0016303507698667756,0.0013607757262283583
-0.8622467393414354,0.51,3.0,57.0,-0.0004283059517666465,0.0003827373927868514,-0.000859873226366464,0.0007867568246955678
-0.8622467393414354,0.57,3.0,53.0,-0.00029984068289297036,0.0002903399298188838,-0.0006145286754335734,0.0005679284355662988
-0.8622467393414354,0.63,3.0,48.0,-0.00026635890482833044,0.00022607030429646802,-0.0005428144812751625,0.0004358644316859547
-0.8622467393414354,0.69,3.0,55.0,-0.00015968305476842686,0.0001447337687249466,-0.00030526680634829125,0.00028209610628703144
-0.8622467393414354,0.75,3.0,42.0,-7.290981848242913e-05,0.00011639287753969485,-0.00012961762505806146,0.00025776382516513364
-0.8622467393414354,0.81,3.0,37.0,-0.00015753934162818743,0.0002056935735956577,-0.0003163776007265928,0.00038946937893314526
-0.8622467393414354,0.87,3.0,42.0,-0.00016721548489636952,0.000177200742641389,-0.00032029657424703114,0.00035575680485362135
-0.8622467393414354,0.93,3.0,48.0,-7.848014210007171e-05,3.8113534360961166e-05,-0.00019123845613063604,6.673264373201502e-05
-0.8622467393414354,0.99,3.0,17.0,-6.32987701162252e-06,5.813059871748332e-06,-1.3092066140348086e-05,1.1054468611236262e-05
-1.0954451150103854,0.27,3.0,7.0,-0.002483214905612082,0.002054993637851475,-0.005288550196840729,0.0036484084889297367
-1.0954451150103854,0.33,3.0,24.0,-0.0015205782761161597,0.0014829998978513326,-0.0028723601331386095,0.003103368455241767
-1.0954451150103854,0.39,3.0,31.0,-0.001351617879676792,0.0012899561102366398,-0.002722659742185404,0.0024705088919706325
-1.0954451150103854,0.45,3.0,38.0,-0.0010977258265363599,0.0010789770810398277,-0.0023032642727628958,0.002022438216383855
-1.0954451150103854,0.51,3.0,59.0,-0.0007305136269553351,0.0006902826638105534,-0.0015409764395355873,0.0012455835563726998
-1.0954451150103854,0.57,3.0,52.0,-0.0004854917814088543,0.0004637139949457901,-0.0009544834375774964,0.0009120349193452006
-1.0954451150103854,0.63,3.0,48.0,-0.00046336020894478287,0.0003698459870495637,-0.0009068702431417663,0.0007021580919509456
-1.0954451150103854,0.69,3.0,55.0,-0.00027321259039782573,0.00021745100488802083,-0.0005350606469747618,0.00045746640841733783
-1.0954451150103854,0.75,3.0,42.0,-0.00011672616285755766,0.00018044169655333575,-0.00021143813307264027,0.00040755861982303494
-1.0954451150103854,0.81,3.0,36.0,-0.0002417817532559078,0.00027226637850209264,-0.00045024652986723447,0.000574938164726616
-1.0954451150103854,0.87,3.0,43.0,-0.0002314012032122386,0.00024092730641464734,-0.0004214102069147944,0.0004887634530395871
-1.0954451150103854,0.93,3.0,48.0,-9.516176203547176e-05,5.398324422778243e-05,-0.00022645361643191451,9.138711111260663e-05
-1.0954451150103854,0.99,3.0,17.0,-9.729766861516879e-06,1.2084473519370912e-05,-1.8492269244996112e-05,2.44812908831904e-05
-1.3917130042340478,0.27,3.0,7.0,-0.0025698277613141556,0.0022121836586943703,-0.005614287349749115,0.004078928815111451
-1.3917130042340478,0.33,3.0,24.0,-0.0018355518109897636,0.002011814887392111,-0.0037118137588912146,0.003835777337460689
-1.3917130042340478,0.39,3.0,32.0,-0.001845160304929219,0.0016563849038336994,-0.003576821769841604,0.0033551490036918662
-1.3917130042340478,0.45,3.0,37.0,-0.0016619275980209501,0.0014690078035744806,-0.0032049403736752677,0.002757108068900437
-1.3917130042340478,0.51,3.0,60.0,-0.0011121766767513397,0.000989358803799973,-0.0022037340173131238,0.00186722492487054
-1.3917130042340478,0.57,3.0,51.0,-0.0007619655818414032,0.0006717747605068071,-0.0014106452667782753,0.0013594739067362552
-1.3917130042340478,0.63,3.0,50.0,-0.0006398152221629072,0.0005872107688191566,-0.0013266658227982608,0.0010732452709408323
-1.3917130042340478,0.69,3.0,53.0,-0.00042619998304379366,0.00033734474413646144,-0.0008374433990930428,0.0006378884832841232
-1.3917130042340478,0.75,3.0,42.0,-0.00017570487555509373,0.00023516829306439026,-0.0003131232464252542,0.0005062153878867754
-1.3917130042340478,0.81,3.0,36.0,-0.0003222498333606761,0.0003681608825455085,-0.0006029679701371218,0.0007532671659153768
-1.3917130042340478,0.87,3.0,42.0,-0.00027664766286275653,0.0002939836241334989,-0.0005459531940303065,0.0005848210923566381
-1.3917130042340478,0.93,3.0,49.0,-0.00011899633003783377,8.957783403500635e-05,-0.00027079400010183833,0.000161278840526186
-1.3917130042340478,0.99,3.0,17.0,-2.1257230705151265e-05,2.660873888699462e-05,-4.014737391928108e-05,5.7608998532400504e-05
-1.7681078308850573,0.27,3.0,7.0,-0.002502934532927222,0.0018926077209270632,-0.004991773409986784,0.0035439382756859987
-1.7681078308850573,0.33,3.0,24.0,-0.0020136461024088262,0.0020924839325477803,-0.003920847221953203,0.004297255311569382
-1.7681078308850573,0.39,3.0,31.0,-0.00212379234231343,0.0020704828208801098,-0.0042961785728173356,0.003942664669851626
-1.7681078308850573,0.45,3.0,38.0,-0.0018317938833349882,0.0017677843533035762,-0.003916318524151219,0.0033246322199036228
-1.7681078308850573,0.51,3.0,59.0,-0.0014506707210454528,0.0013090640725232155,-0.0028813160052672333,0.0025350635096257194
-1.7681078308850573,0.57,3.0,52.0,-0.0010712046736150503,0.0009975555554222971,-0.001993868098552132,0.002025726519126957
-1.7681078308850573,0.63,3.0,50.0,-0.0009264664304981503,0.0008094548228002605,-0.0019335121035988195,0.0015329785419940735
-1.7681078308850573,0.69,3.0,51.0,-0.0005811844599484364,0.0004897440646325841,-0.001280491102376572,0.0008821275193854797
-1.7681078308850573,0.75,3.0,44.0,-0.0003033215043096614,0.00041310016242833783,-0.0005777352265553304,0.0008567650188346903
-1.7681078308850573,0.81,3.0,36.0,-0.0004262447892846684,0.0004665774810078618,-0.0008452983290158651,0.000920732751877952
-1.7681078308850573,0.87,3.0,41.0,-0.00034166475828257214,0.00034972060763115446,-0.0006600811806487029,0.0007393821876887565
-1.7681078308850573,0.93,3.0,49.0,-0.00019291128197337822,0.00013992035139698793,-0.000371686290560844,0.00027153385338505497
-1.7681078308850573,0.99,3.0,18.0,-4.029162632610756e-05,4.9526456740274474e-05,-7.380665482799649e-05,0.00010282348834489481
-2.2463002732069746,0.27,3.0,7.0,-0.001922390883394582,0.001778788853785113,-0.00371491688828231,0.003227342577845785
-2.2463002732069746,0.33,3.0,24.0,-0.0016940015886680799,0.0020992426539518643,-0.0034593286964228415,0.004115609133208821
-2.2463002732069746,0.39,3.0,31.0,-0.0022577033399601935,0.00195538983494983,-0.004135700927641244,0.004001536182549058
-2.2463002732069746,0.45,3.0,38.0,-0.0018987776773763843,0.001842351069880063,-0.003943786208685235,0.0034977848391955367
-2.2463002732069746,0.51,3.0,59.0,-0.0016505106506974657,0.0015335635689594125,-0.0032953900030907473,0.002982410981580468
-2.2463002732069746,0.57,3.0,53.0,-0.0013176307513165628,0.0012674164873275652,-0.0025447049795247136,0.0024578257343539256
-2.2463002732069746,0.63,3.0,49.0,-0.0012079611049899842,0.0010426106838313802,-0.0024080935047033816,0.002011803875778202
-2.2463002732069746,0.69,3.0,51.0,-0.0008496777855216861,0.0006336929750958614,-0.0017343564282336868,0.0011861088902886366
-2.2463002732069746,0.75,3.0,44.0,-0.0004088463837821723,0.0005408374216197423,-0.0007600269808589443,0.0010611027172568372
-2.2463002732069746,0.81,3.0,36.0,-0.0005786482131926029,0.0005723426910997307,-0.0011174786605657396,0.001144167347998378
-2.2463002732069746,0.87,3.0,39.0,-0.00041992529952416695,0.0004684183847517106,-0.0008190476790780975,0.0008984504573645621
-2.2463002732069746,0.93,3.0,49.0,-0.00030845308508387,0.00023640382082257456,-0.0006288702794772248,0.00044265892261992736
-2.2463002732069746,0.99,3.0,20.0,-7.474363789006015e-05,8.860443794327607e-05,-0.00014739393397812677,0.00017517463232539238
-2.85382193849786,0.27,3.0,7.0,-0.0015989271581174443,0.0016875547399980424,-0.0030732269225320435,0.0034063339815076804
-2.85382193849786,0.33,3.0,23.0,-0.001510778977785471,0.001727727344844553,-0.0029579710303968385,0.0036606321940869596
-2.85382193849786,0.39,3.0,32.0,-0.001598224734337009,0.001551570107265175,-0.0031680645269900358,0.0030763515328543294
-2.85382193849786,0.45,3.0,38.0,-0.0014880224310627006,0.001400737259388304,-0.002927721980614342,0.002804211771601173
-2.85382193849786,0.51,3.0,59.0,-0.0014901460944379283,0.0013600248193265147,-0.0029309040843996073,0.002777182655998793
-2.85382193849786,0.57,3.0,54.0,-0.0012791536622538012,0.001342340085865075,-0.0024382513909283737,0.0026454883532350906
-2.85382193849786,0.63,3.0,47.0,-0.0012892860687532556,0.0011563328760667297,-0.0024606710916435246,0.002300614439448741
-2.85382193849786,0.69,3.0,53.0,-0.00093876665216641,0.0007525581388279192,-0.0019206665678987045,0.0014742381886800253
-2.85382193849786,0.75,3.0,44.0,-0.0005485946215419495,0.0006627324762799235,-0.001025153920062798,0.0014235778306300674
-2.85382193849786,0.81,3.0,34.0,-0.0008098098322674847,0.0007736663696303982,-0.0016251819038949151,0.0014969300602331282
-2.85382193849786,0.87,3.0,37.0,-0.00055587168348551,0.000500818454117119,-0.001046801519230824,0.0010583790783845824
-2.85382193849786,0.93,3.0,51.0,-0.00047294929795796956,0.0004032358086948305,-0.0009701688507960664,0.0007719768592795517
-2.85382193849786,0.99,3.0,21.0,-0.0003200606926651359,0.00019571601268762834,-0.0006786024748351807,0.00036434585321249395
-3.625650476828164,0.27,3.0,6.0,-0.0016654361041176797,0.0019695905869566333,-0.0031889296538829184,0.0036575457875335222
-3.625650476828164,0.33,3.0,24.0,-0.0013627767793259493,0.001531551502829542,-0.0024310791033049822,0.0030635075058787612
-3.625650476828164,0.39,3.0,31.0,-0.0012581761567789134,0.0012644002309671663,-0.002477862383200549,0.0025008297288966665
-3.625650476828164,0.45,3.0,39.0,-0.0011209411037718723,0.0010927422507436208,-0.002207147818578203,0.002130312700644526
-3.625650476828164,0.51,3.0,62.0,-0.0011206845914608124,0.0011277401691342352,-0.0022512816395044454,0.0021297061225043386
-3.625650476828164,0.57,3.0,52.0,-0.0010182895243930489,0.0010271977559479716,-0.00196541550034009,0.001994068974603109
-3.625650476828164,0.63,3.0,47.0,-0.0010963485763903537,0.001072523032197868,-0.0021159733641019987,0.0021568508373726587
-3.625650476828164,0.69,3.0,50.0,-0.0008480676869658432,0.0008117853558784585,-0.0017431734203638123,0.001478215512185023
-3.625650476828164,0.75,3.0,46.0,-0.0006945167016076258,0.0008321330536584456,-0.0013454017154987928,0.0016305491157187115
-3.625650476828164,0.81,3.0,31.0,-0.0009326630675821662,0.0008792634663375995,-0.0018837882136966977,0.0016912337527772883
-3.625650476828164,0.87,3.0,37.0,-0.0005529031228220637,0.0005850042180879435,-0.0010777338523765246,0.001130358160767836
-3.625650476828164,0.93,3.0,52.0,-0.0007955080519950958,0.0006493498129887272,-0.0015551114476563192,0.0012829090432591424
-3.625650476828164,0.99,3.0,23.0,-0.0004900255646478465,0.0003656938478595362,-0.0010475258211040128,0.0006709024641687711
-4.6062233956485175,0.27,3.0,6.0,-0.001797487894938351,0.001819233888786686,-0.0032863060427299477,0.0037370188690537902
-4.6062233956485175,0.33,3.0,23.0,-0.0011427867569306866,0.0014064519036460614,-0.0023147232073752176,0.0027642869987573432
-4.6062233956485175,0.39,3.0,32.0,-0.0011315305461531535,0.0010433575609897368,-0.0022639666444241057,0.0019802436614802825
-4.6062233956485175,0.45,3.0,43.0,-0.0009921619321746657,0.0009375154019466354,-0.00200164137478031,0.0018075617317973086
-4.6062233956485175,0.51,3.0,62.0,-0.0008551214586954248,0.000804623548048825,-0.0016566144369026497,0.001647859034763202
-4.6062233956485175,0.57,3.0,56.0,-0.0007948104251844963,0.000804831811550265,-0.001534926986361568,0.0016351516189751496
-4.6062233956485175,0.63,3.0,51.0,-0.0008816684529957122,0.0009260935240246754,-0.0017198538953217713,0.0017723252595687792
-4.6062233956485175,0.69,3.0,41.0,-0.0008235847844387831,0.0007449661500822881,-0.0017048079899698659,0.0013959974450196307
-4.6062233956485175,0.75,3.0,46.0,-0.0006948053533341118,0.0007225170766964256,-0.0013456312424144194,0.0014097421719187484
-4.6062233956485175,0.81,3.0,28.0,-0.0009572051470888371,0.0009473602303419456,-0.0018040632028258913,0.0018867969362446374
-4.6062233956485175,0.87,3.0,32.0,-0.0007424156238057598,0.000670065257549726,-0.0014467786736957837,0.0013050720785659708
-4.6062233956485175,0.93,3.0,49.0,-0.0010380872998284917,0.0009926876528033998,-0.0021460191393192734,0.0017965807199048435
-4.6062233956485175,0.99,3.0,31.0,-0.000580065758590117,0.0004982170153340572,-0.0012037415536627408,0.000971369486723262
-5.851996519306451,0.27,3.0,8.0,-0.001890585977772835,0.0018720203825310644,-0.0037078434224896125,0.003502330620176516
-5.851996519306451,0.33,3.0,20.0,-0.0012385530263341802,0.0011781882308980291,-0.0024256680758411907,0.002245877073443049
-5.851996519306451,0.39,3.0,33.0,-0.0009074305971572027,0.000935531162877833,-0.0018323754660381439,0.0018307682388264185
-5.851996519306451,0.45,3.0,46.0,-0.0009622762384446935,0.0009413992983213165,-0.001864858930379179,0.0018618413022536504
-5.851996519306451,0.51,3.0,68.0,-0.0007258116186044263,0.0007359904439816902,-0.0014918851648378457,0.001360003816349999
-5.851996519306451,0.57,3.0,61.0,-0.0009369490220051782,0.0009251691364874058,-0.001877591170559594,0.001742526284037153
-5.851996519306451,0.63,3.0,51.0,-0.0009743589593209146,0.000938279809646542,-0.0019775852561048127,0.0018156338936165142
-5.851996519306451,0.69,3.0,41.0,-0.0010734957534150225,0.0009603393695896868,-0.002066102497382202,0.0018433513964992247
-5.851996519306451,0.75,3.0,32.0,-0.0007257161336363636,0.0008246596810500658,-0.0013697790443696232,0.0017599809441346285
-5.851996519306451,0.81,3.0,28.0,-0.0010450056698593994,0.0009928753686849,-0.0021045371416924074,0.001949496569003526
-5.851996519306451,0.87,3.0,26.0,-0.0014732445199470764,0.0014203651274499376,-0.0031245657533877577,0.0026953536015643874
-5.851996519306451,0.93,3.0,49.0,-0.0014076456611639163,0.001393790182692291,-0.0026769950221943546,0.0027991426668605404
-5.851996519306451,0.99,3.0,37.0,-0.0011234192225751192,0.0009701754944106428,-0.002292709620186139,0.001794699753451718
-7.434694395049644,0.27,3.0,6.0,-0.002544172878160648,0.0019612618047991823,-0.00490388362988579,0.003518297479085275
-7.434694395049644,0.33,3.0,18.0,-0.0010730973492673762,0.001165215447610442,-0.0021117372163095994,0.0022367633174984274
-7.434694395049644,0.39,3.0,38.0,-0.0010706890276235563,0.0011455189780687754,-0.001995662462852662,0.002465197821472832
-7.434694395049644,0.45,3.0,46.0,-0.00107069217670907,0.0010562759334995057,-0.0021439395636509893,0.0020738858593602268
-7.434694395049644,0.51,3.0,70.0,-0.0009882173828110563,0.0010425390505962014,-0.001967558188766559,0.0020279520563564564
-7.434694395049644,0.57,3.0,67.0,-0.0011896595718806585,0.001210838104994619,-0.00233737496110082,0.0023139188816508833
-7.434694395049644,0.63,3.0,52.0,-0.001259667251444379,0.0013160592345987667,-0.00248592439875032,0.002656295672344452
-7.434694395049644,0.69,3.0,37.0,-0.0014601426986443067,0.0013151997019546678,-0.0029792707842190174,0.002563948728632078
-7.434694395049644,0.75,3.0,29.0,-0.0011456630799186371,0.0012501432504501157,-0.002187732841084884,0.002546139475231227
-7.434694395049644,0.81,3.0,25.0,-0.0016882644493989897,0.0015108615779198624,-0.0034331717405870015,0.0028117628208566506
-7.434694395049644,0.87,3.0,21.0,-0.003124237065256585,0.002735918422987215,-0.0060799591179855365,0.005366345979183675
-7.434694395049644,0.93,3.0,43.0,-0.0017794846840505764,0.0019047505250910871,-0.0036567211495158,0.0036316090063758777
-7.434694395049644,0.99,3.0,48.0,-0.001899254529204365,0.001639170013155056,-0.003963684474173001,0.0030569730636133582
-9.445439785451782,0.33,3.0,21.0,-0.0018090912627087587,0.0012959013796055485,-0.0035849781573534475,0.0025357101452535215
-9.445439785451782,0.39,3.0,35.0,-0.0014372432710548363,0.0013589782162190542,-0.002846287723272829,0.002695801650288474
-9.445439785451782,0.45,3.0,46.0,-0.0014151223851600588,0.001418101587173867,-0.00272676775672739,0.002815806333189192
-9.445439785451782,0.51,3.0,71.0,-0.001239408860367149,0.0013914303640032682,-0.0025486735813429065,0.00278753592445048
-9.445439785451782,0.57,3.0,63.0,-0.0014120472414705743,0.0014562094005030172,-0.002892925356101395,0.0028137597227118746
-9.445439785451782,0.63,3.0,57.0,-0.001409188705783216,0.0012710075656828554,-0.0027842766853552595,0.002510763992021366
-9.445439785451782,0.69,3.0,39.0,-0.0018549069713779762,0.0018374644106219674,-0.003743366962025413,0.0033943421377175998
-9.445439785451782,0.75,3.0,30.0,-0.0018649214785201307,0.0018038999352090429,-0.0037134922569790714,0.0033662431902549577
-9.445439785451782,0.81,3.0,24.0,-0.002039978844822398,0.002038087194288675,-0.004120180123259739,0.003996321035754961
-9.445439785451782,0.87,3.0,21.0,-0.004974908354177934,0.004674691493924437,-0.009887853105033624,0.009014070170227652
-9.445439785451782,0.93,3.0,42.0,-0.0020172020843393754,0.0021843359478495093,-0.004078895987122324,0.004300716783901933
-9.445439785451782,0.99,3.0,48.0,-0.0022277097406776408,0.0019258878366253793,-0.004462630536560452,0.003662767852518676
-12.000000000000009,0.33,3.0,16.0,-0.002665294622687816,0.0024260778558696703,-0.00520188957601236,0.004895106890311098
-12.000000000000009,0.39,3.0,23.0,-0.0020312544913032556,0.002012204561297401,-0.004200649504931833,0.0038544196593765477
-12.000000000000009,0.45,3.0,54.0,-0.0016294405385395608,0.0016392125323670642,-0.003398986769268716,0.003143854332963981
-12.000000000000009,0.51,3.0,56.0,-0.0020033481112806516,0.0018263721297455235,-0.0037708341608632687,0.003688680708514314
-12.000000000000009,0.57,3.0,74.0,-0.0018152476809942767,0.0017193645325608545,-0.003442807770346173,0.003457455784430209
-12.000000000000009,0.63,3.0,63.0,-0.0018508655591629578,0.0017061066552003336,-0.003759076609327891,0.003439681654959948
-12.000000000000009,0.69,3.0,43.0,-0.002722251857902405,0.002419700370096211,-0.005538432105478527,0.004694467108233398
-12.000000000000009,0.75,3.0,30.0,-0.0025844646814705483,0.0027800058103924496,-0.005186675193986655,0.005265871184366029
-12.000000000000009,0.81,3.0,22.0,-0.0019667057787660287,0.0019199728925562082,-0.0038918492791750574,0.0035724425372344808
-12.000000000000009,0.87,3.0,23.0,-0.009667480961342276,0.007751471346841048,-0.018513300699711265,0.014785946210096452
-12.000000000000009,0.93,3.0,30.0,-0.004293022162406742,0.005559767939487159,-0.007877319424133191,0.012023349807931624
-12.000000000000009,0.99,3.0,51.0,-0.0028309728949553305,0.0028464582213477236,-0.005862972353711711,0.005610471433194207
-12.000000000000009,1.05,3.0,13.0,-0.003162447947962174,0.0021809719573087647,-0.006834567903476945,0.0038800877650104343
+0.1000000000000034,0.39,0.0,6.0,-0.0003261233489665525,0.0003972693686810264,-0.0006055081499745283,0.0007832111859300733
+0.1000000000000034,0.45,0.0,21.0,-0.00019549463322920802,0.00020503471249289817,-0.00038809059942242734,0.0004035482560803279
+0.1000000000000034,0.51,0.0,21.0,-0.00017746492805196005,0.00026845021012719293,-0.00033880449192052884,0.0006028009017975041
+0.1000000000000034,0.57,0.0,41.0,-0.00010523082950888781,0.00013271063154053799,-0.0001987967116583062,0.0002822844992665728
+0.1000000000000034,0.63,0.0,59.0,-9.948605779795807e-05,0.00012376298179177166,-0.00018489278376608177,0.0002652922544955034
+0.1000000000000034,0.69,0.0,49.0,-7.41044884850666e-05,0.00010300430171985454,-0.00013434253146771404,0.0002263086432576197
+0.1000000000000034,0.75,0.0,69.0,-9.328513794830062e-05,9.091601793049584e-05,-0.00019576933574832456,0.00017957573800230555
+0.1000000000000034,0.81,0.0,155.0,-7.05341944747958e-05,6.954889735847368e-05,-0.0001295009729652189,0.00014701021306347945
+0.1000000000000034,0.87,0.0,76.0,-0.0001287796273284682,0.00011812416292268937,-0.00025083310958042113,0.00022596875197109238
+0.1270454343320557,0.39,0.0,6.0,-0.0005174327393802266,0.0006380886649899516,-0.0009596976677880842,0.0012237379889364537
+0.1270454343320557,0.45,0.0,21.0,-0.0003303149522153283,0.0003359592582237495,-0.0006286743887265286,0.0006525898458345399
+0.1270454343320557,0.51,0.0,23.0,-0.00023713502560984728,0.0003198030068890879,-0.0004570578702065719,0.000660069497757808
+0.1270454343320557,0.57,0.0,42.0,-0.00013389812741454427,0.00016286912470523345,-0.00026174699754117535,0.000322808818866543
+0.1270454343320557,0.63,0.0,56.0,-0.00012814353735653015,0.00015563266361421835,-0.0002440227821656597,0.0003115653403492406
+0.1270454343320557,0.69,0.0,52.0,-7.997309734325427e-05,0.00010798185503419473,-0.00014884415179208753,0.00023211945172321095
+0.1270454343320557,0.75,0.0,66.0,-7.560297889255447e-05,8.890255380418164e-05,-0.0001389295814675018,0.0001848711176665386
+0.1270454343320557,0.81,0.0,155.0,-7.501287724272192e-05,7.73933988753703e-05,-0.00014629931863689865,0.00015022412247045431
+0.1270454343320557,0.87,0.0,76.0,-0.0001329433943516084,0.000123284015939268,-0.00026704604030275213,0.00023546070500129475
+0.1614054238462012,0.39,0.0,7.0,-0.0008558119739170265,0.000867215151845719,-0.0015791656556129862,0.001724084530740264
+0.1614054238462012,0.45,0.0,19.0,-0.0005166847008112822,0.0005440362492574172,-0.00105397593092272,0.0010154635685741598
+0.1614054238462012,0.51,0.0,27.0,-0.00036616590103988534,0.0004024749621665649,-0.0006873612593628725,0.0008036905317704223
+0.1614054238462012,0.57,0.0,43.0,-0.00019767323174559823,0.0002080621112564705,-0.00036821607440688743,0.00041846092133874445
+0.1614054238462012,0.63,0.0,54.0,-0.00017995916180126365,0.00020396903855566848,-0.000345317748727022,0.0004052351950362934
+0.1614054238462012,0.69,0.0,53.0,-0.00010278869511901774,0.00012840614624117853,-0.00018772106035137853,0.00026764518796915804
+0.1614054238462012,0.75,0.0,67.0,-8.832090962701292e-05,9.739851141193597e-05,-0.00016082626997202163,0.00020444062235493813
+0.1614054238462012,0.81,0.0,154.0,-9.100732942684867e-05,8.637673838777447e-05,-0.0001912437277164383,0.00017166331718416442
+0.1614054238462012,0.87,0.0,73.0,-0.0001450264410800097,0.00013868470693237985,-0.00027165619240626833,0.00026600859000803725
+0.2050582217609059,0.39,0.0,7.0,-0.0015246432767369587,0.001524643276736959,-0.0028456963988880185,0.0028481903847362394
+0.2050582217609059,0.45,0.0,21.0,-0.0008280633472708495,0.000763698207903056,-0.0016057521781454667,0.0015673062500256253
+0.2050582217609059,0.51,0.0,28.0,-0.0005359744202408856,0.0006004040166906315,-0.0010592815262765137,0.0011669444854759425
+0.2050582217609059,0.57,0.0,44.0,-0.0003060120943996633,0.0003215579436147135,-0.0006042189319261705,0.0006002939480907633
+0.2050582217609059,0.63,0.0,54.0,-0.00024813794217672146,0.00029092093126761,-0.000491219603672038,0.0005699716423921107
+0.2050582217609059,0.69,0.0,54.0,-0.0001380126828517936,0.00016126365165300644,-0.000264450499701672,0.00032923564016239135
+0.2050582217609059,0.75,0.0,63.0,-0.00012075770305521967,0.00013095403478911586,-0.00022596722666086194,0.00025946860482491764
+0.2050582217609059,0.81,0.0,156.0,-0.00015163125504686291,0.0001229544727709464,-0.00031750017599569547,0.00023378526667092221
+0.2050582217609059,0.87,0.0,69.0,-0.0001742741642704788,0.0001662752432576156,-0.00035225948141771375,0.0003113633440481267
+0.2605171084697372,0.39,0.0,9.0,-0.0021651511283631935,0.0021490576989620595,-0.004158419483212297,0.0042106282913998245
+0.2605171084697372,0.45,0.0,19.0,-0.0012622019703381249,0.0012347711759910975,-0.0025087315366126364,0.0023036034652299704
+0.2605171084697372,0.51,0.0,30.0,-0.0007942058555313825,0.0007759778391364442,-0.0015366362456336194,0.0015854090738157895
+0.2605171084697372,0.57,0.0,47.0,-0.0004160091451914268,0.00040103959507175615,-0.0008376062672521569,0.0007604302500369512
+0.2605171084697372,0.63,0.0,51.0,-0.0003665505974798807,0.0003731884595718159,-0.0007153161236337822,0.000727204393915921
+0.2605171084697372,0.69,0.0,53.0,-0.00017736889615340388,0.00019611670696389262,-0.0003360047066466862,0.0004093095206843209
+0.2605171084697372,0.75,0.0,64.0,-0.00015299400789156278,0.0001513839183320035,-0.0002956299966947957,0.0003042876472780875
+0.2605171084697372,0.81,0.0,155.0,-0.00021932267489818214,0.00015515241840497978,-0.00044665816089277025,0.0002973691815622279
+0.2605171084697372,0.87,0.0,68.0,-0.00020472062454246568,0.0001976380358517537,-0.0004027406198344559,0.0003837198785182893
+0.3309750919646881,0.39,0.0,11.0,-0.0026637164767773043,0.0030081801571791023,-0.005363138754991974,0.005731600355559804
+0.3309750919646881,0.45,0.0,19.0,-0.0018422842800601713,0.0017124128839796058,-0.003676072751827182,0.0032696476650531537
+0.3309750919646881,0.51,0.0,31.0,-0.0010685666819408505,0.0010638895970186727,-0.002040668832316195,0.002097562958996621
+0.3309750919646881,0.57,0.0,47.0,-0.0006295854576897238,0.0005888842280540563,-0.0012620966223586068,0.0011167006982581132
+0.3309750919646881,0.63,0.0,51.0,-0.00044291517239465497,0.00045286582006572404,-0.0008853226159471093,0.0009008740390379728
+0.3309750919646881,0.69,0.0,51.0,-0.00024355236524571224,0.00023940815368421136,-0.0004489735195020385,0.0004997316433203623
+0.3309750919646881,0.75,0.0,70.0,-0.00019074537258024124,0.0001718431488310298,-0.000367995108945423,0.00034755953218291026
+0.3309750919646881,0.81,0.0,153.0,-0.00023543741849422844,0.00019100857883617257,-0.0004940969265854111,0.0003629654556191791
+0.3309750919646881,0.87,0.0,63.0,-0.0002582201977050475,0.00024099547066830227,-0.0005296716380965756,0.00045783799962342175
+0.4204887431174597,0.39,0.0,10.0,-0.0032615034082941045,0.0037047145073520827,-0.0060408021682325135,0.007522196454131949
+0.4204887431174597,0.45,0.0,20.0,-0.002361146430355885,0.0021603920580159815,-0.00470931591340576,0.0042391121296896
+0.4204887431174597,0.51,0.0,32.0,-0.0013768477747315379,0.00138574604134898,-0.00276159684752735,0.002631924774495667
+0.4204887431174597,0.57,0.0,48.0,-0.0008803901863727874,0.0008663599384214734,-0.001765132609293169,0.0016911317487091823
+0.4204887431174597,0.63,0.0,48.0,-0.00048167304108097695,0.0005614054188779674,-0.0009456559999032307,0.0011085533285209806
+0.4204887431174597,0.69,0.0,50.0,-0.000314951940447625,0.0003317760700380367,-0.0006331152881468114,0.0006387707027135515
+0.4204887431174597,0.75,0.0,86.0,-0.000224115537656723,0.0002095843570187772,-0.00045032236914125653,0.000423515743014392
+0.4204887431174597,0.81,0.0,147.0,-0.0002696223965772755,0.0002337794596733294,-0.0005734463179128187,0.00043896425007657416
+0.4204887431174597,0.87,0.0,55.0,-0.0003269109021898337,0.00027148199176175894,-0.000638713271945229,0.000546920743888224
+0.5342117500109793,0.39,0.0,9.0,-0.003470636059300131,0.0037003383449411434,-0.00674700700623405,0.007809397525819872
+0.5342117500109793,0.45,0.0,22.0,-0.0023886330900317805,0.0025169752842038352,-0.005179430304078284,0.004731652084066421
+0.5342117500109793,0.51,0.0,32.0,-0.0016270875652492191,0.0017433754625009587,-0.0033209618680985807,0.0033661426828988867
+0.5342117500109793,0.57,0.0,47.0,-0.001135003308160422,0.0011020840441879798,-0.00219886048309522,0.0021885744368995877
+0.5342117500109793,0.63,0.0,52.0,-0.0006090501890917197,0.0006908663749424095,-0.0012188219966895945,0.0013569681950604316
+0.5342117500109793,0.69,0.0,47.0,-0.00042346334396660927,0.00038900559162864765,-0.0008049313319982844,0.000795715078481942
+0.5342117500109793,0.75,0.0,111.0,-0.000411777397878959,0.00031038029673058327,-0.0008599891526081324,0.0005700267923703167
+0.5342117500109793,0.81,0.0,134.0,-0.00023849123477664338,0.00024073918288704404,-0.00044703857160564,0.0004721839625063397
+0.5342117500109793,0.87,0.0,41.0,-0.000243519590608945,0.0001673065249152811,-0.0005174292273112522,0.00031431951239450483
+0.6786916380543193,0.39,0.0,7.0,-0.003689093409531323,0.0033815182870439472,-0.007378249391616196,0.006391573225345019
+0.6786916380543193,0.45,0.0,29.0,-0.002438162870634293,0.00244866989057845,-0.004959037407183547,0.004580014222459751
+0.6786916380543193,0.51,0.0,33.0,-0.0019442179209666543,0.0019117728859106892,-0.0036972978869957516,0.0036992000191057206
+0.6786916380543193,0.57,0.0,48.0,-0.0012402819754908875,0.0011643728939014436,-0.0023437541858012147,0.002395779555489312
+0.6786916380543193,0.63,0.0,48.0,-0.0007376439795439048,0.0007471996264539738,-0.0014222327125572906,0.001512015293077002
+0.6786916380543193,0.69,0.0,52.0,-0.0004650878217946753,0.0004634778507365226,-0.0009318067270877973,0.0008957187470134268
+0.6786916380543193,0.75,0.0,125.0,-0.0004290043072832141,0.0003575458953205497,-0.0009637460844249244,0.0006568426947634018
+0.6786916380543193,0.81,0.0,116.0,-0.0002898515097885965,0.00031563345244901055,-0.000581484056440696,0.0006001984767776621
+0.6786916380543193,0.87,0.0,36.0,-0.0001523766959745399,0.00014110142390650593,-0.0003083757079884136,0.00027068579294722096
+0.8622467393414552,0.33,0.0,6.0,-0.003561485473116318,0.003934832345133847,-0.006568436812390481,0.007769821433670461
+0.8622467393414552,0.39,0.0,12.0,-0.0026285335745518633,0.0034347728733188907,-0.00485646352641177,0.007605221576466577
+0.8622467393414552,0.45,0.0,29.0,-0.002519923752796777,0.0023924169486029653,-0.004905818407750871,0.00467916315969358
+0.8622467393414552,0.51,0.0,28.0,-0.0024217622716895134,0.002203729274408326,-0.004970928558390374,0.004140325273283359
+0.8622467393414552,0.57,0.0,51.0,-0.0014281490109053416,0.0012059777138625737,-0.002912838829568672,0.0023740056272526333
+0.8622467393414552,0.63,0.0,50.0,-0.000988814522351882,0.0009258632159873281,-0.0018944695833079115,0.001855406900003563
+0.8622467393414552,0.69,0.0,54.0,-0.0005814471569480671,0.0005672614207295065,-0.0011632271667732178,0.0010902993309484452
+0.8622467393414552,0.75,0.0,133.0,-0.0004772402737974723,0.00039811912797295526,-0.0010053299346799106,0.000759368438918397
+0.8622467393414552,0.81,0.0,102.0,-0.0004203825118623777,0.0004374916737576456,-0.000839778023895685,0.0008338864601402863
+0.8622467393414552,0.87,0.0,32.0,-0.0002170157064449374,0.00019699637922599098,-0.0004157000865758714,0.0003976124028534633
+1.0954451150103253,0.33,0.0,6.0,-0.00433291522357217,0.004011880399473756,-0.008855438399191855,0.007253078249113366
+1.0954451150103253,0.39,0.0,14.0,-0.0025839125891290245,0.002878987800621274,-0.005083773084955349,0.00589284523165694
+1.0954451150103253,0.45,0.0,31.0,-0.0022830223511405836,0.0023194541883517026,-0.004706413791744361,0.004488699130249411
+1.0954451150103253,0.51,0.0,35.0,-0.0023053028551245857,0.0021188906001371874,-0.004863433659476231,0.004095448127348695
+1.0954451150103253,0.57,0.0,47.0,-0.0016271760245363865,0.0014716341239003185,-0.003458287109315473,0.002767414900545486
+1.0954451150103253,0.63,0.0,51.0,-0.0011208159095425028,0.0010601979168653765,-0.002255638465763552,0.002059053210624247
+1.0954451150103253,0.69,0.0,58.0,-0.0006880338542845124,0.0006732789783002951,-0.0014019023724421654,0.0013653577741387641
+1.0954451150103253,0.75,0.0,135.0,-0.0005144301870016399,0.00045353864339773485,-0.0010248016944212155,0.0008882891443336919
+1.0954451150103253,0.81,0.0,89.0,-0.000571155197068823,0.0005799257519585959,-0.0011271448171432453,0.00116066113568009
+1.0954451150103253,0.87,0.0,30.0,-0.0002723085019145976,0.00023152375312569158,-0.0005122006354776205,0.0004531845067809713
+1.3917130042341683,0.33,0.0,12.0,-0.002128320049024042,0.0017511728346944863,-0.004579045977858397,0.003123158990172843
+1.3917130042341683,0.39,0.0,19.0,-0.0014149878834051053,0.0015645742266355593,-0.0027125049550548183,0.0032253723649901906
+1.3917130042341683,0.45,0.0,33.0,-0.0017727258219999212,0.0016500408246965434,-0.0036262552245804386,0.0032503416584117963
+1.3917130042341683,0.51,0.0,39.0,-0.001419447617857197,0.0014310524437584021,-0.002926471013531701,0.0026922538512966455
+1.3917130042341683,0.57,0.0,48.0,-0.0011247216760781789,0.0011761617860043853,-0.002124569940204523,0.0023235387314009645
+1.3917130042341683,0.63,0.0,40.0,-0.0010002085613673784,0.0009523594640561396,-0.001984666226143805,0.0019381627198377114
+1.3917130042341683,0.69,0.0,61.0,-0.0007557551493840524,0.0007122218044505053,-0.001410642395395119,0.001477888639729775
+1.3917130042341683,0.75,0.0,123.0,-0.0006000647291698304,0.0005330248879409158,-0.0012133013957200546,0.0010001414852195232
+1.3917130042341683,0.81,0.0,95.0,-0.0005435186364734132,0.0005692355270864879,-0.0010896506575858906,0.0011094785281101985
+1.3917130042341683,0.87,0.0,24.0,-0.0003390426650349552,0.0003326850771064713,-0.0007040603213883889,0.0006165189966121775
+1.7681078308849945,0.27,0.0,10.0,-0.0017070533339990559,0.0018268519710720496,-0.0035846674990783222,0.0033222631654837493
+1.7681078308849945,0.33,0.0,13.0,-0.0023364099012565124,0.002312115006899213,-0.004695053342623518,0.004482692865929102
+1.7681078308849945,0.39,0.0,24.0,-0.0013734031543833824,0.00135046598948881,-0.0027120255518785817,0.002801139020625814
+1.7681078308849945,0.45,0.0,38.0,-0.0017310842860844323,0.0014293370157910574,-0.003489118387580473,0.0027546998062836473
+1.7681078308849945,0.51,0.0,40.0,-0.0013041561168319464,0.0014347811727933495,-0.0025798123560076764,0.0028768955461507977
+1.7681078308849945,0.57,0.0,48.0,-0.0010556530200625431,0.0010419361261474922,-0.002031176108314189,0.0020966149042332912
+1.7681078308849945,0.63,0.0,31.0,-0.0011103640078625639,0.00094686952262137,-0.0022376384992142504,0.001890184037302756
+1.7681078308849945,0.69,0.0,60.0,-0.0009579660573238881,0.0009886633121195894,-0.0018607157687683122,0.0018887595305890658
+1.7681078308849945,0.75,0.0,115.0,-0.0007019775387942338,0.0006522803044086734,-0.001377703056065987,0.0013104225366404863
+1.7681078308849945,0.81,0.0,99.0,-0.000626500320290734,0.0006003191287515331,-0.001206374294620563,0.001163650965246137
+1.7681078308849945,0.87,0.0,20.0,-0.0009394124265297825,0.0006213557948268487,-0.0019591510631559784,0.001148272233569227
+2.2463002732069133,0.27,0.0,9.0,-0.0017012024608551535,0.0017567361535177303,-0.0034899925834247507,0.00321420626702977
+2.2463002732069133,0.33,0.0,14.0,-0.0015141896391149387,0.0017069545901323923,-0.003033652400466101,0.0032998812999787946
+2.2463002732069133,0.39,0.0,22.0,-0.0017535162945847176,0.0017809591414559192,-0.0034069808173393737,0.003647031341807926
+2.2463002732069133,0.45,0.0,36.0,-0.0014639628949582898,0.0015654684421454348,-0.0027062210361815248,0.003118275947217051
+2.2463002732069133,0.51,0.0,44.0,-0.001491389061855014,0.00164448607390918,-0.0030000103457877604,0.0030654340755555784
+2.2463002732069133,0.57,0.0,49.0,-0.0013914030980326838,0.0013550958154826367,-0.002733545568497115,0.0025920758575946595
+2.2463002732069133,0.63,0.0,39.0,-0.0015121797627315142,0.001462218016109833,-0.003027748071765912,0.002793602277259488
+2.2463002732069133,0.69,0.0,63.0,-0.0009842982027665182,0.00103537720431286,-0.001978877983888475,0.0019579982092222557
+2.2463002732069133,0.75,0.0,130.0,-0.0007400767421180476,0.0006967845322556602,-0.0014516284652979225,0.0013901385555365347
+2.2463002732069133,0.81,0.0,76.0,-0.0007046996809735227,0.0007128521226373181,-0.0014456984631657434,0.0013630219712529054
+2.2463002732069133,0.87,0.0,15.0,-0.0008641119882497875,0.0008956538034758961,-0.0017154743336756921,0.0017444158007740873
+2.853821938497888,0.27,0.0,11.0,-0.001780542608874532,0.001985947691886755,-0.0033136296195257244,0.0041320934133346155
+2.853821938497888,0.33,0.0,14.0,-0.0019346397635391572,0.0017103293189431568,-0.003900744355615281,0.003205497554574271
+2.853821938497888,0.39,0.0,26.0,-0.002116672149756594,0.0024140479725756245,-0.004235292624527361,0.004749167788317331
+2.853821938497888,0.45,0.0,32.0,-0.002317155803603742,0.002750667473347956,-0.004647421494834045,0.005277218396293819
+2.853821938497888,0.51,0.0,44.0,-0.002016061908333637,0.001969505061079079,-0.0039209883373925855,0.003738120480139558
+2.853821938497888,0.57,0.0,49.0,-0.0025941595404706925,0.0024034436580753324,-0.004844667216114583,0.004941533228190611
+2.853821938497888,0.63,0.0,61.0,-0.0017147309237864727,0.001620573265851751,-0.00333006915128173,0.003272648592725186
+2.853821938497888,0.69,0.0,82.0,-0.0013461834528401444,0.0012391144333570448,-0.0025927348571213576,0.0024823518449511254
+2.853821938497888,0.75,0.0,109.0,-0.00092679366736589,0.0008987118859571177,-0.001829282498782718,0.0018289475370025694
+2.853821938497888,0.81,0.0,60.0,-0.000817595926508236,0.0008186108081466036,-0.0016483308178011796,0.001627725771551297
+2.853821938497888,0.87,0.0,9.0,-0.0012325340592426813,0.0013270542413532733,-0.0022956341746967193,0.002568382190151522
+3.625650476828125,0.21,0.0,8.0,-0.002938312238651347,0.002958419758791353,-0.005218696526722119,0.006204123371059804
+3.625650476828125,0.27,0.0,13.0,-0.0017700906812476223,0.0018387277698831365,-0.003305132899485811,0.0035861981815915023
+3.625650476828125,0.33,0.0,31.0,-0.0018255680165351045,0.0018449357791459537,-0.0035608660822433005,0.0037335922328654188
+3.625650476828125,0.39,0.0,41.0,-0.0016273554671760036,0.001762332940866098,-0.003116781092263582,0.003428127116179437
+3.625650476828125,0.45,0.0,54.0,-0.0016054744445256031,0.0016003752282350192,-0.0031360817882528443,0.0032575591584960216
+3.625650476828125,0.51,0.0,44.0,-0.001908959618810463,0.001790389207142502,-0.003657318234208641,0.0033745714962529305
+3.625650476828125,0.57,0.0,48.0,-0.001999021512398784,0.0018720628731732627,-0.004013062475751015,0.003800425823511968
+3.625650476828125,0.63,0.0,38.0,-0.0023479902868056087,0.0021602903926335316,-0.004503658258969174,0.0042842773630217814
+3.625650476828125,0.69,0.0,82.0,-0.0014401867144198364,0.0013835097710455922,-0.002862973139883558,0.00266044903760775
+3.625650476828125,0.75,0.0,99.0,-0.001057569371000772,0.0010407104835672733,-0.0021396781353201205,0.002028940163721969
+3.625650476828125,0.81,0.0,39.0,-0.0011053641334214295,0.0011018911253272833,-0.0020007287778926043,0.002146800778680728
+4.606223395648528,0.21,0.0,14.0,-0.002737626431634571,0.002344952833203086,-0.005267301781433235,0.004502681504139384
+4.606223395648528,0.27,0.0,27.0,-0.001661712345269128,0.001935070952873744,-0.0031703011220783252,0.0038006259944560667
+4.606223395648528,0.33,0.0,38.0,-0.0019080406603984438,0.001961431527269696,-0.0038203295739514674,0.0039632258507432796
+4.606223395648528,0.39,0.0,44.0,-0.0018156183124129676,0.0017443428709381808,-0.003708982468157725,0.0034430229394903093
+4.606223395648528,0.45,0.0,45.0,-0.0020676337531854755,0.0019934180883345387,-0.003936510674060357,0.003964113418874279
+4.606223395648528,0.51,0.0,41.0,-0.0024616362974874263,0.002505457786515926,-0.00526343468457748,0.004684171870303097
+4.606223395648528,0.57,0.0,47.0,-0.0025850431237908296,0.002439938783192195,-0.005435562305794215,0.004714261081015166
+4.606223395648528,0.63,0.0,49.0,-0.00299019805755401,0.00269256909268637,-0.006052516064846127,0.0051668804135468665
+4.606223395648528,0.69,0.0,95.0,-0.0015751367840015176,0.001526655873313422,-0.003183129666503346,0.0029123216799937265
+4.606223395648528,0.75,0.0,81.0,-0.0017704217318999997,0.0016576973594643928,-0.003569191000925626,0.0033252085234608125
+4.606223395648528,0.81,0.0,17.0,-0.0026899030112899564,0.002887800732305369,-0.005497956509446289,0.005358752586303904
+5.851996519306431,0.15,0.0,7.0,-0.0039355650657331475,0.0035646945080767584,-0.007540622039649733,0.00670510357908979
+5.851996519306431,0.21,0.0,19.0,-0.0033566327996226164,0.0027134475817222037,-0.006582665133150123,0.005180527135797528
+5.851996519306431,0.27,0.0,26.0,-0.0026142524472845398,0.002638637947181915,-0.005487238298931111,0.00504145237677152
+5.851996519306431,0.33,0.0,49.0,-0.0021697369137156875,0.002066829244952267,-0.004595195434304126,0.0038700638836804786
+5.851996519306431,0.39,0.0,51.0,-0.002330119502490716,0.002356769163366887,-0.004544824992819499,0.004762839883112423
+5.851996519306431,0.45,0.0,52.0,-0.0025789368661865075,0.0020720474609354235,-0.0052602816626968075,0.004009765637617931
+5.851996519306431,0.51,0.0,49.0,-0.0038300339102505083,0.0034594730669966793,-0.008191105685144156,0.006628466165230158
+5.851996519306431,0.57,0.0,37.0,-0.004301001370981417,0.003511636687526989,-0.008062556765619256,0.007095970073704964
+5.851996519306431,0.63,0.0,51.0,-0.0033268813648422513,0.002916247123404769,-0.0073188381299535135,0.005157410768997346
+5.851996519306431,0.69,0.0,107.0,-0.0018222908621038977,0.001808679117115467,-0.003819827317880423,0.0033166409287531504
+5.851996519306431,0.75,0.0,48.0,-0.0025381762624703545,0.0027587289997666404,-0.004866281921126286,0.0055218258187840355
+7.434694395049639,0.15,0.0,12.0,-0.0035714592362078934,0.004051538901952509,-0.006774696896272084,0.008099950309930127
+7.434694395049639,0.21,0.0,30.0,-0.002099653901683948,0.0023237096301809636,-0.004077447214713673,0.00469632334220028
+7.434694395049639,0.27,0.0,45.0,-0.002160110623874941,0.0021003585546503587,-0.00396725024023674,0.004204272720085585
+7.434694395049639,0.33,0.0,51.0,-0.002013932349695562,0.001748536916257009,-0.003979059939547077,0.003453696238592232
+7.434694395049639,0.39,0.0,61.0,-0.002630890196263402,0.0024715283357254095,-0.0053779243772889476,0.004603109252298137
+7.434694395049639,0.45,0.0,52.0,-0.004249435073568085,0.003809657671793919,-0.008236628069192566,0.007477535360013377
+7.434694395049639,0.51,0.0,44.0,-0.003348395600391008,0.002794480901221874,-0.006957220163165785,0.005163678047497676
+7.434694395049639,0.57,0.0,50.0,-0.0035448267449245986,0.0029526257709416854,-0.007663286635374249,0.005370492018248513
+7.434694395049639,0.63,0.0,79.0,-0.002960444350780078,0.002596864893842597,-0.005793608807164161,0.005126873914549406
+7.434694395049639,0.69,0.0,64.0,-0.0033354611580382596,0.003194727602005651,-0.00650251330486503,0.006220694840442604
+7.434694395049639,0.75,0.0,11.0,-0.004382147175040789,0.0047506115126297955,-0.008172529795080473,0.009255331060248333
+9.445439785451784,0.15,0.0,14.0,-0.004207497223322459,0.004006020213069843,-0.008449865442261489,0.0076625360333315755
+9.445439785451784,0.21,0.0,37.0,-0.0028144849746222977,0.002892140092931315,-0.005211842989998253,0.005841293150079272
+9.445439785451784,0.27,0.0,57.0,-0.0021984919252437713,0.0023454496688190356,-0.004500799533522468,0.004519701042384075
+9.445439785451784,0.33,0.0,78.0,-0.0025310992070448853,0.002665348400741969,-0.0052922212534936295,0.005113977268782903
+9.445439785451784,0.39,0.0,59.0,-0.0035707015249611157,0.003437798634998425,-0.007349360984588353,0.006645121139364217
+9.445439785451784,0.45,0.0,56.0,-0.0036087176071261215,0.003132203252275892,-0.007051401148601893,0.006066532062409136
+9.445439785451784,0.51,0.0,42.0,-0.0037322167010186776,0.0034464765925227682,-0.007195051322478677,0.007043918737306889
+9.445439785451784,0.57,0.0,58.0,-0.0038426689374884645,0.00332664050140772,-0.007875835747127477,0.006431061387656367
+9.445439785451784,0.63,0.0,61.0,-0.004247373285990165,0.004163995624118521,-0.008380212064000104,0.007845200368900768
+9.445439785451784,0.69,0.0,33.0,-0.004332250247924122,0.005328695528485453,-0.008641193330647678,0.01028645785602433
+12.000000000000014,0.15,0.0,19.0,-0.003725713342582328,0.0035231136499634546,-0.007223230262423624,0.006799462242375349
+12.000000000000014,0.21,0.0,39.0,-0.003344182343727684,0.003356400323389763,-0.006425926863931098,0.006651724964752581
+12.000000000000014,0.27,0.0,66.0,-0.003012591108111482,0.0032271728367210114,-0.0058702127470603715,0.0062598605645448275
+12.000000000000014,0.33,0.0,85.0,-0.002757087333265132,0.0027904174685755142,-0.005369635019707297,0.005500511314293261
+12.000000000000014,0.39,0.0,62.0,-0.0029542844730249475,0.0029047248740197325,-0.006097830715446797,0.0056654777797182036
+12.000000000000014,0.45,0.0,65.0,-0.002615916362773637,0.0024521997075506387,-0.005143310247211186,0.004887297299978351
+12.000000000000014,0.51,0.0,54.0,-0.0044452096988927305,0.0040931143011112055,-0.00876371363056944,0.008108467245538225
+12.000000000000014,0.57,0.0,50.0,-0.005541036948884518,0.005333793168719828,-0.011546486568441138,0.010293989877889355
+12.000000000000014,0.63,0.0,40.0,-0.006528583988472255,0.006302170736090908,-0.013001169961512503,0.011890856850111434
+12.000000000000014,0.69,0.0,14.0,-0.008179276281473975,0.007647256788894125,-0.01603623566171478,0.015561890620875372
+0.0999999999999965,0.33,0.125,9.0,-0.0002966536667145693,0.00027615857955249896,-0.000561185264786854,0.00053489209657878
+0.0999999999999965,0.39,0.125,13.0,-0.00010500510595836983,0.00010829229169935121,-0.00019334728431546098,0.00021340897729058543
+0.0999999999999965,0.45,0.125,20.0,-0.00013721265330246006,0.0002158597710186601,-0.0002379520545754335,0.00047070737123270436
+0.0999999999999965,0.51,0.125,32.0,-0.00012912039126603656,0.00016917435252732685,-0.00023889207664338187,0.00037064767162106675
+0.0999999999999965,0.57,0.125,45.0,-0.0001042067092484098,0.00013629374210847925,-0.00018888372792882696,0.00028778088966609824
+0.0999999999999965,0.63,0.125,50.0,-8.943772922672056e-05,0.00011782372562538556,-0.00017297773917116082,0.00025840931243816055
+0.0999999999999965,0.69,0.125,50.0,-7.601796605864821e-05,0.00010881780690615772,-0.00014339981403395334,0.0002227263987561213
+0.0999999999999965,0.75,0.125,114.0,-6.0523217442892545e-05,7.284660145121362e-05,-0.00011710614207245875,0.00014380021825931904
+0.0999999999999965,0.81,0.125,130.0,-6.681927240501803e-05,7.651898663839281e-05,-0.000128287882180592,0.00015073520450626022
+0.0999999999999965,0.87,0.125,35.0,-4.875721984548137e-06,4.628004193903327e-06,-9.756466462241615e-06,8.60733811172537e-06
+0.1270454343320503,0.33,0.125,9.0,-0.0004604168054960687,0.00045689589571659613,-0.0009250022067461245,0.0008660939987538908
+0.1270454343320503,0.39,0.125,14.0,-0.00014890484408219362,0.00015315530305054327,-0.00027065618623601704,0.00032271671898321055
+0.1270454343320503,0.45,0.125,20.0,-0.00020020102482609737,0.00025710280438208903,-0.0003678645101374908,0.000554367634652736
+0.1270454343320503,0.51,0.125,32.0,-0.00015272580303795543,0.00021642781224341643,-0.00028146367860897286,0.0004637865640071892
+0.1270454343320503,0.57,0.125,44.0,-0.00011480026335917445,0.0001584923385524309,-0.0002150390699340072,0.00033237305824235176
+0.1270454343320503,0.63,0.125,54.0,-0.00010794444153410737,0.00013917566152703382,-0.00020889987045531446,0.0002783507854464468
+0.1270454343320503,0.69,0.125,48.0,-8.968954279509987e-05,0.00011829971950218935,-0.00016080927499929524,0.00024912104537009916
+0.1270454343320503,0.75,0.125,114.0,-6.231915759651175e-05,7.489038344502357e-05,-0.00012344738717270606,0.00014350982924939945
+0.1270454343320503,0.81,0.125,129.0,-6.803013292988005e-05,7.898256151786492e-05,-0.00013373244867855832,0.00015403813511803035
+0.1270454343320503,0.87,0.125,34.0,-6.868129139851506e-06,6.102168292298052e-06,-1.3884063095679133e-05,1.1769264876178872e-05
+0.1614054238462021,0.33,0.125,10.0,-0.0006949969930224564,0.000671021129498849,-0.0013037080577864705,0.001313889962784411
+0.1614054238462021,0.39,0.125,14.0,-0.0002309852509592894,0.0002676660838776882,-0.0004347011222337136,0.0005191505873463874
+0.1614054238462021,0.45,0.125,22.0,-0.00026638872508971434,0.0003310620383790852,-0.0005210588385436983,0.0006564656642693548
+0.1614054238462021,0.51,0.125,30.0,-0.00022698140466623158,0.0003071635552384602,-0.0004212284579844452,0.0006603009472171603
+0.1614054238462021,0.57,0.125,47.0,-0.00016149728182687832,0.00019544134183702407,-0.00029284368563167523,0.00043151263344726155
+0.1614054238462021,0.63,0.125,52.0,-0.0001394774917629935,0.00017439314805340697,-0.0002626012179932239,0.00036554338119301635
+0.1614054238462021,0.69,0.125,47.0,-0.00011205858313133207,0.00013861560069672936,-0.00020123957212956747,0.0003017354579495007
+0.1614054238462021,0.75,0.125,116.0,-7.470462276513481e-05,8.072366200111685e-05,-0.0001462900872383654,0.00015398884821554934
+0.1614054238462021,0.81,0.125,127.0,-7.698479663805575e-05,8.685675745828802e-05,-0.00015641513312981726,0.00017115857934463005
+0.1614054238462021,0.87,0.125,33.0,-1.2340546891061822e-05,1.043023453229893e-05,-2.460140169028661e-05,2.0834739494290117e-05
+0.2050582217609076,0.33,0.125,10.0,-0.0010012576166450655,0.0010044824972528308,-0.0020472504963921466,0.0018859087663307768
+0.2050582217609076,0.39,0.125,16.0,-0.0004231908278704961,0.0003941266362342324,-0.0008614566343248096,0.000757716620372529
+0.2050582217609076,0.45,0.125,22.0,-0.0004309771305223628,0.0005078029141445419,-0.0008118090530363788,0.0009886081550493336
+0.2050582217609076,0.51,0.125,30.0,-0.0003324592995128662,0.0004359152266306611,-0.0006112059640796414,0.000886478993336258
+0.2050582217609076,0.57,0.125,48.0,-0.00023041614300808598,0.0002762435660257546,-0.0004403175749325145,0.0005619187755334865
+0.2050582217609076,0.63,0.125,51.0,-0.0001941565692464348,0.0002423061476771654,-0.0003614120109573834,0.000506474023988061
+0.2050582217609076,0.69,0.125,46.0,-0.00014920082155013561,0.0001790539973820887,-0.00027732158432918413,0.00038519420164741166
+0.2050582217609076,0.75,0.125,117.0,-0.0001084749137975487,0.00010601836715752522,-0.0002190383357136933,0.0002057862127302654
+0.2050582217609076,0.81,0.125,126.0,-9.454328066354847e-05,0.00010504099200338471,-0.0001838869145589258,0.00020969092284911368
+0.2050582217609076,0.87,0.125,32.0,-2.3302284137137628e-05,2.1626729076191894e-05,-4.716145335866271e-05,4.16704415475004e-05
+0.2605171084697407,0.33,0.125,10.0,-0.0014211346676156538,0.0012713564606285591,-0.0027618138318587283,0.002534591913095227
+0.2605171084697407,0.39,0.125,16.0,-0.0006156031102440765,0.0005570513763183192,-0.0012506950661491793,0.001072919496298886
+0.2605171084697407,0.45,0.125,22.0,-0.0005639267379081811,0.000616410345222789,-0.001051624544216321,0.0012891581847476546
+0.2605171084697407,0.51,0.125,34.0,-0.00038396095137560945,0.0004899110621630922,-0.0007401529805710312,0.001013674190744422
+0.2605171084697407,0.57,0.125,46.0,-0.0003203201658021418,0.00036644897344747065,-0.0006270945929307272,0.0007482066668319116
+0.2605171084697407,0.63,0.125,52.0,-0.0002313211743784925,0.0002791254210167425,-0.00044758679631882434,0.000564773380888024
+0.2605171084697407,0.69,0.125,46.0,-0.00018849441359305557,0.000232905301582798,-0.00034929123473332094,0.00047261320882718654
+0.2605171084697407,0.75,0.125,112.0,-0.00015544677641930106,0.00013128398825010346,-0.00032380462439250343,0.00024668321476548896
+0.2605171084697407,0.81,0.125,127.0,-0.00010708843789965918,0.00011317886005903356,-0.00020581826421267268,0.00022228800993862
+0.2605171084697407,0.87,0.125,32.0,-3.0894680499882626e-05,3.0482771000596646e-05,-6.334647002953808e-05,5.558825338307248e-05
+0.3309750919646868,0.33,0.125,12.0,-0.0014974796349407897,0.001345702554366678,-0.0031498445330106193,0.0025194141723537985
+0.3309750919646868,0.39,0.125,16.0,-0.0007667544529917998,0.0006526659329597126,-0.0015763171596007107,0.0012754439522385044
+0.3309750919646868,0.45,0.125,26.0,-0.0007118448199326067,0.0007851993415141825,-0.0013176309920701072,0.0016072561856526652
+0.3309750919646868,0.51,0.125,34.0,-0.0005370093369051629,0.0005829712995166719,-0.0009748756459520601,0.0011898170699444705
+0.3309750919646868,0.57,0.125,46.0,-0.0004309308863771921,0.0004564512431837705,-0.0008114211081842062,0.0009595633515193571
+0.3309750919646868,0.63,0.125,48.0,-0.0003305435293197816,0.00039287899624572387,-0.000634087497240011,0.0007934724404784378
+0.3309750919646868,0.69,0.125,46.0,-0.00024750544455127564,0.00028926119556230585,-0.00047403663789791076,0.0005716281666459561
+0.3309750919646868,0.75,0.125,106.0,-0.00020424817625083427,0.00016664981572027054,-0.0004108470878798171,0.000323952297332332
+0.3309750919646868,0.81,0.125,132.0,-0.00012650734988562428,0.0001284440208766389,-0.0002590421846874308,0.0002625948121491342
+0.3309750919646868,0.87,0.125,31.0,-0.00018019613522126093,8.383105674123746e-05,-0.0004437723658242388,0.0001363611433957021
+0.4204887431174628,0.33,0.125,12.0,-0.001872206606114501,0.0014263012881514305,-0.003764561235042524,0.002807076578688674
+0.4204887431174628,0.39,0.125,20.0,-0.000859817589178186,0.0008319319640637144,-0.0016310523775507398,0.0016433016631440436
+0.4204887431174628,0.45,0.125,26.0,-0.0009321433342167913,0.0010627980297626433,-0.0017621859419245439,0.002145450877131042
+0.4204887431174628,0.51,0.125,38.0,-0.0006366563235239579,0.0007324683900526024,-0.0011728428992656458,0.0015306860825628017
+0.4204887431174628,0.57,0.125,44.0,-0.0006231821154928948,0.0006962334484019037,-0.0012249587835174668,0.0013898697119523727
+0.4204887431174628,0.63,0.125,46.0,-0.00044018892339448815,0.0004676247279063573,-0.0008133117050392742,0.0009735248679802545
+0.4204887431174628,0.69,0.125,47.0,-0.0003246656857392712,0.0003700665012161968,-0.0006154585357153329,0.0007612409895549357
+0.4204887431174628,0.75,0.125,95.0,-0.0002759993361996876,0.00024941533888946,-0.0005612501602172141,0.0004605867983954892
+0.4204887431174628,0.81,0.125,139.0,-0.000166810926615834,0.0001671056336009282,-0.0003189916442080901,0.0003321475857174156
+0.4204887431174628,0.87,0.125,29.0,-0.0002203692185841368,0.00010713778582123732,-0.0005344787815571158,0.00018810211278835312
+0.5342117500109743,0.33,0.125,14.0,-0.0014700925387631282,0.0013012814376037933,-0.0030638858384770353,0.002426708307417143
+0.5342117500109743,0.39,0.125,21.0,-0.0010064636567597926,0.001047376479134575,-0.001988291049202622,0.0020259864701708515
+0.5342117500109743,0.45,0.125,28.0,-0.0013025094252686585,0.001502763483519084,-0.0025925222524298603,0.002985037785899766
+0.5342117500109743,0.51,0.125,42.0,-0.0009253468768327736,0.0009441104238193212,-0.0017397327980153729,0.001982045537461082
+0.5342117500109743,0.57,0.125,38.0,-0.0008108609109722711,0.000871104240035398,-0.0015378923156322626,0.0017615356553733082
+0.5342117500109743,0.63,0.125,45.0,-0.000608270424183883,0.0006395066303394859,-0.0011495003218410015,0.0013318893862342349
+0.5342117500109743,0.69,0.125,48.0,-0.00042071597915530913,0.0004532138999379889,-0.0008330737948523448,0.0008653267190039765
+0.5342117500109743,0.75,0.125,89.0,-0.00039350592184917593,0.0003418729950956871,-0.0008025899300079049,0.0006439857079044834
+0.5342117500109743,0.81,0.125,145.0,-0.00021597146703877514,0.0002200220966315447,-0.00041368297436521217,0.00042971334141934703
+0.5342117500109743,0.87,0.125,25.0,-0.0003446272042075557,0.00018503921824981597,-0.0008354658078458038,0.00031062741973969895
+0.6786916380543195,0.27,0.125,7.0,-0.0032967346432308973,0.003112775473975434,-0.006323237450268146,0.005986538198023084
+0.6786916380543195,0.33,0.125,10.0,-0.001405352254098239,0.0016688834633103995,-0.0026114557416806023,0.0033960151138642146
+0.6786916380543195,0.39,0.125,20.0,-0.0013873505759005589,0.0013214335229733572,-0.0028331266223181003,0.002551611252471318
+0.6786916380543195,0.45,0.125,35.0,-0.0015852068970063926,0.0015794042287267536,-0.0032109720219642784,0.0030089015007615265
+0.6786916380543195,0.51,0.125,40.0,-0.0010939745120432196,0.0011150794684049138,-0.0020551516100779897,0.0022323814112881297
+0.6786916380543195,0.57,0.125,41.0,-0.0008963151800217735,0.0009427844432382407,-0.0017231715559384848,0.0018932883325461201
+0.6786916380543195,0.63,0.125,43.0,-0.0007884765639439772,0.0008042596225925279,-0.0015563267488829635,0.001679105925649344
+0.6786916380543195,0.69,0.125,48.0,-0.0005463964370828989,0.0005724868412022639,-0.0011024509964603045,0.0011116101941042477
+0.6786916380543195,0.75,0.125,81.0,-0.0005082531239809584,0.0004649602183729425,-0.0010495239285420836,0.0008939143502297991
+0.6786916380543195,0.81,0.125,148.0,-0.0002876053167107313,0.0002809823984578971,-0.0005527146376270941,0.0005705909869403231
+0.6786916380543195,0.87,0.125,25.0,-0.0006273290019976441,0.00044096898353743603,-0.0013327685467941902,0.0008239256991746557
+0.8622467393414514,0.27,0.125,8.0,-0.0034227412715611277,0.0033572016692711704,-0.006777247998124363,0.006202852216899951
+0.8622467393414514,0.33,0.125,12.0,-0.001526109790513592,0.0017263646970172466,-0.002990914083746827,0.0034497749705091397
+0.8622467393414514,0.39,0.125,20.0,-0.0018222154601045793,0.0015849923299267364,-0.0038376234396319425,0.0027591919748847955
+0.8622467393414514,0.45,0.125,40.0,-0.0018277236734893113,0.0017060874680495791,-0.0036810634914842435,0.0031959083040984182
+0.8622467393414514,0.51,0.125,37.0,-0.0011635987642724303,0.001258215635452252,-0.0023271518379935838,0.0024717191785539245
+0.8622467393414514,0.57,0.125,41.0,-0.0011093513758362499,0.0011424349369434255,-0.0022220421554881545,0.002238216363992745
+0.8622467393414514,0.63,0.125,44.0,-0.0008497824033726605,0.0008495859643759262,-0.001682360475799983,0.0016059152288835777
+0.8622467393414514,0.69,0.125,47.0,-0.0007405323162345879,0.000721200522759727,-0.0014371854781099545,0.0015072406567064012
+0.8622467393414514,0.75,0.125,77.0,-0.0005676838751679474,0.0005383330797775725,-0.0011583646128571488,0.0010345180576451136
+0.8622467393414514,0.81,0.125,150.0,-0.0004296519913977218,0.0004130099905873499,-0.0008063168716744641,0.0008127494059373962
+0.8622467393414514,0.87,0.125,21.0,-0.001003667668637059,0.0008137114743616144,-0.002019474263397066,0.0015554947032887189
+1.095445115010336,0.27,0.125,8.0,-0.0034952740246861273,0.002814432955818527,-0.007160196417874631,0.005135836921570963
+1.095445115010336,0.33,0.125,16.0,-0.0014341095151474757,0.0017353255351805013,-0.0026953642187708933,0.0036711374910658647
+1.095445115010336,0.39,0.125,16.0,-0.0022202447110029637,0.0016291520378683224,-0.004583672050426454,0.00303313660899414
+1.095445115010336,0.45,0.125,42.0,-0.0018536519393656042,0.0017095637818909397,-0.003912604852914957,0.0032295238839295712
+1.095445115010336,0.51,0.125,37.0,-0.0013105202005372029,0.0014345203042651243,-0.002599825581840269,0.0028292434365153455
+1.095445115010336,0.57,0.125,40.0,-0.0013202001670092637,0.00133795034321892,-0.002631298011229979,0.0026121405946461984
+1.095445115010336,0.63,0.125,41.0,-0.0010045411203091126,0.0010617757720302833,-0.001998808936247297,0.0020622881258092096
+1.095445115010336,0.69,0.125,49.0,-0.0009356200908028113,0.001011511697911956,-0.0018524608617348042,0.0019346402921660278
+1.095445115010336,0.75,0.125,80.0,-0.0006403839469300592,0.0006142782158085951,-0.0012654390342235864,0.0012259067083798686
+1.095445115010336,0.81,0.125,149.0,-0.0005300587077200664,0.0005798904025629063,-0.0010833831874701373,0.0010940166296550965
+1.095445115010336,0.87,0.125,19.0,-0.001341788707602015,0.0011486755379773957,-0.002853126961765049,0.002035368197557566
+1.3917130042341548,0.27,0.125,8.0,-0.0013082223932105175,0.0013540517960073486,-0.0026058953047801503,0.0025941262631535844
+1.3917130042341548,0.33,0.125,15.0,-0.0026439665059906753,0.002700706859131091,-0.005437402505672683,0.0050677112731475245
+1.3917130042341548,0.39,0.125,18.0,-0.002141197288015894,0.0018154024387256522,-0.004537737236652761,0.003353764784746506
+1.3917130042341548,0.45,0.125,34.0,-0.001805187648895275,0.0018048431591966996,-0.0034802844616967864,0.003648826267718258
+1.3917130042341548,0.51,0.125,44.0,-0.0012659266266164817,0.0014508218205175629,-0.0024493485199893633,0.002813566210577816
+1.3917130042341548,0.57,0.125,35.0,-0.0016486487433068275,0.0017453978708258963,-0.0031935819492467004,0.0034163337701804248
+1.3917130042341548,0.63,0.125,43.0,-0.001096394739521422,0.0010249676580062277,-0.002050326059959789,0.0021272504729661244
+1.3917130042341548,0.69,0.125,60.0,-0.0009674564419166667,0.0009615211023499227,-0.0018901170753947837,0.0018927542000026594
+1.3917130042341548,0.75,0.125,105.0,-0.0006735134948243316,0.0006846870202539498,-0.0013840947439989347,0.0013079484057361202
+1.3917130042341548,0.81,0.125,121.0,-0.0006506586274223331,0.0006587068102711974,-0.001272119572984354,0.0012880253715876074
+1.3917130042341548,0.87,0.125,15.0,-0.001287973654006517,0.0010149306761397469,-0.0029237115757951944,0.001733668020473464
+1.7681078308849825,0.27,0.125,8.0,-0.002696768155107443,0.002509717193680122,-0.005438123918532753,0.00458047147026581
+1.7681078308849825,0.33,0.125,14.0,-0.003943360622896369,0.0038087179878751485,-0.007729738390996099,0.007391290692451297
+1.7681078308849825,0.39,0.125,20.0,-0.002608351042966497,0.0022981778516969727,-0.005192658954987985,0.00466613480492955
+1.7681078308849825,0.45,0.125,37.0,-0.0017297925182261243,0.0019192187413830063,-0.0034337012513959327,0.00397876577833114
+1.7681078308849825,0.51,0.125,32.0,-0.0017135442513577096,0.0018791038567390838,-0.003380843773993472,0.0037214479843991686
+1.7681078308849825,0.57,0.125,40.0,-0.0018281412413512373,0.0018598238595849315,-0.003610581011180201,0.0037099098599237316
+1.7681078308849825,0.63,0.125,50.0,-0.0014522904898234478,0.0015331259910942893,-0.002833491242844217,0.002929872944656362
+1.7681078308849825,0.69,0.125,66.0,-0.0012636704094266724,0.0012114252683267217,-0.0024222324103458028,0.002416169468374352
+1.7681078308849825,0.75,0.125,126.0,-0.0007688843009930621,0.0007503242085036688,-0.0015359869101017232,0.0014933315481843116
+1.7681078308849825,0.81,0.125,95.0,-0.0008082713926788432,0.0007927629552823495,-0.0016036516779191652,0.001495211378882759
+1.7681078308849825,0.87,0.125,10.0,-0.00172525794478932,0.0010876978636778726,-0.00380162686049873,0.0018807147375538903
+2.246300273206917,0.27,0.125,8.0,-0.00429136872930323,0.003181465806530805,-0.009000569333004646,0.0058491722258222694
+2.246300273206917,0.33,0.125,18.0,-0.0019629868858029127,0.002084183480587122,-0.0037581161502174883,0.004227736276273669
+2.246300273206917,0.39,0.125,28.0,-0.0016292235783487354,0.0017092446659326334,-0.0032257631427514612,0.0032440943375696297
+2.246300273206917,0.45,0.125,35.0,-0.0014223987771957737,0.0014987371137573707,-0.0027456976703152526,0.0030472830974532707
+2.246300273206917,0.51,0.125,46.0,-0.0016138164720380906,0.001584252224035504,-0.003066198221286094,0.003275175735846807
+2.246300273206917,0.57,0.125,43.0,-0.0015429198708565737,0.0015423169306181433,-0.0029885166879573305,0.0030647148180686047
+2.246300273206917,0.63,0.125,46.0,-0.0012766002970392406,0.0012438036555776344,-0.0024599445224557934,0.0024179345676854243
+2.246300273206917,0.69,0.125,75.0,-0.0010607942257742668,0.001046197377864487,-0.0020360772103696074,0.0021273454115822254
+2.246300273206917,0.75,0.125,127.0,-0.0008075675541899295,0.0007671849485289515,-0.0015768768400277865,0.001555762845346602
+2.246300273206917,0.81,0.125,69.0,-0.0008186618772284044,0.0008032800911547765,-0.0016124105653413914,0.0015930901107931799
+2.85382193849788,0.21,0.125,7.0,-0.002574057853151855,0.0024445039983185734,-0.005036024158404063,0.004736566234893047
+2.85382193849788,0.27,0.125,11.0,-0.0016726323785912552,0.00205421032688111,-0.003369651196524597,0.003950775553328705
+2.85382193849788,0.33,0.125,32.0,-0.0012492105135878842,0.0011434641212305656,-0.0024178708968567567,0.002211252384507624
+2.85382193849788,0.39,0.125,27.0,-0.001241810454876677,0.0011739636312671903,-0.0023602693070330968,0.0023767202581703533
+2.85382193849788,0.45,0.125,54.0,-0.001343949685917688,0.001505409635534887,-0.0026146195642393513,0.002980532872508719
+2.85382193849788,0.51,0.125,47.0,-0.0013140854432050302,0.001337531691852704,-0.002524528397254744,0.002733607371860038
+2.85382193849788,0.57,0.125,47.0,-0.0012512880826562112,0.0011700268483492214,-0.0025871865917333264,0.002350668911994066
+2.85382193849788,0.63,0.125,46.0,-0.0016749391833366077,0.001574261778946785,-0.0032831707238983304,0.0029551841350370315
+2.85382193849788,0.69,0.125,78.0,-0.001343154378888985,0.0011411827895660032,-0.0026713023634665624,0.002298495490162058
+2.85382193849788,0.75,0.125,110.0,-0.00101647629599488,0.0008810826766073955,-0.001975178846166086,0.0018024227203977967
+2.85382193849788,0.81,0.125,38.0,-0.001270583569665907,0.0011080542878316843,-0.0025646671208414762,0.0021567307725078506
+3.62565047682813,0.21,0.125,12.0,-0.002477724927127139,0.001544645908915717,-0.005016833596190743,0.002912782060753425
+3.62565047682813,0.27,0.125,19.0,-0.00216694700921581,0.0020898715075045983,-0.004253844308710515,0.00412980076757499
+3.62565047682813,0.33,0.125,30.0,-0.0013418686036306623,0.0013740870507724058,-0.00247419423697441,0.0029635011458820876
+3.62565047682813,0.39,0.125,48.0,-0.001320159674841557,0.0013022881743907089,-0.002555202893545719,0.0024728395018150493
+3.62565047682813,0.45,0.125,46.0,-0.0014683613692467233,0.0014992000014491102,-0.0027933596308006257,0.002990774990924916
+3.62565047682813,0.51,0.125,45.0,-0.0015263599883705012,0.0015514637167654893,-0.0030815041258691685,0.0028987113322667788
+3.62565047682813,0.57,0.125,40.0,-0.0019966156824034642,0.0017101778752562698,-0.0040474778860875174,0.0032813068050638575
+3.62565047682813,0.63,0.125,41.0,-0.0024710423853626243,0.002325849136930944,-0.004985910675884483,0.004514266831886496
+3.62565047682813,0.69,0.125,64.0,-0.0016425859642820583,0.0014006059608389738,-0.003404473042193715,0.0027873670046421476
+3.62565047682813,0.75,0.125,125.0,-0.0009389873817729653,0.0009372111404564967,-0.0018949165778556832,0.0018395146353309495
+3.62565047682813,0.81,0.125,28.0,-0.0014674457076123664,0.0014708517716926224,-0.0027819870950456503,0.0029093583620743773
+4.606223395648531,0.21,0.125,13.0,-0.002134614489789254,0.00221283357732011,-0.004185750304145614,0.004491601060116204
+4.606223395648531,0.27,0.125,31.0,-0.0017083522435620523,0.0017403100544766076,-0.003324285670338427,0.003371539584785124
+4.606223395648531,0.33,0.125,42.0,-0.0016591145367722748,0.0017216546761851012,-0.003369770746909321,0.003260988358130591
+4.606223395648531,0.39,0.125,56.0,-0.0014982496961190713,0.0014698854088594233,-0.0029027186465732206,0.0028959608312123697
+4.606223395648531,0.45,0.125,44.0,-0.0019158427710655069,0.001953798037462835,-0.0038587296670612513,0.0038937447755105206
+4.606223395648531,0.51,0.125,43.0,-0.0021905437783518544,0.0018795586349848153,-0.004348455994441188,0.003639305344052638
+4.606223395648531,0.57,0.125,42.0,-0.0025181319824781837,0.0023560651911114106,-0.005039434085846067,0.004427765935280849
+4.606223395648531,0.63,0.125,52.0,-0.0024180517393174697,0.002320051477939284,-0.004673618625266326,0.004323351777022334
+4.606223395648531,0.69,0.125,86.0,-0.0014581375356022869,0.0013660650712726886,-0.0028198277638153274,0.002754668879294799
+4.606223395648531,0.75,0.125,77.0,-0.0013575872483847498,0.0014841063312924267,-0.002686484171638388,0.0028136425058936662
+4.606223395648531,0.81,0.125,12.0,-0.003267366616836303,0.0031630875905846504,-0.006656827188861125,0.005848767525162828
+5.851996519306441,0.15,0.125,10.0,-0.0016236634867302965,0.0018966848072851815,-0.0032057513127935243,0.003564500831957971
+5.851996519306441,0.21,0.125,22.0,-0.001791670382565771,0.0019210074469753165,-0.003475042417564123,0.0039024693194839016
+5.851996519306441,0.27,0.125,36.0,-0.0019726709085806328,0.0020898981979602968,-0.0040404166027687705,0.003933289041122328
+5.851996519306441,0.33,0.125,53.0,-0.001538483535344319,0.0014532619734629073,-0.003103408128049972,0.0030300061638438933
+5.851996519306441,0.39,0.125,52.0,-0.0017696546627839597,0.0019727638487042317,-0.003519109684214994,0.003747341242760533
+5.851996519306441,0.45,0.125,50.0,-0.002364173214907892,0.0022237004585738806,-0.004785856406384205,0.004291357946929659
+5.851996519306441,0.51,0.125,45.0,-0.0031386817061228732,0.0027898453187170393,-0.006301885274844766,0.005453588498924035
+5.851996519306441,0.57,0.125,48.0,-0.002777907119014548,0.0022226211235859303,-0.0056379206734810585,0.004312624965102478
+5.851996519306441,0.63,0.125,54.0,-0.0024983413724205964,0.0023384911912594803,-0.005246461476266476,0.0044586328390176354
+5.851996519306441,0.69,0.125,90.0,-0.0016925689816129571,0.0016997672590342797,-0.003582546161580804,0.0030464028880394737
+5.851996519306441,0.75,0.125,34.0,-0.0026166281040754685,0.0026707156704819696,-0.005263425783083016,0.005211782795192385
+5.851996519306441,0.81,0.125,6.0,-0.0060217843195161285,0.0045264375093193405,-0.012170587619942183,0.008373817403692925
+7.434694395049633,0.15,0.125,10.0,-0.002758803531266297,0.002046471174001436,-0.005755892152924575,0.0036854529289716024
+7.434694395049633,0.21,0.125,30.0,-0.001731245130135548,0.0017656468687380128,-0.003356837448823861,0.0034322567570975312
+7.434694395049633,0.27,0.125,45.0,-0.0018703918441010266,0.0017764633327530081,-0.0035566346187335344,0.0036308360177919863
+7.434694395049633,0.33,0.125,57.0,-0.0015009155769534488,0.0015824103762068224,-0.002935828855471153,0.0030480426805575217
+7.434694395049633,0.39,0.125,58.0,-0.0016675211707016105,0.0016551612394027275,-0.003255005404819003,0.003270157754946792
+7.434694395049633,0.45,0.125,52.0,-0.002176125440297541,0.0021062919305364445,-0.004287225170102578,0.004266963983035107
+7.434694395049633,0.51,0.125,41.0,-0.0026215709733628956,0.002120548080993543,-0.00533452361206026,0.004225001274225289
+7.434694395049633,0.57,0.125,48.0,-0.002227076084678324,0.002372706470145675,-0.0044810168867107985,0.004717326763901737
+7.434694395049633,0.63,0.125,75.0,-0.0021067335924726443,0.0018828403043464534,-0.004152634691830176,0.003704501214348803
+7.434694395049633,0.69,0.125,66.0,-0.0023211538468872034,0.002284618657242999,-0.0044908018566927575,0.004471492769553852
+7.434694395049633,0.75,0.125,14.0,-0.00370510191717307,0.003690978170545831,-0.007561137344581197,0.007131068432133763
+9.44543978545179,0.15,0.125,14.0,-0.002764241383520815,0.002339210257953007,-0.005440433231068321,0.004589122044004135
+9.44543978545179,0.21,0.125,35.0,-0.0018996902854317539,0.0019901721483189744,-0.0035038828639899493,0.004221909521798445
+9.44543978545179,0.27,0.125,62.0,-0.0019012684479698917,0.0018319227922480403,-0.003683979329691426,0.0037167892961897913
+9.44543978545179,0.33,0.125,67.0,-0.0018461433624605496,0.001995119096607575,-0.003616713740978345,0.003876268924385712
+9.44543978545179,0.39,0.125,62.0,-0.0018745320361264368,0.0019413186466658316,-0.003636440175738122,0.0037832233458928543
+9.44543978545179,0.45,0.125,55.0,-0.0021520440634732454,0.00219054543981442,-0.004345542720164839,0.004489650055282025
+9.44543978545179,0.51,0.125,46.0,-0.002825407930701003,0.002980778801252697,-0.005397462361105783,0.006086728590329366
+9.44543978545179,0.57,0.125,51.0,-0.0026245120162951365,0.002491122817001134,-0.005219360459382105,0.004791025971729964
+9.44543978545179,0.63,0.125,65.0,-0.0030169418505165972,0.002894751951102216,-0.005940800963830783,0.005902390023968179
+9.44543978545179,0.69,0.125,35.0,-0.0035681675131119324,0.003579654034296209,-0.006872465903758681,0.007098493970478005
+12.000000000000002,0.15,0.125,18.0,-0.0017837014352588988,0.0016735912851680362,-0.0035302309212272972,0.0031941285141063986
+12.000000000000002,0.21,0.125,32.0,-0.0025551268430684423,0.0026161024199892434,-0.004862878019390418,0.005310635367965043
+12.000000000000002,0.27,0.125,62.0,-0.002746000501286837,0.0028265003794727623,-0.005510636674869744,0.005699736035788965
+12.000000000000002,0.33,0.125,80.0,-0.0021629826724674354,0.0020121644247965533,-0.004257707525609027,0.0038570139234951014
+12.000000000000002,0.39,0.125,70.0,-0.0021500645917803215,0.0019319423381025705,-0.004427873698485818,0.0038363951219077415
+12.000000000000002,0.45,0.125,64.0,-0.001921636555113833,0.0020252982508366366,-0.003695673913965532,0.00411249092212584
+12.000000000000002,0.51,0.125,50.0,-0.0025930807409406116,0.0029565202842985394,-0.005216712188731165,0.005681878666140678
+12.000000000000002,0.57,0.125,48.0,-0.0041426268416281,0.003999313220945655,-0.00876641742988391,0.0077781257373868585
+12.000000000000002,0.63,0.125,40.0,-0.004644950999955979,0.0039894511657627835,-0.009311065151450805,0.007603884449118332
+12.000000000000002,0.69,0.125,24.0,-0.006557356647190802,0.006010531787130814,-0.01231670353153279,0.01258843408049915
+12.000000000000002,0.75,0.125,6.0,-0.018617682060644333,0.015496081486959795,-0.03962837804274048,0.02666220584076506
+0.1000000000000064,0.27,0.5,8.0,-0.00021796357450813708,0.0001437131433116995,-0.00045893199666165174,0.00025460476982928915
+0.1000000000000064,0.33,0.5,21.0,-6.534035166785786e-05,5.401734936079616e-05,-0.00013739906144004158,0.00010427020479658035
+0.1000000000000064,0.39,0.5,32.0,-5.6250612633519244e-05,0.0001046002684391431,-9.691057264297253e-05,0.00023676076692642222
+0.1000000000000064,0.45,0.5,29.0,-0.00011497199263012959,0.00015257774210492204,-0.0002060282575558746,0.00033327244571137137
+0.1000000000000064,0.51,0.5,48.0,-7.372981643917913e-05,0.00010562299652185463,-0.00013697950411933207,0.0002180208310721918
+0.1000000000000064,0.57,0.5,33.0,-9.637403101450807e-05,0.00013357381840878473,-0.00018214903889667017,0.0002728388370880569
+0.1000000000000064,0.63,0.5,45.0,-7.904371881533036e-05,0.00010464861665009917,-0.00014308425708066248,0.0002200956154506569
+0.1000000000000064,0.69,0.5,59.0,-7.79909592667403e-05,9.157779107889039e-05,-0.00014303147357894576,0.00019003224086832084
+0.1000000000000064,0.75,0.5,107.0,-4.7614709220381786e-05,5.808473676654564e-05,-9.290049936509114e-05,0.00011991809567861104
+0.1000000000000064,0.81,0.5,104.0,-7.446928504179016e-05,8.172418655135362e-05,-0.00014523303210826904,0.00014750678088149184
+0.1000000000000064,0.87,0.5,10.0,-4.6737552857777824e-06,4.684351282958483e-06,-9.06589114251556e-06,8.98290048021444e-06
+0.1270454343320617,0.27,0.5,9.0,-0.0002795938422586107,0.00024340968269346652,-0.0005745071381257164,0.0004653299959890234
+0.1270454343320617,0.33,0.5,20.0,-9.375207743070347e-05,7.86757780358069e-05,-0.00019553775764522783,0.000153085591538606
+0.1270454343320617,0.39,0.5,32.0,-7.066247717587573e-05,0.00011856980390278071,-0.0001280549136971779,0.0002707939334440486
+0.1270454343320617,0.45,0.5,31.0,-0.00013067807046455467,0.00017522430827475,-0.00024066446319714538,0.0003783780768660061
+0.1270454343320617,0.51,0.5,46.0,-8.93074969576498e-05,0.00012304252095383388,-0.00017099854365192646,0.00027324690653183635
+0.1270454343320617,0.57,0.5,35.0,-0.00010838909879714082,0.00013672997629920122,-0.00019875624417235626,0.0003056670146421633
+0.1270454343320617,0.63,0.5,45.0,-8.967047068776985e-05,0.0001133703551955859,-0.0001608429397306767,0.00024102900483341072
+0.1270454343320617,0.69,0.5,58.0,-8.40530865821338e-05,0.00010357339169777555,-0.00016177639438555056,0.00021238194466384968
+0.1270454343320617,0.75,0.5,107.0,-4.8697825133220585e-05,5.613622890695667e-05,-9.188323804496044e-05,0.000114899849901461
+0.1270454343320617,0.81,0.5,103.0,-7.969858776192803e-05,7.348434944210762e-05,-0.0001491377751321958,0.00015585045295763724
+0.1270454343320617,0.87,0.5,10.0,-6.480952069211372e-06,5.949226171452292e-06,-1.3109605213338535e-05,1.1561040791821108e-05
+0.1614054238462062,0.27,0.5,9.0,-0.0004356943779327497,0.000425845521960681,-0.0008992214630247414,0.0008027375545724744
+0.1614054238462062,0.33,0.5,20.0,-0.00014127943740739572,0.00012597789193840762,-0.00028074357986136077,0.000242313404798053
+0.1614054238462062,0.39,0.5,32.0,-0.0001062939725212203,0.00014844940323930175,-0.0001858614164948675,0.0003376258464857288
+0.1614054238462062,0.45,0.5,31.0,-0.00018329037676217502,0.00023166102358873928,-0.00034083533546474187,0.0004979808810650439
+0.1614054238462062,0.51,0.5,47.0,-0.0001232763739191628,0.00015027993458258473,-0.00022547332749773275,0.00031543650069550886
+0.1614054238462062,0.57,0.5,39.0,-0.0001372028612545583,0.0001780862934298555,-0.0002518864715280852,0.00037535732978910655
+0.1614054238462062,0.63,0.5,41.0,-0.0001059839808772458,0.00014385874440182823,-0.00019899810077198031,0.0002834543459305694
+0.1614054238462062,0.69,0.5,59.0,-0.00010942171441133812,0.00011591958477519527,-0.0002014081434585021,0.00024225343197973695
+0.1614054238462062,0.75,0.5,107.0,-4.9473772310436326e-05,6.046704704857461e-05,-9.585239800791962e-05,0.00012497953884737516
+0.1614054238462062,0.81,0.5,101.0,-8.248662169145673e-05,8.596323239516041e-05,-0.00015416393893168037,0.00016944846000414593
+0.1614054238462062,0.87,0.5,10.0,-1.0293459525939325e-05,9.666050385282117e-06,-1.9568303668163297e-05,2.0105972338889507e-05
+0.2050582217609147,0.27,0.5,9.0,-0.0006958190625772741,0.0006313189522592818,-0.0013850127301685271,0.0012202921307045997
+0.2050582217609147,0.33,0.5,20.0,-0.0002268499988065328,0.00020566156703540148,-0.00043777340807935885,0.00041427438751368223
+0.2050582217609147,0.39,0.5,32.0,-0.0001691082746148168,0.00022358691423760398,-0.0002976089376834028,0.0004793506906707466
+0.2050582217609147,0.45,0.5,33.0,-0.0002583961817999047,0.00033343633211431456,-0.0004837575780422194,0.0006748299622298624
+0.2050582217609147,0.51,0.5,45.0,-0.00018542376640412963,0.00023421508066153392,-0.00034465080537062295,0.00046273621097443914
+0.2050582217609147,0.57,0.5,41.0,-0.0001840017471173274,0.0002461460911848774,-0.0003593623865897969,0.0004907463600595088
+0.2050582217609147,0.63,0.5,42.0,-0.00013485488032996022,0.00017620226537431042,-0.0002460025762944597,0.0003763509933872841
+0.2050582217609147,0.69,0.5,56.0,-0.00013994776218737736,0.0001567067139415994,-0.0002746084199492073,0.0003058644958953815
+0.2050582217609147,0.75,0.5,109.0,-6.378656023468342e-05,7.666028911080374e-05,-0.00012045319724285293,0.0001527304479157593
+0.2050582217609147,0.81,0.5,99.0,-9.590801208378904e-05,0.00010088938070131577,-0.00019545208485796707,0.00019340036058790032
+0.2050582217609147,0.87,0.5,10.0,-1.888533874530497e-05,2.2049362899190216e-05,-3.687623898371789e-05,4.208762916009243e-05
+0.2605171084697273,0.27,0.5,9.0,-0.0010136441465618622,0.000898809106216245,-0.002090224489746445,0.0017073280209631179
+0.2605171084697273,0.33,0.5,20.0,-0.00037606622836597385,0.000355161998909601,-0.0007403354239637739,0.0006846933567549818
+0.2605171084697273,0.39,0.5,31.0,-0.0002519838643937253,0.0002954413766645134,-0.00045715476467775876,0.000611047096637007
+0.2605171084697273,0.45,0.5,34.0,-0.00038473370496440906,0.0004397879856917748,-0.0007099247747184462,0.0009312017083611953
+0.2605171084697273,0.51,0.5,46.0,-0.0002442817909341781,0.00028062757910281305,-0.000453278415765905,0.0005961641483380047
+0.2605171084697273,0.57,0.5,42.0,-0.000254867239985731,0.00028108677336021246,-0.00045919261360193926,0.0006105441138209439
+0.2605171084697273,0.63,0.5,44.0,-0.00015501492177359834,0.000209507560601858,-0.0002939407233638859,0.00043110415254611547
+0.2605171084697273,0.69,0.5,54.0,-0.000167373115700189,0.0001845965648990568,-0.00032369174482068004,0.00037824612040484023
+0.2605171084697273,0.75,0.5,108.0,-7.27920712373341e-05,8.403175010626354e-05,-0.00013408503861483454,0.00017383656578018442
+0.2605171084697273,0.81,0.5,98.0,-0.00010617009747879533,0.00010742698455322059,-0.00020317778545747813,0.0002104398934696091
+0.2605171084697273,0.87,0.5,10.0,-2.80861060420163e-05,3.26201340832055e-05,-5.5619164666302394e-05,6.146032234947595e-05
+0.3309750919646941,0.27,0.5,10.0,-0.0010911414246592831,0.0010230354292434056,-0.002229652270545184,0.002007213347576357
+0.3309750919646941,0.33,0.5,18.0,-0.0006325676822082327,0.0007154513186032967,-0.0012743285979579454,0.00137381535447012
+0.3309750919646941,0.39,0.5,31.0,-0.0003668666328042369,0.0004126448898488313,-0.0007081717816411288,0.000852799076092695
+0.3309750919646941,0.45,0.5,37.0,-0.0005004657840456659,0.0005995674336249555,-0.0009631739055050155,0.001185259499638231
+0.3309750919646941,0.51,0.5,45.0,-0.0003357750546064437,0.000403691461456061,-0.0006610613503234988,0.0008132192588238807
+0.3309750919646941,0.57,0.5,46.0,-0.00029157318671707886,0.0003765817601541025,-0.0005728444034141036,0.0007677502167358436
+0.3309750919646941,0.63,0.5,41.0,-0.00021734778424663202,0.00029621206256987546,-0.0004031929883480334,0.000620400392317849
+0.3309750919646941,0.69,0.5,55.0,-0.00021348688297358206,0.00022221344140191659,-0.00039535050037546734,0.0004666055953651223
+0.3309750919646941,0.75,0.5,105.0,-8.519914505982091e-05,9.91477600572405e-05,-0.00016356210481532901,0.0002010357924602451
+0.3309750919646941,0.81,0.5,97.0,-0.0001225232436595189,0.00011663192940583822,-0.0002302492225390738,0.0002398961763779953
+0.3309750919646941,0.87,0.5,10.0,-4.2294615920543475e-05,4.3215123972465586e-05,-8.0956166523527e-05,9.196412787921346e-05
+0.4204887431174585,0.27,0.5,10.0,-0.001393653808857982,0.0013921427320846044,-0.0027188617221579094,0.0027813423412414964
+0.4204887431174585,0.33,0.5,20.0,-0.0009793019850202172,0.0009847340056901588,-0.0018191087267114077,0.002010031196749623
+0.4204887431174585,0.39,0.5,30.0,-0.0005255615934520453,0.0006569830093915988,-0.0010569576458059628,0.0012820967084387863
+0.4204887431174585,0.45,0.5,41.0,-0.0006420964931840822,0.0007754888088076587,-0.0012504866665296126,0.0015271604955598153
+0.4204887431174585,0.51,0.5,45.0,-0.0005166866101501144,0.00052683684684529,-0.0009632803617077992,0.001090694317826783
+0.4204887431174585,0.57,0.5,42.0,-0.00042109063415052495,0.0005250708507702931,-0.0007910206762636173,0.0010802242741479045
+0.4204887431174585,0.63,0.5,46.0,-0.0002916136763007831,0.00038103652807110465,-0.0005703812522093599,0.0007416227332347518
+0.4204887431174585,0.69,0.5,52.0,-0.0002675674442265764,0.00029620516698683074,-0.0005304846607105952,0.0006045625738308865
+0.4204887431174585,0.75,0.5,105.0,-0.00011190522266737914,0.00012814971721930463,-0.0002108775747180872,0.0002635263670831396
+0.4204887431174585,0.81,0.5,95.0,-0.00013699745192027418,0.00014680775528694734,-0.000267768025436003,0.0002870766182874118
+0.4204887431174585,0.87,0.5,9.0,-6.125952342403738e-05,6.753771868485193e-05,-0.0001235808285981057,0.00012600006456631174
+0.5342117500109825,0.21,0.5,6.0,-0.002356458032160511,0.0024597359572518704,-0.004421545996565153,0.004965208921746234
+0.5342117500109825,0.27,0.5,10.0,-0.0025823006933415487,0.0023774899678944738,-0.0051895739019936025,0.00437177649946373
+0.5342117500109825,0.33,0.5,24.0,-0.0012020233009020782,0.0011988521393488166,-0.0022435189240747762,0.002409045835921166
+0.5342117500109825,0.39,0.5,25.0,-0.0009312020638599891,0.0010699458749839608,-0.0019024696956627194,0.0022215085789415345
+0.5342117500109825,0.45,0.5,43.0,-0.0008767719454792615,0.0009592608692218298,-0.0016002083286878015,0.0020344037289548368
+0.5342117500109825,0.51,0.5,45.0,-0.0006618642591094972,0.0007940026907132659,-0.0013250457168775937,0.0015574383092999658
+0.5342117500109825,0.57,0.5,41.0,-0.0006287107823425098,0.0007207740117282987,-0.0011528225852164065,0.001451716052641968
+0.5342117500109825,0.63,0.5,50.0,-0.00039300958014503503,0.00044404424917939716,-0.0007399657104285833,0.0009484072641613113
+0.5342117500109825,0.69,0.5,51.0,-0.0003747420772948411,0.00041593132431301847,-0.0007256173375369751,0.0008212598935930865
+0.5342117500109825,0.75,0.5,99.0,-0.00014598273584372546,0.00017227445639164543,-0.0002851322938582594,0.0003422591216953465
+0.5342117500109825,0.81,0.5,99.0,-0.00018790336142644393,0.00017642220058750716,-0.0003616481658777012,0.00035423989902191513
+0.5342117500109825,0.87,0.5,6.0,-0.0001260155432506461,9.297701420435393e-05,-0.00025042876811300546,0.0001694770297168505
+0.6786916380543135,0.21,0.5,7.0,-0.0030209346880088086,0.0028411375866723393,-0.005908878090287698,0.005390076994308554
+0.6786916380543135,0.27,0.5,10.0,-0.0035939659019193168,0.0030797005143655474,-0.006905139647934027,0.006127669211532458
+0.6786916380543135,0.33,0.5,24.0,-0.0019083328460686947,0.0018225603138611773,-0.0035498677513510664,0.0035779076567382414
+0.6786916380543135,0.39,0.5,27.0,-0.0012438415464000332,0.0012828073898827406,-0.00236919352593201,0.002646657426853783
+0.6786916380543135,0.45,0.5,42.0,-0.001112684836968187,0.0011987150801994325,-0.002111378731869792,0.0024968012017755766
+0.6786916380543135,0.51,0.5,48.0,-0.0008454231539466254,0.0009591470048489393,-0.0016758219002139876,0.001881831450669687
+0.6786916380543135,0.57,0.5,42.0,-0.0006912124368469611,0.0007674048793456063,-0.0013187392962257065,0.0015161941250453764
+0.6786916380543135,0.63,0.5,45.0,-0.0005457228285155675,0.0006179292231633604,-0.0010666262747575925,0.0012276102851228512
+0.6786916380543135,0.69,0.5,53.0,-0.00047267521009112514,0.0004972913588575665,-0.0009057535675020968,0.0009578598275059825
+0.6786916380543135,0.75,0.5,95.0,-0.00021319812991735316,0.00022756550130688757,-0.0003998944169114438,0.00045732874215848035
+0.6786916380543135,0.81,0.5,101.0,-0.0002480599150131195,0.00025673623407422835,-0.00048192546268334614,0.00048070520194242003
+0.6786916380543135,0.87,0.5,5.0,-0.0002223134749926194,0.00018504789301743136,-0.00042351405800564754,0.0003409031337601396
+0.8622467393414459,0.21,0.5,9.0,-0.0038746228607601844,0.0031869547381232224,-0.007387976684532279,0.006111731729525142
+0.8622467393414459,0.27,0.5,11.0,-0.00410800442926625,0.004609032847286798,-0.007981454270919971,0.009342884016253555
+0.8622467393414459,0.33,0.5,24.0,-0.002261657213701967,0.0019812904242971397,-0.004344735972214648,0.0039991059747368635
+0.8622467393414459,0.39,0.5,30.0,-0.001679783965130973,0.0016580386892683374,-0.0032635430540060716,0.00328717816916248
+0.8622467393414459,0.45,0.5,43.0,-0.0012427861491280388,0.0013267904606352738,-0.002434986590029727,0.0026479181077099638
+0.8622467393414459,0.51,0.5,50.0,-0.0009351175224373385,0.0010759603838738907,-0.0018734619868899125,0.0020960703704205577
+0.8622467393414459,0.57,0.5,36.0,-0.000985809197115088,0.0009225137056653193,-0.0019370267362141982,0.001741832588205599
+0.8622467393414459,0.63,0.5,46.0,-0.0007175376506543623,0.0007630311861951418,-0.0014194803222033515,0.0015253550135168612
+0.8622467393414459,0.69,0.5,51.0,-0.0006072666906232915,0.0006157757066040314,-0.0011557086125193975,0.0012285454803218322
+0.8622467393414459,0.75,0.5,98.0,-0.00030639906762240627,0.0003413128674501231,-0.0005955622562606198,0.0006795336472719376
+0.8622467393414459,0.81,0.5,98.0,-0.0003685578268034377,0.00037063199499922695,-0.0007369879537804953,0.0007023673536985615
+1.095445115010328,0.21,0.5,9.0,-0.0039206874788131835,0.0035226674825096175,-0.007649061191401285,0.006787691817886522
+1.095445115010328,0.27,0.5,12.0,-0.00442012115821514,0.004781387923101607,-0.008950427262028637,0.009048710403589117
+1.095445115010328,0.33,0.5,26.0,-0.0023137823424605403,0.0021845307601499795,-0.004787453654480133,0.004063668244452421
+1.095445115010328,0.39,0.5,31.0,-0.0020720688857527618,0.001988572079846006,-0.004006249868075155,0.004258822585556039
+1.095445115010328,0.45,0.5,44.0,-0.001401224589248173,0.001411026566591381,-0.0028277378296203775,0.0028503121853997834
+1.095445115010328,0.51,0.5,46.0,-0.0012072537488875344,0.0013509474854120304,-0.0022923942600347356,0.002643355720242115
+1.095445115010328,0.57,0.5,41.0,-0.0011013022717088921,0.0010513545684701958,-0.002297500344290744,0.0020917334235305792
+1.095445115010328,0.63,0.5,45.0,-0.0009478400162281534,0.0009848121875093109,-0.0018946934244259812,0.0019116538360679737
+1.095445115010328,0.69,0.5,50.0,-0.0007916298796197826,0.0008717543725955627,-0.001563311416953725,0.0016545012610434586
+1.095445115010328,0.75,0.5,97.0,-0.0004321246126714886,0.00047718988037954063,-0.0008250034165773015,0.0009642153447984776
+1.095445115010328,0.81,0.5,96.0,-0.0005712576713063973,0.0005316888864646195,-0.0011116665934422108,0.0010252439575330471
+1.391713004234154,0.21,0.5,9.0,-0.002892370398674181,0.0031830239175867016,-0.005423579533778697,0.00613858286156182
+1.391713004234154,0.27,0.5,17.0,-0.0031718664114690448,0.003408547386418606,-0.006214057001230425,0.006740355400021925
+1.391713004234154,0.33,0.5,27.0,-0.00213312086816789,0.0016863921910012553,-0.004359242996319959,0.003211399367326077
+1.391713004234154,0.39,0.5,33.0,-0.0016910183648312298,0.001790215660224025,-0.003384132048002519,0.003580634670523488
+1.391713004234154,0.45,0.5,47.0,-0.001435216923499138,0.0013586067110763725,-0.002754864329273249,0.0027142727109651247
+1.391713004234154,0.51,0.5,39.0,-0.0013436056889583009,0.0015460659569871149,-0.002775725925492772,0.00292554962796546
+1.391713004234154,0.57,0.5,42.0,-0.0012557344076248639,0.0012661829825209795,-0.002550216011158487,0.002413877019581807
+1.391713004234154,0.63,0.5,49.0,-0.0009891989576265273,0.0010085316665004785,-0.0019938900378318842,0.00196600349487365
+1.391713004234154,0.69,0.5,50.0,-0.0009292947614887062,0.0010006697559984351,-0.0018099601508044967,0.0020644825328816666
+1.391713004234154,0.75,0.5,107.0,-0.0005300390279792934,0.0005445754373090089,-0.0010454920121326667,0.0010746215575286968
+1.391713004234154,0.81,0.5,78.0,-0.0007398353129890952,0.0006936996318922328,-0.0014805957540916003,0.0013323622240232324
+1.7681078308849796,0.21,0.5,9.0,-0.0031583861284251395,0.003861414486129594,-0.00606798279128552,0.007537302597600267
+1.7681078308849796,0.27,0.5,18.0,-0.002195467067792378,0.0023179991031840462,-0.004244201648797831,0.004626317481539821
+1.7681078308849796,0.33,0.5,28.0,-0.0017378183674858078,0.0014684451361198076,-0.003728478851408011,0.002751652699600252
+1.7681078308849796,0.39,0.5,43.0,-0.0013337073463355231,0.0014024386740913747,-0.002701241564005793,0.0026378347932449844
+1.7681078308849796,0.45,0.5,41.0,-0.0014347221189352185,0.0012957779379770419,-0.0028164355703788092,0.002527021575383429
+1.7681078308849796,0.51,0.5,43.0,-0.0014457121878166078,0.0015108274240498013,-0.002819856452858594,0.003068961147985198
+1.7681078308849796,0.57,0.5,41.0,-0.0010434017383385754,0.0011279424957750888,-0.0019498387939682776,0.002338781773366123
+1.7681078308849796,0.63,0.5,54.0,-0.0010947673381356692,0.0011673780588025424,-0.0021473815125120457,0.002279929918684076
+1.7681078308849796,0.69,0.5,53.0,-0.0008476019459449087,0.0008484160649050223,-0.0016637797120964675,0.0016824947607687862
+1.7681078308849796,0.75,0.5,117.0,-0.0006154573477108237,0.0005992970467697417,-0.001216218620446393,0.0011670642808700006
+1.7681078308849796,0.81,0.5,50.0,-0.0009374338828322437,0.0007554619316045109,-0.0019420658540036722,0.0014437321115046305
+2.2463002732069235,0.21,0.5,11.0,-0.00403759458789623,0.003420728350127364,-0.008362857269623348,0.006542028767468344
+2.2463002732069235,0.27,0.5,26.0,-0.0015711876142326616,0.001452540183569921,-0.0033817374007087913,0.002685097969126174
+2.2463002732069235,0.33,0.5,25.0,-0.0020974790614884343,0.0017873446832267362,-0.004210626410151774,0.0034006600794194305
+2.2463002732069235,0.39,0.5,50.0,-0.0012738203494898305,0.001343763407677245,-0.0026960867547255645,0.0024931709507608835
+2.2463002732069235,0.45,0.5,44.0,-0.001385495517923341,0.0013337545897153455,-0.0028377710024134234,0.002504330245616281
+2.2463002732069235,0.51,0.5,41.0,-0.0013241324430623143,0.0013421122146334392,-0.0025381307025086276,0.0027198980803622035
+2.2463002732069235,0.57,0.5,45.0,-0.0012029060732922934,0.0012361381639374462,-0.0024303794055040733,0.0024604785653061824
+2.2463002732069235,0.63,0.5,45.0,-0.0012889915762529403,0.001290460178346197,-0.0025699893309159547,0.0025840898474186248
+2.2463002732069235,0.69,0.5,64.0,-0.0009509248934722614,0.0009071733860235572,-0.0018692099366336386,0.0018602436006887658
+2.2463002732069235,0.75,0.5,103.0,-0.0007432774819983665,0.0007277294638416934,-0.0015014230231932132,0.0014299266356085137
+2.2463002732069235,0.81,0.5,44.0,-0.001220614758052412,0.0009650947113139025,-0.002614661753204746,0.0017762740802878452
+2.8538219384978856,0.21,0.5,13.0,-0.002061282984742943,0.0020648444789931383,-0.003978123506017336,0.00404312350850639
+2.8538219384978856,0.27,0.5,33.0,-0.0014932866662694417,0.0014514889091221145,-0.0029649403956363554,0.0029091278072480337
+2.8538219384978856,0.33,0.5,31.0,-0.0018297316638961696,0.0015989445039205372,-0.0033636656458752227,0.0032904632506276887
+2.8538219384978856,0.39,0.5,44.0,-0.0014341209186889416,0.001370202937839513,-0.0028287437114300003,0.002666647898458234
+2.8538219384978856,0.45,0.5,51.0,-0.0011888969619740012,0.0010944303067958608,-0.002359215290672493,0.00215137030098646
+2.8538219384978856,0.51,0.5,40.0,-0.001163025534753516,0.0011125680348999872,-0.002339722825351587,0.002144852605291698
+2.8538219384978856,0.57,0.5,48.0,-0.0009851352852524504,0.0009323934945807609,-0.0019498537131906785,0.0018223141347243725
+2.8538219384978856,0.63,0.5,43.0,-0.0012588368445866395,0.0014403750118888563,-0.002480188224921441,0.002935090371412256
+2.8538219384978856,0.69,0.5,56.0,-0.0008628521381120642,0.0008613366255823819,-0.0016995306253291718,0.0016512415764743456
+2.8538219384978856,0.75,0.5,107.0,-0.0007161448346352346,0.0007911198207034375,-0.0015110223258768278,0.0014075032251116882
+2.8538219384978856,0.81,0.5,32.0,-0.0012961063554423936,0.001018024090495724,-0.0025996828712055893,0.001956510795983033
+3.6256504768281257,0.21,0.5,16.0,-0.0021015101949551497,0.0021244370024857562,-0.003909968648404502,0.0042835179014046754
+3.6256504768281257,0.27,0.5,30.0,-0.002015870106997474,0.001998591855385749,-0.003971737134739152,0.003793226510131275
+3.6256504768281257,0.33,0.5,41.0,-0.0016319537535483025,0.001410253703932015,-0.003139654145603247,0.0027978780161585035
+3.6256504768281257,0.39,0.5,45.0,-0.0014373389576215023,0.0013448639246472806,-0.002823681376769858,0.002681099243742783
+3.6256504768281257,0.45,0.5,53.0,-0.0011745321847787184,0.0011875856000572724,-0.0023469177433973355,0.002309788085767113
+3.6256504768281257,0.51,0.5,45.0,-0.0009843837383650149,0.0008339825148549106,-0.00200736989570754,0.0015832528208860833
+3.6256504768281257,0.57,0.5,43.0,-0.0012271610488439344,0.0012821523326217237,-0.0025082650534450986,0.0024731994980184756
+3.6256504768281257,0.63,0.5,47.0,-0.001143725721213554,0.001272085877761203,-0.002233326604766204,0.002641245952707736
+3.6256504768281257,0.69,0.5,55.0,-0.0009975069425506686,0.0009306236048126899,-0.0018543373954566483,0.001967155948877865
+3.6256504768281257,0.75,0.5,103.0,-0.0007914411876670165,0.0008175112384512469,-0.0015555708338283079,0.0015683935135256035
+3.6256504768281257,0.81,0.5,18.0,-0.0017357506948320425,0.001570954747756223,-0.0034714264988332756,0.003134927955429268
+4.606223395648538,0.15,0.5,5.0,-0.005040494965158815,0.003984484696905821,-0.01007532646872471,0.007019255527746115
+4.606223395648538,0.21,0.5,16.0,-0.0018694784714757954,0.002085125851356631,-0.003772490758355724,0.0040012350172018065
+4.606223395648538,0.27,0.5,29.0,-0.0017437571775344033,0.0018120257053578879,-0.003385665543315383,0.003620139822319834
+4.606223395648538,0.33,0.5,51.0,-0.001300417968682461,0.0012645791156156404,-0.002501758986638626,0.0024896618940826285
+4.606223395648538,0.39,0.5,47.0,-0.001226216997511144,0.0012103632045319854,-0.002448418829714219,0.0022669003403240516
+4.606223395648538,0.45,0.5,51.0,-0.001137514049560107,0.00111539507146812,-0.002304182068553032,0.0021911671230738345
+4.606223395648538,0.51,0.5,53.0,-0.0010131637422056722,0.0010298034283634896,-0.0020874356633677252,0.0019514566902586108
+4.606223395648538,0.57,0.5,33.0,-0.0016065176026548288,0.0018660932310343042,-0.0030003660824944726,0.00384521060992165
+4.606223395648538,0.63,0.5,58.0,-0.0014678904984293149,0.0014617510938659982,-0.00278907813390781,0.0029221699494753166
+4.606223395648538,0.69,0.5,73.0,-0.0011934741284397312,0.0011838767121358775,-0.002379533509318283,0.0022347385804924193
+4.606223395648538,0.75,0.5,72.0,-0.0011657614085068722,0.0011983082018521057,-0.0021924729777394857,0.002382379506146587
+4.606223395648538,0.81,0.5,10.0,-0.00297221682455392,0.003295794094147261,-0.005731574791311788,0.006656961780431694
+5.851996519306426,0.15,0.5,9.0,-0.0010155824840157,0.0009501642243956458,-0.0020110250675449775,0.0017611624924918237
+5.851996519306426,0.21,0.5,22.0,-0.002348530905059072,0.0023008871979131543,-0.004513101662855034,0.004556967246334088
+5.851996519306426,0.27,0.5,43.0,-0.001793497994778005,0.001810721979239543,-0.0037282486956234607,0.0032215119655538667
+5.851996519306426,0.33,0.5,55.0,-0.0013247831630424187,0.0013287455783147642,-0.0025657823203687996,0.002619201620140048
+5.851996519306426,0.39,0.5,49.0,-0.001266170365004605,0.0012170310554914024,-0.002515395197888145,0.0024108414577579305
+5.851996519306426,0.45,0.5,56.0,-0.0013963418518753517,0.0014093077827959791,-0.002861054461363994,0.002713415464803894
+5.851996519306426,0.51,0.5,46.0,-0.0018651257646994375,0.0018680191064598263,-0.0037803306999331524,0.0036328522985019664
+5.851996519306426,0.57,0.5,49.0,-0.0018504941931410236,0.0017878630170196934,-0.0036427298745594534,0.00344810427836921
+5.851996519306426,0.63,0.5,48.0,-0.0019404616117179715,0.001625039468996745,-0.003954352638985577,0.0031689800012073893
+5.851996519306426,0.69,0.5,76.0,-0.0016623568783086429,0.001756711954220255,-0.003516981596811426,0.0032168729805946454
+5.851996519306426,0.75,0.5,38.0,-0.002497311172492787,0.0026497985846707893,-0.005015132789145112,0.005042952286756067
+5.851996519306426,0.81,0.5,8.0,-0.0044337711660059065,0.004472144485499763,-0.008826084157619055,0.00841177861072576
+7.434694395049636,0.15,0.5,9.0,-0.0013369756796927318,0.0013967061081338248,-0.002599324452178827,0.0027905156797450215
+7.434694395049636,0.21,0.5,26.0,-0.0017817208454330659,0.0016315770753440584,-0.0034757742411116403,0.0030732059590795496
+7.434694395049636,0.27,0.5,48.0,-0.0018034652757678905,0.0018055674684663429,-0.003593680102026331,0.0033763404721698534
+7.434694395049636,0.33,0.5,56.0,-0.0016622711501353916,0.0017630070470876888,-0.003199411682759494,0.0035730571090488465
+7.434694395049636,0.39,0.5,62.0,-0.0013174006421125864,0.0011949582104596773,-0.002592033463294491,0.0024893776016312948
+7.434694395049636,0.45,0.5,61.0,-0.0017771637214134424,0.0017200415074490416,-0.003626774692936376,0.0033213860969038473
+7.434694395049636,0.51,0.5,53.0,-0.0018971039177758644,0.001853026990405056,-0.003897286388830539,0.003524241508174706
+7.434694395049636,0.57,0.5,36.0,-0.002919565776308753,0.002888726082023526,-0.006026936827148612,0.005584147819121307
+7.434694395049636,0.63,0.5,60.0,-0.0021255826236787137,0.002010309461285276,-0.004180362727831323,0.003908192152528606
+7.434694395049636,0.69,0.5,58.0,-0.0026872282850881235,0.002484069320545587,-0.0056318586228198825,0.00485604340800514
+7.434694395049636,0.75,0.5,24.0,-0.004496692054005055,0.003919285969184616,-0.009343350019150098,0.0073247743607901695
+9.445439785451788,0.15,0.5,9.0,-0.0012436150420560255,0.001431070234850315,-0.002420461362818113,0.002667884045990529
+9.445439785451788,0.21,0.5,27.0,-0.0016955124940431462,0.001889420546432057,-0.0033500227021244482,0.0036249962704300743
+9.445439785451788,0.27,0.5,57.0,-0.0015785969808168594,0.0014733123402307234,-0.0029917804781373347,0.0029251137094546253
+9.445439785451788,0.33,0.5,66.0,-0.0015981334543196523,0.0015997817309214449,-0.003192706072722524,0.0031166035225767704
+9.445439785451788,0.39,0.5,58.0,-0.0024327840915495994,0.002175557693415477,-0.004765653540628734,0.004416362351033448
+9.445439785451788,0.45,0.5,69.0,-0.002033069381220517,0.002009509787837112,-0.0039422768574123275,0.0038495944555750347
+9.445439785451788,0.51,0.5,45.0,-0.002977811588952349,0.002746288170011293,-0.006052319285780621,0.005332561397123113
+9.445439785451788,0.57,0.5,48.0,-0.0032864496931029378,0.002907639575091382,-0.0068143992258002,0.005400183847082059
+9.445439785451788,0.63,0.5,48.0,-0.005003828491725451,0.0038952451737784078,-0.009813734249185116,0.00757044989931955
+9.445439785451788,0.69,0.5,42.0,-0.005244275354090568,0.004976619575200202,-0.010415759378268892,0.009498479760919292
+9.445439785451788,0.75,0.5,17.0,-0.006730288624831094,0.0069107011378111,-0.01333464364219476,0.013467821166590982
+9.445439785451788,0.81,0.5,9.0,-0.009015773702208725,0.00783406727322252,-0.01867939919993127,0.014380301916567233
+9.445439785451788,0.87,0.5,5.0,-0.004678552913567778,0.0049761083150501335,-0.008393705520528403,0.009903277590454309
+11.999999999999996,0.15,0.5,6.0,-0.0017716113439707286,0.002719914399673118,-0.0033093216517176183,0.005856787132097048
+11.999999999999996,0.21,0.5,29.0,-0.0022311009342395405,0.0024347932014225763,-0.004362524828202662,0.004642393963217007
+11.999999999999996,0.27,0.5,57.0,-0.0022417735427679815,0.002414310202287673,-0.004222364115393287,0.004963446807318465
+11.999999999999996,0.33,0.5,68.0,-0.0018573171305766678,0.001972781821564478,-0.0038116324699943847,0.0037566191737316533
+11.999999999999996,0.39,0.5,76.0,-0.0022437308011793973,0.0022859926860244423,-0.004455728117749431,0.0042514740483213355
+11.999999999999996,0.45,0.5,67.0,-0.002553005384462906,0.0024558092436630513,-0.005084207897369087,0.004835639766694246
+11.999999999999996,0.51,0.5,49.0,-0.00384735572192515,0.0032996911535685355,-0.007918253972336269,0.006366550729204166
+11.999999999999996,0.57,0.5,44.0,-0.003516305436631942,0.003278698073825342,-0.007159532086077884,0.006229664429177133
+11.999999999999996,0.63,0.5,35.0,-0.007747412329234919,0.0067018676186782495,-0.016076052939532067,0.012381197957252468
+11.999999999999996,0.69,0.5,33.0,-0.009352773145550178,0.00857651373566413,-0.019488822139028666,0.016491525415576115
+11.999999999999996,0.75,0.5,15.0,-0.011178071247086403,0.014708185047566777,-0.020141878915260696,0.03143778308585784
+11.999999999999996,0.81,0.5,8.0,-0.0041855570881015,0.00699747784279368,-0.006913815494819091,0.016238632769244865
+11.999999999999996,0.87,0.5,8.0,-0.015059296498633572,0.011855155924305277,-0.029873749395486794,0.021601202555432866
+11.999999999999996,0.93,0.5,5.0,-0.004966006587513627,0.0067388072902384785,-0.009867791171291307,0.014098644798623949
+0.0999999999999931,0.21,1.0,12.0,-9.532189774014866e-05,9.332669036175209e-05,-0.00019486295419827857,0.00017063882152477518
+0.0999999999999931,0.27,1.0,20.0,-6.92888754671859e-05,6.152159203622726e-05,-0.00013911309076721653,0.00012058655511410555
+0.0999999999999931,0.33,1.0,33.0,-5.709400684855561e-05,4.776516913081223e-05,-0.00011994948459098641,8.648637363826675e-05
+0.0999999999999931,0.39,1.0,47.0,-2.7418363213701937e-05,2.5048777744443658e-05,-5.8364493073483667e-05,4.7275046207741345e-05
+0.0999999999999931,0.45,1.0,40.0,-5.834946048846429e-05,7.500524499908042e-05,-0.00010387459407497472,0.0001570655679312824
+0.0999999999999931,0.51,1.0,51.0,-6.474742522950933e-05,7.332629152343393e-05,-0.00011510546740784901,0.00016103755231521038
+0.0999999999999931,0.57,1.0,34.0,-7.732690258282765e-05,0.00010437147459292012,-0.00014859725152896716,0.0002113264533493232
+0.0999999999999931,0.63,1.0,51.0,-7.515921643763847e-05,8.28925018534699e-05,-0.00014190750786027245,0.00016589955163161143
+0.0999999999999931,0.69,1.0,55.0,-4.5081148708229315e-05,5.856441852505759e-05,-8.264402822280166e-05,0.00012473491535387065
+0.0999999999999931,0.75,1.0,88.0,-4.53342965236571e-05,5.0186216352660996e-05,-8.252547503195483e-05,0.00010550462421919743
+0.0999999999999931,0.81,1.0,62.0,-7.52568392172048e-05,6.936788204962625e-05,-0.00014616432694939766,0.00013924314238791024
+0.0999999999999931,0.87,1.0,5.0,-5.190015617095868e-06,3.2129045544504457e-06,-1.2503322773715908e-05,5.997229917165114e-06
+0.1270454343320614,0.21,1.0,12.0,-0.00013724398285884398,0.00011720757474878035,-0.0002764154077063786,0.00022708597852249792
+0.1270454343320614,0.27,1.0,22.0,-0.00010380993610484462,9.5857403820586e-05,-0.00020346085284514607,0.00018257973663020463
+0.1270454343320614,0.33,1.0,32.0,-8.267026962098887e-05,6.930893424682759e-05,-0.00017594487015294607,0.00012777535709492844
+0.1270454343320614,0.39,1.0,46.0,-3.863704018100751e-05,3.457473164125409e-05,-8.301190902855127e-05,6.264573431007735e-05
+0.1270454343320614,0.45,1.0,42.0,-6.0624061958027e-05,7.994539509026523e-05,-0.00011711353346722301,0.00015061123065225572
+0.1270454343320614,0.51,1.0,49.0,-7.008823625750626e-05,8.901642847955361e-05,-0.00013658448308793075,0.00018044185873084307
+0.1270454343320614,0.57,1.0,34.0,-8.900092120041934e-05,0.00011327157192106508,-0.00016020598358370235,0.0002376074525909023
+0.1270454343320614,0.63,1.0,51.0,-8.029744987758936e-05,8.809902295164109e-05,-0.00015574259134928074,0.00017811890569816244
+0.1270454343320614,0.69,1.0,55.0,-4.5177340641792346e-05,6.712903763854618e-05,-8.607020889846836e-05,0.00013544622177929234
+0.1270454343320614,0.75,1.0,88.0,-4.419358466615105e-05,5.296531400633942e-05,-8.726372532185334e-05,0.00010704349696348948
+0.1270454343320614,0.81,1.0,62.0,-7.411784402100415e-05,7.09392966722494e-05,-0.00014640264745606994,0.00013658854228774955
+0.1270454343320614,0.87,1.0,5.0,-5.981385514575169e-06,3.640006671146165e-06,-1.3470102459800518e-05,6.720148662209266e-06
+0.1614054238462154,0.21,1.0,12.0,-0.00021178195039646996,0.0001760925496415897,-0.00041720565267003583,0.00034369359530617713
+0.1614054238462154,0.27,1.0,22.0,-0.00016639445609621388,0.00016291686844364142,-0.00035132014117659886,0.0003031905068925892
+0.1614054238462154,0.33,1.0,32.0,-0.00012582679196256437,0.00010881834095241444,-0.00026245078049012745,0.00020517345626311806
+0.1614054238462154,0.39,1.0,46.0,-6.230115012766571e-05,5.280220800464935e-05,-0.00012662165777600765,9.900424213246161e-05
+0.1614054238462154,0.45,1.0,42.0,-8.186297486026215e-05,9.54271016269593e-05,-0.00015349411642838785,0.000204790581286716
+0.1614054238462154,0.51,1.0,49.0,-8.831789668872021e-05,0.00010588510448204912,-0.00017039876012119574,0.00022214910623433466
+0.1614054238462154,0.57,1.0,35.0,-0.00010373146382019322,0.0001351344331026262,-0.00020186164047293596,0.00027434099134778607
+0.1614054238462154,0.63,1.0,50.0,-9.370972976148458e-05,0.00010042559447530962,-0.00018193785409121685,0.00020951328557851007
+0.1614054238462154,0.69,1.0,55.0,-5.313619858356557e-05,7.329629121574059e-05,-9.743603958492859e-05,0.00015088919994798216
+0.1614054238462154,0.75,1.0,86.0,-4.978072601253295e-05,5.809039863675698e-05,-9.161966792650248e-05,0.00011664158854977791
+0.1614054238462154,0.81,1.0,64.0,-7.893809545517649e-05,7.126085581590011e-05,-0.00015717156566058774,0.00014269529123720783
+0.1614054238462154,0.87,1.0,5.0,-7.90846028366764e-06,6.624242825292736e-06,-2.190013973102003e-05,7.853379602796734e-06
+0.2050582217608949,0.21,1.0,12.0,-0.0003467189095009368,0.0003115953044732354,-0.0006990592234937695,0.0005856625499596488
+0.2050582217608949,0.27,1.0,23.0,-0.00029747116511047423,0.0002698115155599849,-0.0005657551914596686,0.0005336484566904169
+0.2050582217608949,0.33,1.0,31.0,-0.0002271189636833392,0.00019476730728518836,-0.00046638640919311576,0.0003578355419986527
+0.2050582217608949,0.39,1.0,46.0,-0.00010425263026823915,9.248770542074224e-05,-0.00021796657757611163,0.00017869279941681198
+0.2050582217608949,0.45,1.0,44.0,-0.0001256013349582331,0.00013116970592691037,-0.00022812360384945655,0.00027271777607709426
+0.2050582217608949,0.51,1.0,47.0,-0.0001371480361144355,0.0001509668561071634,-0.0002504258917805677,0.0003193858045702004
+0.2050582217608949,0.57,1.0,36.0,-0.00014113763821466777,0.00017154220714188156,-0.00025881770638251606,0.0003448771527316896
+0.2050582217608949,0.63,1.0,49.0,-0.00012079867231283898,0.00014072338549877105,-0.00023765039763297313,0.0002793506709381959
+0.2050582217608949,0.69,1.0,55.0,-6.468042619035155e-05,8.947776647229066e-05,-0.00012034281886783787,0.00019283404006464986
+0.2050582217608949,0.75,1.0,86.0,-6.041609512206222e-05,6.698699129536063e-05,-0.00010822781378125422,0.00013899956716744772
+0.2050582217608949,0.81,1.0,64.0,-9.031504208314368e-05,8.183615043965426e-05,-0.00017691342415879276,0.00015578319614023345
+0.2050582217608949,0.87,1.0,5.0,-2.0525807128102236e-05,1.4189770164385628e-05,-5.130738074585748e-05,2.052580712810228e-05
+0.2605171084697473,0.21,1.0,12.0,-0.0006100816743400128,0.0005243326468084073,-0.0012146617877171187,0.0009945709769332857
+0.2605171084697473,0.27,1.0,24.0,-0.00048455036494625647,0.0004553447401817036,-0.00095759191662112,0.0008700674376344068
+0.2605171084697473,0.33,1.0,31.0,-0.0003722499430568164,0.00032196875547547255,-0.0007748092246178208,0.0006188195382755571
+0.2605171084697473,0.39,1.0,46.0,-0.0001786590945806817,0.0001496664743725626,-0.00035050979525214326,0.00029800738462416475
+0.2605171084697473,0.45,1.0,43.0,-0.00018938632727260986,0.00018371210496627937,-0.00037497842546845993,0.000354679532580644
+0.2605171084697473,0.51,1.0,47.0,-0.00018002714658905042,0.00022098115376035292,-0.00035772541921152756,0.0004318918180130295
+0.2605171084697473,0.57,1.0,37.0,-0.00019404804046041204,0.00022984914910109563,-0.0003638867324595119,0.0004649629628638154
+0.2605171084697473,0.63,1.0,49.0,-0.0001630330368892187,0.00018137856428326033,-0.0003113855757786139,0.00036575587610782084
+0.2605171084697473,0.69,1.0,56.0,-8.711648930826299e-05,0.00011335407671719068,-0.0001502482313056619,0.00024343711330755954
+0.2605171084697473,0.75,1.0,83.0,-7.400660137701075e-05,8.708097362533523e-05,-0.00014431523329286168,0.00017385902067442314
+0.2605171084697473,0.81,1.0,64.0,-0.00010549759640386249,0.00010753787963997347,-0.00021316481143994655,0.00019968360045875274
+0.2605171084697473,0.87,1.0,6.0,-2.514643990625402e-05,2.1102688998223874e-05,-5.312781798609097e-05,3.745559955897756e-05
+0.3309750919646949,0.21,1.0,12.0,-0.0010620600163139737,0.0008304223463053797,-0.00212899538149889,0.001553192813241945
+0.3309750919646949,0.27,1.0,26.0,-0.0008071036354829737,0.0007515912991005046,-0.0016089562379147393,0.0014318481984456812
+0.3309750919646949,0.33,1.0,30.0,-0.0005561534122876171,0.00048352523166950037,-0.0011380493347787721,0.0009188467473876728
+0.3309750919646949,0.39,1.0,45.0,-0.0002795731435172772,0.00025034914991656,-0.0005700606702221963,0.00046561049727088954
+0.3309750919646949,0.45,1.0,43.0,-0.00028977785313396426,0.0002813582827962212,-0.0005999739186712682,0.0005273059757633181
+0.3309750919646949,0.51,1.0,47.0,-0.00026892293816495615,0.0003082536259517484,-0.0005258373407209294,0.0006019874814496511
+0.3309750919646949,0.57,1.0,37.0,-0.00025801060797938177,0.0003098161660064067,-0.0004807880645943657,0.0006284181374025504
+0.3309750919646949,0.63,1.0,49.0,-0.00022560379620415168,0.00022331733124569193,-0.0004143733399575322,0.0004795521482650289
+0.3309750919646949,0.69,1.0,56.0,-0.000105014402705601,0.0001433618531406133,-0.0001988674146351137,0.00029202991180642617
+0.3309750919646949,0.75,1.0,83.0,-8.97857520254973e-05,0.00010439631065782352,-0.00017184681075590026,0.00021311674547097982
+0.3309750919646949,0.81,1.0,64.0,-0.00012122709447713764,0.00011539257784563946,-0.00024813941100725485,0.0002247767714897864
+0.3309750919646949,0.87,1.0,6.0,-3.928152849376939e-05,3.378409870796739e-05,-8.326846235854705e-05,6.219603265920452e-05
+0.4204887431174611,0.21,1.0,12.0,-0.001740553154920676,0.0014285233203373696,-0.003852385427003046,0.00263913468559949
+0.4204887431174611,0.27,1.0,26.0,-0.0012149046738626644,0.0011266262226103953,-0.002432756846905888,0.0022006398683034646
+0.4204887431174611,0.33,1.0,29.0,-0.0008641050322232863,0.0007968314915997748,-0.0017940729845569317,0.0014879273006756337
+0.4204887431174611,0.39,1.0,47.0,-0.0003981758377874266,0.0003833017580236566,-0.0008203197086392986,0.0007307172459961452
+0.4204887431174611,0.45,1.0,45.0,-0.000457113341928883,0.0004083874230612182,-0.0009061641384502179,0.0007666277955464463
+0.4204887431174611,0.51,1.0,44.0,-0.0004245762923718016,0.00044019184654128,-0.000813564829586694,0.0009040796440364181
+0.4204887431174611,0.57,1.0,38.0,-0.0003586876948775565,0.00040936809080052006,-0.0006701704011751764,0.000855106942930486
+0.4204887431174611,0.63,1.0,47.0,-0.00029457289086689506,0.00032595888951436256,-0.0005698260917393103,0.000631361807358805
+0.4204887431174611,0.69,1.0,55.0,-0.00014363291851834744,0.00018007925064435885,-0.00026984275601910215,0.0003860033700673594
+0.4204887431174611,0.75,1.0,87.0,-0.0001075991489799167,0.000128571618637494,-0.0002138807800919349,0.0002465729882792364
+0.4204887431174611,0.81,1.0,61.0,-0.00014010695578644064,0.0001380852487088239,-0.0002757486702912577,0.00027524522549989065
+0.4204887431174611,0.87,1.0,6.0,-5.81950092224948e-05,5.2624674549935504e-05,-0.00013483219781705122,0.00011069876498306001
+0.5342117500109862,0.21,1.0,12.0,-0.0026055422826788298,0.002135783607641052,-0.005767274599114078,0.003782309197508411
+0.5342117500109862,0.27,1.0,27.0,-0.001718595227956741,0.0015685216550079444,-0.0033413195863662864,0.003131242727370773
+0.5342117500109862,0.33,1.0,29.0,-0.0013361983020222371,0.0011348035211931466,-0.0026365828407933314,0.0022631548348007223
+0.5342117500109862,0.39,1.0,47.0,-0.0005730830208242372,0.0005300724948085823,-0.0011704811655669986,0.0010326137650244888
+0.5342117500109862,0.45,1.0,46.0,-0.0006605276498922957,0.0006105736824885806,-0.0013511667815312431,0.0011455995231679792
+0.5342117500109862,0.51,1.0,43.0,-0.0006243188562013811,0.0006323042349872704,-0.001237857247325566,0.0013387890390742336
+0.5342117500109862,0.57,1.0,41.0,-0.0004953119702610469,0.0005508363004429255,-0.0009273804572370775,0.0011193550105204424
+0.5342117500109862,0.63,1.0,42.0,-0.0004407401158360184,0.0005018820298367106,-0.0008361725813617332,0.0010006087229719888
+0.5342117500109862,0.69,1.0,57.0,-0.00019946457943055847,0.00024069700462171374,-0.0003597853670419444,0.0005129331354234468
+0.5342117500109862,0.75,1.0,88.0,-0.0001491080044769676,0.00016082192998548528,-0.00028153750722573727,0.0003269646550639015
+0.5342117500109862,0.81,1.0,59.0,-0.00018202108618427734,0.0001790314311647283,-0.0003675461293712297,0.0003359017620638914
+0.5342117500109862,0.87,1.0,6.0,-0.00011254782844283269,0.00010442699199423684,-0.00021197074254018322,0.0002121784791017656
+0.6786916380543102,0.21,1.0,12.0,-0.0036582427060545225,0.0026617224155769128,-0.007324038043321715,0.0049984565304317385
+0.6786916380543102,0.27,1.0,28.0,-0.002162142103219344,0.0021955076356306854,-0.004490479905713659,0.004206991125184398
+0.6786916380543102,0.33,1.0,30.0,-0.0017336428813502932,0.0015872047630027253,-0.003516275885772651,0.0030126311060685996
+0.6786916380543102,0.39,1.0,45.0,-0.0008485051822951556,0.0007684917178688398,-0.001688186153015841,0.001445804383396813
+0.6786916380543102,0.45,1.0,51.0,-0.0008703639259863688,0.0007368514260575472,-0.001710100760904737,0.001471707669247435
+0.6786916380543102,0.51,1.0,41.0,-0.0008328075779807352,0.0008607655069781574,-0.0016600649047183696,0.0016399869524965798
+0.6786916380543102,0.57,1.0,38.0,-0.00070252496376992,0.0007549576654797686,-0.0013500751858328158,0.0015099672659866438
+0.6786916380543102,0.63,1.0,46.0,-0.0005573307775175767,0.0005797508479880354,-0.0011057542014953922,0.0011771057223478104
+0.6786916380543102,0.69,1.0,54.0,-0.00025156639592107576,0.0003034127037947615,-0.00047967886261064365,0.000607198508090335
+0.6786916380543102,0.75,1.0,87.0,-0.00017915526054297453,0.00020135677613067622,-0.00033916887731131695,0.000407258182298347
+0.6786916380543102,0.81,1.0,59.0,-0.00022275250456302092,0.00019788928110922677,-0.0004316730394926607,0.00037876887109905766
+0.6786916380543102,0.87,1.0,6.0,-0.0001580501957380761,0.00018602279082685633,-0.00031445040133132324,0.0003777927076062762
+0.8622467393414467,0.21,1.0,12.0,-0.004083323220830981,0.0031946665194773098,-0.008465958761618823,0.005880095089036148
+0.8622467393414467,0.27,1.0,29.0,-0.0027221113467352743,0.0024221536454777067,-0.005406594062480181,0.004848418185836737
+0.8622467393414467,0.33,1.0,29.0,-0.002322311073607492,0.0021455524492558836,-0.004683603149457182,0.003887755638832195
+0.8622467393414467,0.39,1.0,46.0,-0.0010617087468613741,0.0010163989601129973,-0.0022045924791282267,0.0019285473044388006
+0.8622467393414467,0.45,1.0,51.0,-0.0011708793033820138,0.0009656989892910697,-0.0023109949263032397,0.0019154431408570007
+0.8622467393414467,0.51,1.0,41.0,-0.0011197015706743247,0.001028355088427625,-0.002258275503387677,0.002004247603904146
+0.8622467393414467,0.57,1.0,38.0,-0.0009035133540522284,0.001003279204268974,-0.0017480952081133894,0.0019927995313514936
+0.8622467393414467,0.63,1.0,46.0,-0.0007106457308591012,0.0007326812350129613,-0.0013651110770846729,0.0014541182802901985
+0.8622467393414467,0.69,1.0,55.0,-0.0003221559750289475,0.00040193620401981686,-0.0006270401959806753,0.000770531930014402
+0.8622467393414467,0.75,1.0,85.0,-0.00023220058544754388,0.00024722662749897506,-0.0004647100750829489,0.0004877103115424073
+0.8622467393414467,0.81,1.0,59.0,-0.00027039538984340657,0.00024366156077880276,-0.000522346519432566,0.0004785729164284884
+0.8622467393414467,0.87,1.0,6.0,-0.00022688246672205223,0.00030243480639173076,-0.00042553782048565525,0.0005915242354310735
+1.0954451150103437,0.21,1.0,12.0,-0.00420797516647967,0.0031410815001152483,-0.00857668486444256,0.0060522629378570204
+1.0954451150103437,0.27,1.0,29.0,-0.00300108345644105,0.0026076889636286933,-0.005820069366429338,0.005189407559404885
+1.0954451150103437,0.33,1.0,34.0,-0.0024859763170904854,0.002119580929191155,-0.004931223377274454,0.004143639646855548
+1.0954451150103437,0.39,1.0,41.0,-0.0012995516770532025,0.0012457431390645597,-0.002566261141301594,0.0023553793060746174
+1.0954451150103437,0.45,1.0,50.0,-0.0014051441147653301,0.0012278868974840596,-0.0029446255316408925,0.0023368299541738097
+1.0954451150103437,0.51,1.0,44.0,-0.0014388531726837273,0.001376401164482336,-0.0029758229024366384,0.0026281679434287056
+1.0954451150103437,0.57,1.0,41.0,-0.001140535871796747,0.001217487290533945,-0.002197018504959989,0.0025042575153843734
+1.0954451150103437,0.63,1.0,48.0,-0.0009046329942353252,0.0009208017602673705,-0.001769240547063602,0.0018114647246876905
+1.0954451150103437,0.69,1.0,52.0,-0.0004531071581208623,0.0005452270749525865,-0.0008827577860858712,0.0010798360495034626
+1.0954451150103437,0.75,1.0,84.0,-0.0003282745155301287,0.0003505222236812626,-0.0006453460463202262,0.0006861804262959663
+1.0954451150103437,0.81,1.0,56.0,-0.0003412887457932178,0.00034281848768856336,-0.000712163997921237,0.000626307624405523
+1.0954451150103437,0.87,1.0,6.0,-0.0003081233557481468,0.00038127193099459395,-0.0005685323838334017,0.0008240269124282771
+1.3917130042341592,0.21,1.0,13.0,-0.0029786368036894065,0.003002813612983594,-0.006191050504870516,0.0055056567330549816
+1.3917130042341592,0.27,1.0,29.0,-0.0024192856768300787,0.0024006539510480446,-0.004746524042856524,0.004647084471466046
+1.3917130042341592,0.33,1.0,35.0,-0.0022682944431446947,0.0021143711555003364,-0.004709845807146585,0.0039124955523879585
+1.3917130042341592,0.39,1.0,44.0,-0.0014628471922266198,0.0013994660169576437,-0.0028885525935883616,0.0028383892805413577
+1.3917130042341592,0.45,1.0,50.0,-0.001776451339534948,0.0015076534828339508,-0.0034922229234774192,0.002929137731351111
+1.3917130042341592,0.51,1.0,42.0,-0.001765860543404577,0.0018519614444771914,-0.0036664723080485945,0.0036033759196564684
+1.3917130042341592,0.57,1.0,46.0,-0.0014794246839860618,0.0015417567609443679,-0.0028220881701050025,0.0032020002938418063
+1.3917130042341592,0.63,1.0,47.0,-0.0010905180372727333,0.0012268273775392358,-0.002198256650889337,0.002421155678686064
+1.3917130042341592,0.69,1.0,51.0,-0.0006891765042390718,0.000805425385334491,-0.001370068447592608,0.0016116505633683217
+1.3917130042341592,0.75,1.0,86.0,-0.0004292527323810025,0.0004641900483675913,-0.0008400377563708394,0.0008798931482724967
+1.3917130042341592,0.81,1.0,49.0,-0.000520196843711993,0.00045850215484506495,-0.0010562874903468301,0.0008482826158825543
+1.3917130042341592,0.87,1.0,6.0,-0.00031578611496502234,0.00034171400016513837,-0.0006128962073872852,0.0009091892805275778
+1.7681078308849765,0.21,1.0,12.0,-0.003123458336827649,0.002393847070558587,-0.006358246390498145,0.004436000037759037
+1.7681078308849765,0.27,1.0,29.0,-0.0020638287338240907,0.0019578243009534288,-0.004074455442804925,0.0036339685089992607
+1.7681078308849765,0.33,1.0,42.0,-0.0017397435878954745,0.001567069112502523,-0.0037656592005933026,0.0027130245459321403
+1.7681078308849765,0.39,1.0,37.0,-0.0017300234862739638,0.0017025879293297113,-0.0034089769347373728,0.003365752975526943
+1.7681078308849765,0.45,1.0,53.0,-0.0018275908816023532,0.0016457158641313427,-0.0034345349234125573,0.0032211893256859675
+1.7681078308849765,0.51,1.0,42.0,-0.001997957576990829,0.0018910600892694807,-0.003743211274439074,0.00393981549266931
+1.7681078308849765,0.57,1.0,50.0,-0.0016198990056498286,0.0018305545212127235,-0.0032447465901256907,0.0036976863495700885
+1.7681078308849765,0.63,1.0,49.0,-0.0010800743977273774,0.0012871041604619901,-0.002092973725602682,0.002637995572871457
+1.7681078308849765,0.69,1.0,48.0,-0.000798052235850215,0.0008903335388244768,-0.0015847113699746461,0.0017801712032454193
+1.7681078308849765,0.75,1.0,83.0,-0.0006141962321296232,0.0005417477522869326,-0.0011237321980620797,0.001101401516593541
+1.7681078308849765,0.81,1.0,45.0,-0.0006362448377752805,0.0005115740648080455,-0.0013108777611406438,0.0009746723429938139
+1.7681078308849765,0.87,1.0,6.0,-0.00037112056065036143,0.00044418730077559347,-0.0006582544646736756,0.0009610387868428574
+2.2463002732069106,0.21,1.0,12.0,-0.003468589851179911,0.002752895451599102,-0.006860593753489976,0.005184990018153911
+2.2463002732069106,0.27,1.0,33.0,-0.0016988946013772298,0.0015069407774826033,-0.003343387503372027,0.002957326781553409
+2.2463002732069106,0.33,1.0,41.0,-0.0017384667360076636,0.0015885820505273627,-0.0036322420519381035,0.0030660962394852337
+2.2463002732069106,0.39,1.0,40.0,-0.001507618270600381,0.0015629551350895383,-0.003124981472549116,0.002867506377566279
+2.2463002732069106,0.45,1.0,54.0,-0.0016249584179624493,0.0015632917271336476,-0.003338680528120563,0.002985422625202688
+2.2463002732069106,0.51,1.0,40.0,-0.0018229215356814438,0.0018834906255853587,-0.0036260847473119245,0.00370746658729219
+2.2463002732069106,0.57,1.0,56.0,-0.0014626447189820513,0.0015750649994922287,-0.002764562396933545,0.003298586987984433
+2.2463002732069106,0.63,1.0,44.0,-0.0012301370203689462,0.001416833012047332,-0.002297696713260505,0.0028989888658170976
+2.2463002732069106,0.69,1.0,62.0,-0.0007906821376219976,0.0008230032505974089,-0.0015483620910432885,0.0015398117265431445
+2.2463002732069106,0.75,1.0,66.0,-0.0007010853698790605,0.0006694631948148367,-0.0014505169447413886,0.0012696322321634917
+2.2463002732069106,0.81,1.0,41.0,-0.0008196975957498801,0.000622202615741641,-0.0016408182143128798,0.0011269286697183024
+2.2463002732069106,0.87,1.0,7.0,-0.0018137610283205858,0.0014966110751509928,-0.004978467522382593,0.0017572989273818805
+2.853821938497869,0.15,1.0,5.0,-0.003922340772214051,0.004613366644864713,-0.007189598153931655,0.008710131982052614
+2.853821938497869,0.21,1.0,12.0,-0.0027252102465360026,0.0024640477908147275,-0.0052576405241967425,0.004772406245248951
+2.853821938497869,0.27,1.0,32.0,-0.0017161275877470943,0.0016138260995170741,-0.0033796327710084533,0.003238906480849351
+2.853821938497869,0.33,1.0,45.0,-0.0013873610131639716,0.001253305255945929,-0.0027526939245262044,0.002423362415756605
+2.853821938497869,0.39,1.0,42.0,-0.0014244040420494986,0.001213697386101888,-0.0029813775989950423,0.0023226522182439296
+2.853821938497869,0.45,1.0,56.0,-0.0012528714667138037,0.0012091611443354265,-0.002464205637226642,0.0024350643740868793
+2.853821938497869,0.51,1.0,42.0,-0.0014883792100369472,0.0016716097536991987,-0.0029531001494987903,0.003258473264754143
+2.853821938497869,0.57,1.0,53.0,-0.0013175257716085131,0.0014132595102477972,-0.002578013784648502,0.002852708215752285
+2.853821938497869,0.63,1.0,50.0,-0.001208485160132144,0.001160548806005706,-0.0021631822236377815,0.0024564836883232163
+2.853821938497869,0.69,1.0,56.0,-0.0008320699092049553,0.0008658358171913507,-0.0017030160666011672,0.0016347697868737796
+2.853821938497869,0.75,1.0,67.0,-0.0007189625398708239,0.0006612614809472407,-0.0014483480889930292,0.001251339001457912
+2.853821938497869,0.81,1.0,31.0,-0.0008548469386758328,0.0006791666321808502,-0.0017325257776785092,0.0012815168108671242
+2.853821938497869,0.87,1.0,9.0,-0.00233007708048398,0.0015570922889878533,-0.005598783282816984,0.0020053657509071705
+3.6256504768281226,0.21,1.0,16.0,-0.0020494134802979545,0.001961207279377527,-0.003986994206028186,0.0037656677230432627
+3.6256504768281226,0.27,1.0,32.0,-0.0015407671203342408,0.0016081833660956141,-0.00296256699025312,0.0032680073716861305
+3.6256504768281226,0.33,1.0,52.0,-0.0011630629810879122,0.0012361245365295718,-0.0023951157500466066,0.002346071392562145
+3.6256504768281226,0.39,1.0,47.0,-0.0011071584028790045,0.0010579358337405996,-0.0021553442508090363,0.0022049226459353822
+3.6256504768281226,0.45,1.0,54.0,-0.00098003007388791,0.0009485860442023269,-0.0019675438740705833,0.0018974763230005028
+3.6256504768281226,0.51,1.0,49.0,-0.0010661455037327863,0.0011191237864557916,-0.0021670197921109754,0.002187734829570052
+3.6256504768281226,0.57,1.0,50.0,-0.001135232634554759,0.0012599790821200053,-0.002224402603692394,0.0025687529211062404
+3.6256504768281226,0.63,1.0,45.0,-0.0010761296329464744,0.0011931473924693418,-0.0021104306995939743,0.0023408658047659086
+3.6256504768281226,0.69,1.0,54.0,-0.0009437608654458992,0.000919992906493015,-0.0018417766584580845,0.0017739213827724705
+3.6256504768281226,0.75,1.0,63.0,-0.000809313396916487,0.0007972630879585928,-0.001634761696282539,0.0015847943036122773
+3.6256504768281226,0.81,1.0,24.0,-0.0011582155251980083,0.0010405434272904763,-0.0023846802828810165,0.0019741381450420507
+3.6256504768281226,0.87,1.0,10.0,-0.0029118411553082863,0.0016532559205133907,-0.006692632674196434,0.0028279113850326106
+4.6062233956485255,0.15,1.0,5.0,-0.002357142116110133,0.002123287815231901,-0.006653286390724422,0.0023755621809270497
+4.6062233956485255,0.21,1.0,16.0,-0.0016925699599184523,0.0016227878010815083,-0.003342723061625813,0.003260345095792936
+4.6062233956485255,0.27,1.0,36.0,-0.0016604845211193834,0.001513568934814151,-0.0031923619244272946,0.002884386526153265
+4.6062233956485255,0.33,1.0,50.0,-0.0011760989694141674,0.001162915494078568,-0.002333788327956967,0.0022604581455747267
+4.6062233956485255,0.39,1.0,51.0,-0.0010553654709791614,0.0010095195109719951,-0.0020821353915719486,0.0020417856449357072
+4.6062233956485255,0.45,1.0,54.0,-0.0008827549424588845,0.0009487914622452426,-0.0017456512007448831,0.0018373977687027707
+4.6062233956485255,0.51,1.0,55.0,-0.000835638286303874,0.0007817947106872132,-0.0016098319705964545,0.0015610842145767038
+4.6062233956485255,0.57,1.0,49.0,-0.0009154557475502273,0.0010681758962253834,-0.0017958972456541356,0.0020596258055822986
+4.6062233956485255,0.63,1.0,44.0,-0.0011759200224493469,0.001154110934998558,-0.0022593571615696253,0.002250928346806328
+4.6062233956485255,0.69,1.0,50.0,-0.0011034037808549577,0.0010069733336010782,-0.0022225057710413276,0.0019234073431831842
+4.6062233956485255,0.75,1.0,59.0,-0.0012965960759153041,0.001200629330999034,-0.002560764547943924,0.002371267903234663
+4.6062233956485255,0.81,1.0,20.0,-0.0019399064875210885,0.0018175821854800932,-0.003908454498462248,0.003583210280690423
+4.6062233956485255,0.87,1.0,10.0,-0.0038720745203714656,0.002701835999996228,-0.008203408993160664,0.005063305161063969
+5.851996519306434,0.15,1.0,5.0,-0.0026330108590214103,0.003002112210926679,-0.005006808315898258,0.00563512306994809
+5.851996519306434,0.21,1.0,18.0,-0.0013382800509372209,0.0011235913467535546,-0.0026832578327837214,0.002177753089602615
+5.851996519306434,0.27,1.0,40.0,-0.0016052730774679933,0.0015470835851882293,-0.003149138530948495,0.0030871053548919562
+5.851996519306434,0.33,1.0,52.0,-0.0013091586800923292,0.001323651493427142,-0.0025837700314097875,0.0025512625486230583
+5.851996519306434,0.39,1.0,58.0,-0.0011971604536816136,0.0011888882292807404,-0.0023252382112628526,0.00235767126449691
+5.851996519306434,0.45,1.0,51.0,-0.0013952113257026935,0.0013647603829685362,-0.0025728693640089013,0.0029677064909113936
+5.851996519306434,0.51,1.0,59.0,-0.0012505431221608244,0.0012711554914543036,-0.0025325191977857843,0.002324521548296964
+5.851996519306434,0.57,1.0,43.0,-0.0013060552530145758,0.001300114305697259,-0.0025991754209640588,0.0024733992820603623
+5.851996519306434,0.63,1.0,48.0,-0.0013819937175899677,0.0013917431384489491,-0.0028032472934141537,0.0027151763181996217
+5.851996519306434,0.69,1.0,48.0,-0.001873447351495627,0.0016374188761118028,-0.003974156235772746,0.0030803504276956327
+5.851996519306434,0.75,1.0,46.0,-0.00276697316780365,0.002562415553169827,-0.005413877373225642,0.004955523913636494
+5.851996519306434,0.81,1.0,18.0,-0.0033463793863184373,0.0035420903278626423,-0.006701136662366484,0.00695211819480929
+5.851996519306434,0.87,1.0,11.0,-0.004590365855754231,0.003938899164817483,-0.009438819752733673,0.007433559532683757
+7.434694395049639,0.21,1.0,23.0,-0.0011583829357622033,0.0012158012842299806,-0.002349278023504093,0.002327941171043454
+7.434694395049639,0.27,1.0,44.0,-0.001438235796449789,0.0013437147772237912,-0.0028667416560903755,0.0025904483428378054
+7.434694395049639,0.33,1.0,54.0,-0.0016960487967188054,0.0017580712250976093,-0.003282826537812139,0.0035687230343003046
+7.434694395049639,0.39,1.0,63.0,-0.0013926091047391164,0.0013771726273339405,-0.0026586005564148626,0.0027297524659675586
+7.434694395049639,0.45,1.0,54.0,-0.0015587107913389898,0.001612167922846185,-0.003222736122930857,0.0031202356047820966
+7.434694395049639,0.51,1.0,61.0,-0.0021514854156326605,0.0020416719520455913,-0.004327548313747258,0.003996534658911905
+7.434694395049639,0.57,1.0,45.0,-0.002625478671017188,0.0027024236513858934,-0.005216967044738685,0.005193304478007888
+7.434694395049639,0.63,1.0,44.0,-0.002476323373899042,0.0024195078364728432,-0.005017661340739389,0.004436273052681458
+7.434694395049639,0.69,1.0,36.0,-0.004353982459179576,0.0036157116924613454,-0.009160333086708139,0.00662302725179566
+7.434694395049639,0.75,1.0,35.0,-0.006456413989962589,0.006333538565238736,-0.012651766362867143,0.012277508120207751
+7.434694395049639,0.81,1.0,17.0,-0.005489490371490347,0.0037957738518258006,-0.012091112291556598,0.007028643800697522
+7.434694395049639,0.87,1.0,16.0,-0.0034750083233451735,0.0028925921053792373,-0.006801848009449462,0.005563748195372971
+7.434694395049639,0.93,1.0,6.0,-0.00697359083618832,0.003905832875131169,-0.013950960397867288,0.007302023187210478
+9.445439785451804,0.21,1.0,20.0,-0.0012489170555577925,0.0014726874345466897,-0.002336082813975873,0.0029387792926563634
+9.445439785451804,0.27,1.0,48.0,-0.0015813034471148896,0.0015922817078727303,-0.003281784413987961,0.002924666231124168
+9.445439785451804,0.33,1.0,47.0,-0.0021556723673655264,0.0020686217215388817,-0.004293585627090758,0.004021193371566263
+9.445439785451804,0.39,1.0,68.0,-0.0016867366937479737,0.0018216742900166332,-0.0033774447958435515,0.003473517467775984
+9.445439785451804,0.45,1.0,68.0,-0.002063268433101463,0.0020352573785865575,-0.00403220452830777,0.003979029714097702
+9.445439785451804,0.51,1.0,52.0,-0.0030859998316757438,0.0027527051039929495,-0.006405398228688432,0.0052510536150996365
+9.445439785451804,0.57,1.0,48.0,-0.003809860151056089,0.0036841366572621308,-0.00731489761782926,0.007352847927974894
+9.445439785451804,0.63,1.0,43.0,-0.004887011870519557,0.0038443809389583907,-0.009949814597715398,0.007264731512285518
+9.445439785451804,0.69,1.0,30.0,-0.007052679702908632,0.0056953838458058854,-0.014265939745626212,0.01067533558357969
+9.445439785451804,0.75,1.0,33.0,-0.008961649839539301,0.008931539949417014,-0.018203172160227824,0.016881029524737905
+9.445439785451804,0.81,1.0,15.0,-0.007138857979433023,0.009651581927714228,-0.013959163395983808,0.01941748506213012
+9.445439785451804,0.87,1.0,14.0,-0.004915843708456634,0.004039180601244143,-0.009996696579910614,0.0078961204069211
+9.445439785451804,0.93,1.0,11.0,-0.008268765034734978,0.006959071186026744,-0.016621622210319584,0.013416139376056223
+12.000000000000014,0.21,1.0,22.0,-0.0019156561489776733,0.0018277889269661639,-0.003727851621058305,0.0036789480555001436
+12.000000000000014,0.27,1.0,39.0,-0.0021015114525930346,0.0020766406538978138,-0.004340383209579359,0.00393978740396373
+12.000000000000014,0.33,1.0,65.0,-0.002022366632774088,0.002167914601575524,-0.004055307785014897,0.004114527145147244
+12.000000000000014,0.39,1.0,70.0,-0.0023431598660690997,0.002422975940377579,-0.004606538217905921,0.0047928772580882245
+12.000000000000014,0.45,1.0,57.0,-0.004105811439301713,0.0033809761135796413,-0.008557590653997436,0.006371636645290371
+12.000000000000014,0.51,1.0,66.0,-0.00514240686659719,0.004319037180371527,-0.010252478206658023,0.008297539277899791
+12.000000000000014,0.57,1.0,46.0,-0.0074507845366569864,0.006647187143986042,-0.015624945186677019,0.012508201430815732
+12.000000000000014,0.63,1.0,30.0,-0.011969996727496587,0.010151911988372727,-0.024327098496447968,0.019012754303795214
+12.000000000000014,0.69,1.0,31.0,-0.013647982725329267,0.011340488316909744,-0.027003907192114165,0.022492440044557634
+12.000000000000014,0.75,1.0,20.0,-0.02153711977423874,0.019462696740635332,-0.038899780684698175,0.03909701593361997
+12.000000000000014,0.81,1.0,13.0,-0.01805729211165119,0.02431239640405351,-0.032486119965747656,0.05240169981424689
+12.000000000000014,0.87,1.0,18.0,-0.005362494109219791,0.004632638693877102,-0.010043626467673523,0.009573629548756974
+12.000000000000014,0.93,1.0,17.0,-0.009134053086831483,0.009268722033053093,-0.018155173021460035,0.018099744229375617
+12.000000000000014,0.99,1.0,5.0,-0.02171574818067658,0.01527588321780109,-0.046511093071922534,0.027151967201808302
+0.0999999999999522,0.21,2.0,10.0,-8.180722939881674e-05,7.328662966093794e-05,-0.00017319583939183768,0.00013443336266188952
+0.0999999999999522,0.27,2.0,19.0,-4.3729152835852475e-05,3.4357818094335626e-05,-9.081850978201427e-05,6.516935502997439e-05
+0.0999999999999522,0.33,2.0,43.0,-3.010649571626698e-05,2.7275240015463744e-05,-5.856317651556138e-05,5.226538327685991e-05
+0.0999999999999522,0.39,2.0,48.0,-1.795324328076623e-05,1.6428756476032012e-05,-3.718129315653154e-05,3.120759617390029e-05
+0.0999999999999522,0.45,2.0,51.0,-1.5736731856022036e-05,1.3586142250985407e-05,-3.196161385568439e-05,2.5248345283296332e-05
+0.0999999999999522,0.51,2.0,45.0,-1.2046620972381052e-05,1.1011626872610323e-05,-2.40657629542512e-05,2.1982636278225028e-05
+0.0999999999999522,0.57,2.0,50.0,-2.023958245288672e-05,2.4827608090841903e-05,-3.595402417671537e-05,5.334759640226669e-05
+0.0999999999999522,0.63,2.0,41.0,-1.9343993502122782e-05,2.7632477520777957e-05,-3.363530106071664e-05,6.06847720906052e-05
+0.0999999999999522,0.69,2.0,54.0,-2.6647811823878173e-05,2.980594517109521e-05,-4.832240830776059e-05,6.242571310378609e-05
+0.0999999999999522,0.75,2.0,40.0,-3.266899968809017e-05,3.929151701195175e-05,-6.151224848721787e-05,8.01696171757357e-05
+0.0999999999999522,0.81,2.0,37.0,-3.7832245331663e-05,4.3335712826571395e-05,-7.345120553357726e-05,8.460185308444896e-05
+0.0999999999999522,0.87,2.0,28.0,-3.8924563818682736e-05,1.9789524401374402e-05,-8.27217344095803e-05,3.8510929937443804e-05
+0.0999999999999522,0.93,2.0,34.0,-1.1226917953393966e-06,7.155438206634169e-07,-2.380339550826865e-06,1.335181539452938e-06
+0.1270454343321273,0.21,2.0,10.0,-0.00012208579687920089,0.00010320952229972996,-0.00024162344447016721,0.00019850061007805443
+0.1270454343321273,0.27,2.0,19.0,-6.092856999419316e-05,5.011094260391077e-05,-0.00012510447316113277,9.339095799534071e-05
+0.1270454343321273,0.33,2.0,43.0,-3.9182694021926624e-05,3.961276514144994e-05,-8.382955014650763e-05,7.436177225737421e-05
+0.1270454343321273,0.39,2.0,48.0,-2.640878581198869e-05,2.3071555132020505e-05,-5.410088072178093e-05,4.383153901736497e-05
+0.1270454343321273,0.45,2.0,51.0,-2.0931603710507024e-05,1.889558017225488e-05,-4.425980759138772e-05,3.402269138943099e-05
+0.1270454343321273,0.51,2.0,45.0,-1.6218932405017995e-05,1.4335009046818225e-05,-3.365939499331862e-05,2.7348996039272213e-05
+0.1270454343321273,0.57,2.0,50.0,-1.953116114619952e-05,2.5966578504213963e-05,-3.7304314538562094e-05,5.101987959547707e-05
+0.1270454343321273,0.63,2.0,42.0,-1.9404132872209193e-05,2.721981137120693e-05,-3.4542101329822404e-05,5.885049382850557e-05
+0.1270454343321273,0.69,2.0,53.0,-2.6167915079817363e-05,3.2330560474181494e-05,-4.922718684045607e-05,6.481547720827883e-05
+0.1270454343321273,0.75,2.0,40.0,-3.226889157192679e-05,3.9657331411416244e-05,-6.071411134799507e-05,7.939649386011525e-05
+0.1270454343321273,0.81,2.0,37.0,-3.828842417373756e-05,4.204365869384392e-05,-7.602281475884032e-05,8.2735647739099e-05
+0.1270454343321273,0.87,2.0,28.0,-3.866812325948198e-05,1.986435696525625e-05,-8.086465882103222e-05,3.8560877990062107e-05
+0.1270454343321273,0.93,2.0,34.0,-1.4666415567597683e-06,1.0855490842067717e-06,-3.0756539398252785e-06,1.979530940644814e-06
+0.161405423846201,0.21,2.0,10.0,-0.00018307959808111932,0.00016794740524283467,-0.0003638485592216856,0.0003080082087091884
+0.161405423846201,0.27,2.0,19.0,-9.261816520395802e-05,7.81643441918025e-05,-0.00019082869163685966,0.00014593515295567724
+0.161405423846201,0.33,2.0,43.0,-6.713941197220107e-05,5.7455377831132325e-05,-0.00012740709185172266,0.00011588163082710831
+0.161405423846201,0.39,2.0,48.0,-3.948775994009261e-05,3.605064088843882e-05,-8.426909009969863e-05,6.81491107666854e-05
+0.161405423846201,0.45,2.0,52.0,-3.3183555862306634e-05,2.6922648191322212e-05,-6.557597951425388e-05,5.1709102105373794e-05
+0.161405423846201,0.51,2.0,45.0,-2.3991405615980996e-05,2.3983659640590953e-05,-5.0139305985438656e-05,4.15229039896755e-05
+0.161405423846201,0.57,2.0,49.0,-2.27735917462507e-05,2.5184899207177883e-05,-4.55762000583066e-05,5.007235579985866e-05
+0.161405423846201,0.63,2.0,42.0,-2.14204445371883e-05,2.970109537836183e-05,-4.017295132353193e-05,6.206753167775904e-05
+0.161405423846201,0.69,2.0,53.0,-2.8007907445277156e-05,3.191723310156638e-05,-5.116185513666943e-05,6.535014397494061e-05
+0.161405423846201,0.75,2.0,40.0,-3.341957787530816e-05,3.979994302111563e-05,-6.280026940965993e-05,7.913057414877549e-05
+0.161405423846201,0.81,2.0,38.0,-3.721913467199892e-05,4.155355721015695e-05,-7.286820386652888e-05,8.389426445438869e-05
+0.161405423846201,0.87,2.0,27.0,-3.753485793545295e-05,1.8555025696258578e-05,-8.151060435934557e-05,2.1778600051976732e-05
+0.161405423846201,0.93,2.0,34.0,-2.029763231570622e-06,1.4419536417368617e-06,-4.187228269480715e-06,2.903280434705879e-06
+0.2050582217609678,0.21,2.0,10.0,-0.0003110460133674249,0.00026873120708414624,-0.0006099276751240633,0.0005376439147072394
+0.2050582217609678,0.27,2.0,19.0,-0.00016041608801123245,0.00013783892219735393,-0.00033464001135285657,0.00024829547487265226
+0.2050582217609678,0.33,2.0,43.0,-0.00011290092879758227,0.00010682954693585232,-0.00022886193772003936,0.0001942155388099402
+0.2050582217609678,0.39,2.0,48.0,-6.831455596275642e-05,6.476138027684774e-05,-0.00014230693149626524,0.00012333608055376647
+0.2050582217609678,0.45,2.0,52.0,-5.303037826986509e-05,4.8090172120681445e-05,-0.00010952261057294961,8.836385583300679e-05
+0.2050582217609678,0.51,2.0,45.0,-4.2739116999351686e-05,3.967982048499499e-05,-9.035818085124238e-05,7.366091056657915e-05
+0.2050582217609678,0.57,2.0,50.0,-3.2487505347407796e-05,2.9787004966510047e-05,-6.359466728506e-05,5.713196619549208e-05
+0.2050582217609678,0.63,2.0,41.0,-2.7437780185538463e-05,3.519629393386096e-05,-5.465829229437714e-05,7.018914305775283e-05
+0.2050582217609678,0.69,2.0,53.0,-3.110805975311679e-05,3.6346521832105895e-05,-5.794268207694737e-05,7.469228519122859e-05
+0.2050582217609678,0.75,2.0,40.0,-3.766747547520529e-05,4.267470884175048e-05,-7.111365411778787e-05,9.007933056715347e-05
+0.2050582217609678,0.81,2.0,38.0,-4.110382636252534e-05,4.589168317861932e-05,-7.886424598619884e-05,8.880999115003489e-05
+0.2050582217609678,0.87,2.0,27.0,-3.906054965329579e-05,1.9694230111697815e-05,-9.01699230297326e-05,2.497845747184193e-05
+0.2050582217609678,0.93,2.0,34.0,-2.9159474178667483e-06,2.461965648062074e-06,-6.295858973861794e-06,4.601143069058904e-06
+0.2605171084697549,0.21,2.0,10.0,-0.0005306877422854707,0.0004758286022561786,-0.0010588195328592618,0.0008637169200878623
+0.2605171084697549,0.27,2.0,19.0,-0.0002666503747023683,0.0002283544729364482,-0.0005505138028724144,0.00042880968973868863
+0.2605171084697549,0.33,2.0,43.0,-0.00018546211919357567,0.00017750108185770377,-0.00039611707927680233,0.00033021034689802593
+0.2605171084697549,0.39,2.0,48.0,-0.00012626116584793504,0.0001067654624590811,-0.0002474238137354267,0.00021162871277732317
+0.2605171084697549,0.45,2.0,52.0,-9.070742606618099e-05,8.020736194260768e-05,-0.0001886749376950276,0.000147421617678822
+0.2605171084697549,0.51,2.0,45.0,-7.474807240002954e-05,6.767385406616351e-05,-0.00014728096232538763,0.0001316906525550975
+0.2605171084697549,0.57,2.0,50.0,-5.1238452581289624e-05,4.27716912418065e-05,-0.00010318477381915814,7.967819661096146e-05
+0.2605171084697549,0.63,2.0,41.0,-4.1352515393143195e-05,4.868114536495355e-05,-8.460802340067934e-05,9.563969990740633e-05
+0.2605171084697549,0.69,2.0,53.0,-4.139804188361869e-05,4.860699074923161e-05,-8.10222310655689e-05,9.885352457331968e-05
+0.2605171084697549,0.75,2.0,40.0,-4.832250916271421e-05,5.9647480687208773e-05,-9.295093153681993e-05,0.00012117948128158987
+0.2605171084697549,0.81,2.0,38.0,-5.608385767407276e-05,5.867773780872207e-05,-0.00010474904870790237,0.00011936901610725267
+0.2605171084697549,0.87,2.0,27.0,-5.337360522399971e-05,2.3762850419389725e-05,-0.00012587661584344728,3.529276372323739e-05
+0.2605171084697549,0.93,2.0,34.0,-7.103624975807008e-06,4.967067117817046e-06,-1.4675712061643682e-05,9.52489236821812e-06
+0.3309750919646429,0.21,2.0,10.0,-0.0008706670036480774,0.000779145416752242,-0.0017289964850558874,0.0014523352078674521
+0.3309750919646429,0.27,2.0,19.0,-0.0004356187577222336,0.0003739750742305885,-0.0008849749177910149,0.0007211102636598242
+0.3309750919646429,0.33,2.0,42.0,-0.00033131362390439306,0.00029019028110893036,-0.0006493856462336283,0.000577072559007543
+0.3309750919646429,0.39,2.0,49.0,-0.00020463953813456998,0.00018132241294131573,-0.0004091025679090696,0.0003630113199343131
+0.3309750919646429,0.45,2.0,52.0,-0.00015381762309513405,0.00012727741532162957,-0.00030768497017343114,0.000248094061185661
+0.3309750919646429,0.51,2.0,45.0,-0.00012640110753556506,0.00011100517017181036,-0.00025847432680090596,0.00021586593387834521
+0.3309750919646429,0.57,2.0,51.0,-7.984811283948241e-05,6.030254247266655e-05,-0.00016577043450354638,0.00011533918805666875
+0.3309750919646429,0.63,2.0,40.0,-5.8822608675530666e-05,6.674442229032575e-05,-0.00012384408467136385,0.00012749835807539505
+0.3309750919646429,0.69,2.0,53.0,-5.482952723789599e-05,6.0519968513237106e-05,-0.00010110148822506566,0.00012412212706383008
+0.3309750919646429,0.75,2.0,40.0,-5.83345654273061e-05,7.360464355542226e-05,-0.00011344990814064425,0.00014707876961173104
+0.3309750919646429,0.81,2.0,38.0,-6.22237384409891e-05,6.858327318370254e-05,-0.0001232861454598466,0.00013763753182660237
+0.3309750919646429,0.87,2.0,27.0,-5.401995331183979e-05,2.6660499641038398e-05,-0.00012718718859232802,4.3507149901133304e-05
+0.3309750919646429,0.93,2.0,34.0,-1.2640119072859209e-05,8.696606183032065e-06,-2.6059460169343405e-05,1.676896440725662e-05
+0.4204887431174827,0.21,2.0,10.0,-0.0013290034457410064,0.001200281691093119,-0.002670647942078104,0.0022797545236514605
+0.4204887431174827,0.27,2.0,19.0,-0.0006734921473261317,0.0006179666685390472,-0.0013677267954197304,0.0011466960013683338
+0.4204887431174827,0.33,2.0,41.0,-0.0005259956260840235,0.0004911190936076832,-0.0010592964743772822,0.0009389056975498788
+0.4204887431174827,0.39,2.0,50.0,-0.00033281516112547817,0.0002975963150754459,-0.0006914008282837875,0.000560006427573587
+0.4204887431174827,0.45,2.0,53.0,-0.0002303324667405288,0.00020666401071160352,-0.0005191747383684655,0.0003781301966877621
+0.4204887431174827,0.51,2.0,44.0,-0.00020809442454054863,0.0001871607167630241,-0.0004204604157354129,0.00036401237452817316
+0.4204887431174827,0.57,2.0,51.0,-0.0001269505531894189,9.578770762303373e-05,-0.0002518513851928286,0.0001851642728869143
+0.4204887431174827,0.63,2.0,41.0,-8.972134819311325e-05,8.484875009083605e-05,-0.00018338661622288463,0.00016674217371421743
+0.4204887431174827,0.69,2.0,52.0,-6.338818198353455e-05,6.927633603711665e-05,-0.00012328328130647772,0.00014195119079007197
+0.4204887431174827,0.75,2.0,41.0,-7.004651640348719e-05,7.907042710519426e-05,-0.00012799280632586757,0.00015774595883433874
+0.4204887431174827,0.81,2.0,37.0,-6.763477885496287e-05,8.084547384945063e-05,-0.0001324689928420166,0.0001581362050281345
+0.4204887431174827,0.87,2.0,27.0,-5.7404205379461106e-05,3.259463878920063e-05,-0.00013777945302803572,5.6196033410027974e-05
+0.4204887431174827,0.93,2.0,34.0,-1.8544775922013602e-05,1.27298568407424e-05,-4.186182027743165e-05,2.3267920242628626e-05
+0.5342117500109839,0.21,2.0,10.0,-0.001977926768655322,0.0018878335442464025,-0.004033040779990449,0.003504508747954593
+0.5342117500109839,0.27,2.0,19.0,-0.0010051571940138148,0.0009500361143346842,-0.0021298656780195627,0.0018089998096109151
+0.5342117500109839,0.33,2.0,41.0,-0.0007987122387466129,0.0007771960212667405,-0.0016483434850127583,0.0014923702272876028
+0.5342117500109839,0.39,2.0,51.0,-0.0005246274546166549,0.00046299618668885944,-0.0010642806460882121,0.0009207677195309209
+0.5342117500109839,0.45,2.0,52.0,-0.00038323225136858296,0.00030284564334818656,-0.0007658564476309492,0.0005718386400258943
+0.5342117500109839,0.51,2.0,44.0,-0.00032197842117465966,0.0003010362120472835,-0.0006754129806546136,0.0005595487828833233
+0.5342117500109839,0.57,2.0,53.0,-0.00018379401006809985,0.00014426564134552378,-0.0003837031371939675,0.0002758353969010012
+0.5342117500109839,0.63,2.0,39.0,-0.00014468351739231958,0.0001224632429371563,-0.0003091612865124739,0.00023538643884033942
+0.5342117500109839,0.69,2.0,52.0,-8.100062832885262e-05,9.017309622668247e-05,-0.0001542521760678777,0.00018314489672711159
+0.5342117500109839,0.75,2.0,42.0,-8.114606825973315e-05,9.717218674050827e-05,-0.00014776168783747933,0.00020229643086127605
+0.5342117500109839,0.81,2.0,36.0,-8.32376125448163e-05,9.330314896824282e-05,-0.00015886843268368142,0.00018615965135937226
+0.5342117500109839,0.87,2.0,27.0,-6.959263415335145e-05,4.146186219928631e-05,-0.00015886776427912554,7.45434773613093e-05
+0.5342117500109839,0.93,2.0,34.0,-2.9653510095633144e-05,1.9115117260135052e-05,-7.160714508124916e-05,3.4338429549180265e-05
+0.6786916380543009,0.21,2.0,10.0,-0.0028360024658033185,0.002528155866762546,-0.005731321104805302,0.004832533596662266
+0.6786916380543009,0.27,2.0,19.0,-0.0015186520643288147,0.001414143674404624,-0.002996186295864955,0.002698056985086989
+0.6786916380543009,0.33,2.0,42.0,-0.0012399422938731551,0.001060593789609209,-0.0023759868121246623,0.0022052098427184823
+0.6786916380543009,0.39,2.0,50.0,-0.0008289495329383042,0.0007348117509912069,-0.0016239344201015265,0.0014671699969805959
+0.6786916380543009,0.45,2.0,53.0,-0.0005617424898161988,0.00045111974288817295,-0.0011415896321151893,0.0008495577084571662
+0.6786916380543009,0.51,2.0,48.0,-0.0005115618184425829,0.0004446461218987901,-0.0009839914869319128,0.0008639601082557251
+0.6786916380543009,0.57,2.0,49.0,-0.0002471476013758061,0.00021854572181450308,-0.0005140971935202281,0.0004083741298730878
+0.6786916380543009,0.63,2.0,39.0,-0.00022234699368805244,0.0001863260731162701,-0.000473813384485303,0.0003417630572935218
+0.6786916380543009,0.69,2.0,52.0,-0.00010893269567824192,0.00011618581983145637,-0.00020622988973721307,0.00024152302591935143
+0.6786916380543009,0.75,2.0,42.0,-0.00011266346674532093,0.00012486548379984217,-0.00021849932126193224,0.0002462440041123217
+0.6786916380543009,0.81,2.0,34.0,-0.0001086308982983002,0.00011937483040337397,-0.00020425107861370327,0.00025418389476621625
+0.6786916380543009,0.87,2.0,28.0,-9.69905550111558e-05,6.76285481232949e-05,-0.000220270289730348,0.00012036022217022958
+0.6786916380543009,0.93,2.0,34.0,-5.7785076447948635e-05,3.380766466008646e-05,-0.0001332491701450113,5.9645941818877264e-05
+0.8622467393414361,0.21,2.0,10.0,-0.0038119830874508882,0.003195805904552235,-0.00739743564451641,0.006243024754175292
+0.8622467393414361,0.27,2.0,19.0,-0.0021359558880127195,0.0019073063374164534,-0.004289684824441804,0.003930528217006024
+0.8622467393414361,0.33,2.0,42.0,-0.0016951045629376145,0.0016225940050041624,-0.003338606435527165,0.0031149924917677667
+0.8622467393414361,0.39,2.0,50.0,-0.0011500043315299197,0.001136819969365401,-0.002410017468484127,0.002052127770937817
+0.8622467393414361,0.45,2.0,54.0,-0.0008156582718400809,0.0006967683999755717,-0.001664231159560806,0.0013108875603166244
+0.8622467393414361,0.51,2.0,47.0,-0.0007608950440704279,0.000732208440693339,-0.0015550723488433327,0.0013680699720240873
+0.8622467393414361,0.57,2.0,50.0,-0.00039508490058470406,0.00033369518992709283,-0.0007844589697533304,0.0006523522706742504
+0.8622467393414361,0.63,2.0,38.0,-0.00034915000639102763,0.00028699634326067274,-0.0007479437779947701,0.0005265693131536607
+0.8622467393414361,0.69,2.0,52.0,-0.0001501406788309344,0.0001664688471878893,-0.00030270503428770317,0.00033485359844171277
+0.8622467393414361,0.75,2.0,42.0,-0.00015874642423131238,0.0001755453324082499,-0.0003145313092746154,0.0003400335390486481
+0.8622467393414361,0.81,2.0,34.0,-0.0001673861714296745,0.00015596605581041622,-0.0003061590192223617,0.0003283988996893619
+0.8622467393414361,0.87,2.0,28.0,-0.00016042931527866298,0.00010780959637436303,-0.0003350030218404684,0.00019927616192385434
+0.8622467393414361,0.93,2.0,34.0,-0.00010553038849928273,6.153043688960285e-05,-0.0002449561713449976,0.00010906280708301058
+1.095445115010334,0.21,2.0,10.0,-0.004250930279979703,0.003834114794118532,-0.00831592647283688,0.007504985009703599
+1.095445115010334,0.27,2.0,20.0,-0.002644619431434012,0.002541065170367949,-0.005368963299637697,0.004710336096605481
+1.095445115010334,0.33,2.0,43.0,-0.002224900809569507,0.0021917115779825627,-0.004582262812262322,0.004301251985283723
+1.095445115010334,0.39,2.0,48.0,-0.0017583812998115049,0.0015632470184656373,-0.0034302514678663126,0.0031090738712186245
+1.095445115010334,0.45,2.0,54.0,-0.0011787131842955565,0.0010414867049224983,-0.002390355186476435,0.0019109811307458343
+1.095445115010334,0.51,2.0,49.0,-0.0010983408031407622,0.0010614018532931794,-0.0023224329518430086,0.0019867915087571366
+1.095445115010334,0.57,2.0,49.0,-0.0005816933856539353,0.0005510980679392849,-0.0012216048440674104,0.0010484944488871543
+1.095445115010334,0.63,2.0,37.0,-0.0005656592900956923,0.00044999661500927493,-0.0012340805852793576,0.0008107536556827243
+1.095445115010334,0.69,2.0,52.0,-0.000219002632065878,0.00023856792182494244,-0.00044406745020075556,0.00046879577193397474
+1.095445115010334,0.75,2.0,44.0,-0.0002378940634146279,0.00023409778618005574,-0.0004592558138322918,0.0004745735598385989
+1.095445115010334,0.81,2.0,32.0,-0.0002744501738962964,0.00023734143329016074,-0.0005494213325229684,0.00045700885282765443
+1.095445115010334,0.87,2.0,28.0,-0.0002504744371641687,0.0001781043544432696,-0.0005588567464594159,0.00032840782471248636
+1.095445115010334,0.93,2.0,34.0,-0.0001809152532191929,0.00010696433841241028,-0.0003992720051812472,0.00018745249808950967
+1.3917130042341654,0.21,2.0,10.0,-0.003722357235819709,0.0036935944859033845,-0.007307121495331578,0.0070748187088291985
+1.3917130042341654,0.27,2.0,20.0,-0.0029423453143661584,0.0026692209715811098,-0.006010973578652045,0.005078733671641334
+1.3917130042341654,0.33,2.0,43.0,-0.002741837659830815,0.002562274901188691,-0.0055231713378301244,0.005051245993302863
+1.3917130042341654,0.39,2.0,48.0,-0.0020915448420418615,0.0020946846304901773,-0.00405329805833069,0.003941326964094912
+1.3917130042341654,0.45,2.0,55.0,-0.0015871315967064875,0.0013947364144734754,-0.0033167815577962866,0.002542488103786879
+1.3917130042341654,0.51,2.0,50.0,-0.0016345522413857103,0.0014372697581580612,-0.002971336251925332,0.002748710659141835
+1.3917130042341654,0.57,2.0,50.0,-0.0008412504476776059,0.0007744537135820014,-0.0017929321328864496,0.0014348376400913846
+1.3917130042341654,0.63,2.0,34.0,-0.0008805865049042731,0.0007410402152348169,-0.0020171358659027,0.0012671587228754902
+1.3917130042341654,0.69,2.0,55.0,-0.00030487112098592626,0.0002860202047883305,-0.0005874156000183772,0.0005735307679187255
+1.3917130042341654,0.75,2.0,42.0,-0.00037819532634837726,0.00034665237098901514,-0.0007561985705941031,0.0006624580960841094
+1.3917130042341654,0.81,2.0,30.0,-0.00048197314201633713,0.0003385604001675821,-0.0010390414447613303,0.0006395622597476819
+1.3917130042341654,0.87,2.0,29.0,-0.0004241226786777124,0.0003271890308889708,-0.0009611249170936509,0.0005680123863358646
+1.3917130042341654,0.93,2.0,34.0,-0.00029414734683613574,0.0001817492907312606,-0.0006818388786087707,0.00031916736763355877
+1.7681078308850182,0.21,2.0,10.0,-0.0027564521705750094,0.0029116646893316833,-0.005210747911856225,0.005960627255486383
+1.7681078308850182,0.27,2.0,20.0,-0.002932813657643718,0.0035245300296612467,-0.005506772487792814,0.007175125451089875
+1.7681078308850182,0.33,2.0,43.0,-0.002440564161674311,0.0023274809879131587,-0.004930752220471237,0.0044884528281236265
+1.7681078308850182,0.39,2.0,48.0,-0.0022509369006654886,0.0021687984623407343,-0.004540257079182823,0.004230506013770502
+1.7681078308850182,0.45,2.0,57.0,-0.001798873670965611,0.0016907199639135152,-0.0037117086618137464,0.0030498034547334985
+1.7681078308850182,0.51,2.0,49.0,-0.001942449069836557,0.0018467401773312841,-0.003996740063733278,0.0034469023183887515
+1.7681078308850182,0.57,2.0,50.0,-0.001185435645768202,0.0009950645070494707,-0.0023808578968108154,0.0019635700002821267
+1.7681078308850182,0.63,2.0,37.0,-0.0011716742703023633,0.0009312452415688352,-0.0024058155983473243,0.0017174486337177513
+1.7681078308850182,0.69,2.0,51.0,-0.0004266185510671495,0.0003998826684768041,-0.0008284169016364492,0.0007983504897081556
+1.7681078308850182,0.75,2.0,40.0,-0.0006378318148863261,0.0005200824764403498,-0.0013634674426934404,0.000976525011100176
+1.7681078308850182,0.81,2.0,32.0,-0.000775089957503075,0.0005149612140742964,-0.0016803731059449826,0.0009324331443145718
+1.7681078308850182,0.87,2.0,29.0,-0.0007352905930903021,0.0005010610722482228,-0.001536475975487141,0.0009378064966945768
+1.7681078308850182,0.93,2.0,34.0,-0.0005085063074250877,0.0003174218783254023,-0.0010895578767504241,0.0005750483609901111
+2.2463002732069217,0.21,2.0,10.0,-0.0020676079095996148,0.002185465679296083,-0.003729887753291045,0.004593049453608575
+2.2463002732069217,0.27,2.0,20.0,-0.0024947317763911363,0.0030988097593993265,-0.0047725191925324165,0.006222071263824498
+2.2463002732069217,0.33,2.0,43.0,-0.0019709554648880316,0.0018152840692013926,-0.0038657651558768086,0.0035797777126747596
+2.2463002732069217,0.39,2.0,51.0,-0.002059273874971269,0.001975839765573368,-0.0041764660554744525,0.00388432797471198
+2.2463002732069217,0.45,2.0,57.0,-0.0018248762475804683,0.0016958688678522548,-0.003705386089133446,0.003232680489448039
+2.2463002732069217,0.51,2.0,47.0,-0.0022552799075564026,0.0020136780937073206,-0.004507365118017249,0.003902613360505021
+2.2463002732069217,0.57,2.0,51.0,-0.0013317527063325964,0.0011686607112064951,-0.0026524292709453044,0.002250768992145014
+2.2463002732069217,0.63,2.0,37.0,-0.0015011083975788723,0.0012452010649170123,-0.003122053143790468,0.002237496193551748
+2.2463002732069217,0.69,2.0,49.0,-0.000582869908126027,0.0005593669212559743,-0.0011431044109885254,0.0010995115149141676
+2.2463002732069217,0.75,2.0,40.0,-0.0009475056355423794,0.0007222819781920149,-0.0019935449104865276,0.001342208212973085
+2.2463002732069217,0.81,2.0,33.0,-0.0011268072942539151,0.000811600048914703,-0.0025143598306742736,0.0014623697190293235
+2.2463002732069217,0.87,2.0,28.0,-0.0011840706833224789,0.0008193629624330251,-0.0024455304485885643,0.001508540425230757
+2.2463002732069217,0.93,2.0,34.0,-0.0008241563426601274,0.0005232653304284075,-0.0016516776753077208,0.000981265072673715
+2.8538219384978727,0.21,2.0,10.0,-0.0018710373095565324,0.0021014812910130297,-0.003615974448265753,0.0040268898527833705
+2.8538219384978727,0.27,2.0,22.0,-0.0023750018471083876,0.0024026617845823574,-0.004581121842978104,0.004665380850853209
+2.8538219384978727,0.33,2.0,42.0,-0.0015091892750908732,0.0014819053910628574,-0.003060999065661995,0.0027664809898726565
+2.8538219384978727,0.39,2.0,49.0,-0.0017913243727296759,0.0016428668988796617,-0.0035174648868632535,0.0032877596893157047
+2.8538219384978727,0.45,2.0,62.0,-0.0014349184861390158,0.0014255706028955398,-0.0030400762608530536,0.0026877129630383362
+2.8538219384978727,0.51,2.0,47.0,-0.001899506295452662,0.0017858981056450382,-0.0038006865832818076,0.003439691306854522
+2.8538219384978727,0.57,2.0,48.0,-0.0013718532694939807,0.001201682035883645,-0.0026639240521512293,0.0023990854197881305
+2.8538219384978727,0.63,2.0,38.0,-0.0014565833101434988,0.001281224335309662,-0.00311921985785739,0.002318305673648796
+2.8538219384978727,0.69,2.0,49.0,-0.0007192013181071151,0.0006713352367262708,-0.0013869226619046223,0.0013541024852926574
+2.8538219384978727,0.75,2.0,38.0,-0.001266273228975432,0.0010152071079196864,-0.002819950495618341,0.001788262259673882
+2.8538219384978727,0.81,2.0,32.0,-0.0017234053687069676,0.0012626356730601335,-0.0034655609512860546,0.0022722260565345574
+2.8538219384978727,0.87,2.0,29.0,-0.0016534306606846285,0.0011975372818704185,-0.00353594743047694,0.0021196453007814014
+2.8538219384978727,0.93,2.0,34.0,-0.0010943983924849143,0.0008287199654205977,-0.0023231386789899938,0.0014876886297264028
+3.6256504768281177,0.21,2.0,10.0,-0.0016524896631180917,0.001738952551312478,-0.003202259248447756,0.0034769213078413193
+3.6256504768281177,0.27,2.0,21.0,-0.0019610132307710617,0.0021389479789223993,-0.003969369207929718,0.004107751414179846
+3.6256504768281177,0.33,2.0,49.0,-0.001110927374030954,0.0010829517764744485,-0.0022005755506857533,0.002053461211318086
+3.6256504768281177,0.39,2.0,47.0,-0.0014489379642368834,0.0014706399889806235,-0.0030002580984364305,0.0027803303008072343
+3.6256504768281177,0.45,2.0,60.0,-0.0010559706588798878,0.000943576193230894,-0.0021015456677906715,0.0019009841084881149
+3.6256504768281177,0.51,2.0,48.0,-0.0014521192987906333,0.0013968436925768264,-0.0029272696313724002,0.002679051881605561
+3.6256504768281177,0.57,2.0,49.0,-0.0009927345564813206,0.0009156423560379981,-0.0019924775066461338,0.0016926310238213047
+3.6256504768281177,0.63,2.0,37.0,-0.001270467371424201,0.001032878344192246,-0.0026230485220520325,0.0019380017819140513
+3.6256504768281177,0.69,2.0,47.0,-0.0006798402877328549,0.0006693021936115042,-0.001328089726896599,0.0013110188207882398
+3.6256504768281177,0.75,2.0,36.0,-0.0013268659075755189,0.0010368063380328237,-0.0027325947533855368,0.0019480434179206898
+3.6256504768281177,0.81,2.0,33.0,-0.0021750076573265843,0.0018274768641801324,-0.004551735873832535,0.003422860410068789
+3.6256504768281177,0.87,2.0,28.0,-0.0020246345127240086,0.0014215695042422084,-0.003947124763440197,0.0026495493867319015
+3.6256504768281177,0.93,2.0,35.0,-0.001328826597824548,0.0011358361637914323,-0.0028204098456759853,0.0021253851951570277
+4.606223395648549,0.21,2.0,10.0,-0.0017548723305957508,0.0016772031868907856,-0.00341530661646114,0.003162620371522984
+4.606223395648549,0.27,2.0,21.0,-0.0016905175908500066,0.001716470478952065,-0.003209625598315938,0.003449665015834076
+4.606223395648549,0.33,2.0,49.0,-0.0011801113405804794,0.0013319016939634342,-0.0024198962665265052,0.0024338727863271485
+4.606223395648549,0.39,2.0,52.0,-0.0011999306806639947,0.001255765856425674,-0.002342547141743029,0.0024040234379971814
+4.606223395648549,0.45,2.0,61.0,-0.0009832319215451865,0.0009771075063118885,-0.0019441432573260949,0.001878477774822581
+4.606223395648549,0.51,2.0,51.0,-0.0010818492760542799,0.0010321027246700152,-0.0020820689947611735,0.0020356495863504465
+4.606223395648549,0.57,2.0,47.0,-0.001099009584477831,0.0009487035076533699,-0.0023252522855606575,0.0017515184427970881
+4.606223395648549,0.63,2.0,37.0,-0.0014616861640205398,0.0011372434621632764,-0.003008784570853427,0.0021150493542351307
+4.606223395648549,0.69,2.0,43.0,-0.0008692434638939592,0.0008938928262712568,-0.001771107531341339,0.0016934139320403552
+4.606223395648549,0.75,2.0,34.0,-0.0017992400242051484,0.0013943371322674071,-0.003743805864358028,0.0026615318940850455
+4.606223395648549,0.81,2.0,31.0,-0.0028852334912239826,0.0024283717266868157,-0.006073653781705375,0.004564722014292013
+4.606223395648549,0.87,2.0,26.0,-0.0025657735457111554,0.00225055227266365,-0.005430444124504428,0.004078877502461564
+4.606223395648549,0.93,2.0,38.0,-0.0016308681737590089,0.0014450358337072752,-0.003235104738589357,0.002813480952988508
+5.851996519306407,0.21,2.0,9.0,-0.0025326377773520455,0.0024491565611978058,-0.004869478539021215,0.004769038494544765
+5.851996519306407,0.27,2.0,23.0,-0.0016435707433183255,0.0016820519990141658,-0.003430437855022838,0.003191016736943824
+5.851996519306407,0.33,2.0,50.0,-0.0014060884520124297,0.001408202965981057,-0.0028184645387042385,0.002734257746075937
+5.851996519306407,0.39,2.0,59.0,-0.0013474019263408348,0.0013584999184463012,-0.0025972273613241773,0.0027742944668853547
+5.851996519306407,0.45,2.0,57.0,-0.001270064347473461,0.001283598327318128,-0.0025176809343544974,0.0024730695597908183
+5.851996519306407,0.51,2.0,53.0,-0.0012328704315380382,0.0013134360021209472,-0.0024742229846548077,0.002429347946697159
+5.851996519306407,0.57,2.0,46.0,-0.0014598848287639805,0.001155892912679147,-0.0027454503220644905,0.0022774013953743423
+5.851996519306407,0.63,2.0,34.0,-0.0022333893071227687,0.00212118504757255,-0.004475885359746573,0.004182996993170347
+5.851996519306407,0.69,2.0,43.0,-0.001407599263402113,0.0013259938814521109,-0.0028161310533209895,0.0023766374137374952
+5.851996519306407,0.75,2.0,30.0,-0.002521365402843165,0.0021526885364389326,-0.005436687722915602,0.004061523494916289
+5.851996519306407,0.81,2.0,30.0,-0.003448975353589998,0.0034927956922850795,-0.007001267334749802,0.0065420091996427855
+5.851996519306407,0.87,2.0,22.0,-0.003355704755419592,0.003128223375881654,-0.006783364655795618,0.005624118051565234
+5.851996519306407,0.93,2.0,42.0,-0.0020437634975348424,0.001955385140217069,-0.004156944259099816,0.0038994202365897263
+7.434694395049636,0.21,2.0,10.0,-0.0017422916177316464,0.0014139711429455052,-0.0035769052979639426,0.0026692208779273622
+7.434694395049636,0.27,2.0,21.0,-0.0018462584080443435,0.001579050628190512,-0.0038926199359016816,0.002911098855030843
+7.434694395049636,0.33,2.0,50.0,-0.001189571807490766,0.0012021748485126153,-0.002384742153175363,0.002299342703229202
+7.434694395049636,0.39,2.0,51.0,-0.0015816057799966643,0.0016520543352243453,-0.0031451954059717566,0.003217871539930826
+7.434694395049636,0.45,2.0,63.0,-0.001393216480247115,0.0014071237232749277,-0.002655640860507914,0.002799786420535888
+7.434694395049636,0.51,2.0,56.0,-0.001435968461325133,0.0014416813658368287,-0.0028252510801573846,0.0028899534180024883
+7.434694395049636,0.57,2.0,47.0,-0.0016469546982810699,0.001497241202834768,-0.003197492862988718,0.0029242673251663734
+7.434694395049636,0.63,2.0,35.0,-0.0024622476632558334,0.0023809397918179063,-0.004897975585544801,0.004750970137210518
+7.434694395049636,0.69,2.0,37.0,-0.0023187611275048542,0.002203409022871806,-0.0045625525170097875,0.00436531813181617
+7.434694395049636,0.75,2.0,32.0,-0.004141705767003437,0.003529395723356232,-0.008973472356613695,0.006434430946511571
+7.434694395049636,0.81,2.0,28.0,-0.005778050810465495,0.005630710144824483,-0.011413103075648114,0.01096810435629288
+7.434694395049636,0.87,2.0,21.0,-0.0037326001918368936,0.0054237300999853575,-0.007337923865936953,0.010815910061397723
+7.434694395049636,0.93,2.0,37.0,-0.0024484796972826105,0.002154826846428319,-0.004680227180583764,0.004187224838614908
+7.434694395049636,0.99,2.0,12.0,-0.0030919863466354353,0.0027806666708689604,-0.006508192211807676,0.005144127150706691
+9.445439785451793,0.21,2.0,9.0,-0.0017274760760646666,0.002730243202209492,-0.0031087573855844387,0.006044042600031769
+9.445439785451793,0.27,2.0,20.0,-0.0020323329277045416,0.0015505803612830982,-0.00445514063235705,0.002841972997494057
+9.445439785451793,0.33,2.0,47.0,-0.0018410699139224703,0.001584107379613888,-0.0036767383074721304,0.003041527944434733
+9.445439785451793,0.39,2.0,55.0,-0.0019766705702255706,0.001993479431174865,-0.004046514686663545,0.003982976598604015
+9.445439785451793,0.45,2.0,64.0,-0.0019316021965713962,0.0019083279524122912,-0.0038541090053667917,0.003795283267908715
+9.445439785451793,0.51,2.0,49.0,-0.0022071760569802685,0.0022920222970328327,-0.004322807814147102,0.004600556079194165
+9.445439785451793,0.57,2.0,51.0,-0.002215588171515868,0.002071475816673492,-0.004377000999086294,0.004127254203997795
+9.445439785451793,0.63,2.0,36.0,-0.0034055807223232737,0.003233757748040196,-0.006442362800577788,0.0064429382603347326
+9.445439785451793,0.69,2.0,37.0,-0.003812782016726925,0.00357764178928631,-0.007514137426308185,0.006998119931846497
+9.445439785451793,0.75,2.0,31.0,-0.006775534830463015,0.005253414310690387,-0.014207355509555325,0.009653859130793831
+9.445439785451793,0.81,2.0,27.0,-0.007992005733110446,0.00789062553879955,-0.01629060549146655,0.015402707425342856
+9.445439785451793,0.87,2.0,23.0,-0.004220962187415791,0.00746611561790828,-0.007617654958155525,0.0172109168933066
+9.445439785451793,0.93,2.0,35.0,-0.0030258025746064295,0.00254243575257433,-0.005843566170012372,0.005006073503745441
+9.445439785451793,0.99,2.0,16.0,-0.0032713583804299486,0.003291659274327244,-0.00632903451730572,0.0066392927217122045
+11.999999999999998,0.27,2.0,24.0,-0.0023318970724105666,0.0021206555800763294,-0.004803772499689494,0.004060020041300723
+11.999999999999998,0.33,2.0,43.0,-0.0023059309252991453,0.0020421970919798325,-0.004503739340329581,0.004068056536016944
+11.999999999999998,0.39,2.0,56.0,-0.00266618642440418,0.0026293562667518543,-0.005425864095284182,0.00513047378263135
+11.999999999999998,0.45,2.0,67.0,-0.002517372880674503,0.0028598401011609553,-0.005196726015857295,0.005360501926720364
+11.999999999999998,0.51,2.0,57.0,-0.0029881330560212523,0.0027154266127558243,-0.005753920287516746,0.005594617175671063
+11.999999999999998,0.57,2.0,49.0,-0.003557841063238469,0.0033064658882446304,-0.007086391849630259,0.0064580342200285966
+11.999999999999998,0.63,2.0,40.0,-0.004901146747741736,0.004333765911218874,-0.009395906242308407,0.00857551190177355
+11.999999999999998,0.69,2.0,29.0,-0.007341384879156289,0.006782052460106533,-0.015009003603387864,0.01326272755495292
+11.999999999999998,0.75,2.0,27.0,-0.011173292280304099,0.009660393574142025,-0.02320275313072377,0.017611168714722455
+11.999999999999998,0.81,2.0,26.0,-0.013365277810197643,0.012498489666453793,-0.027621268933101267,0.02346863358143254
+11.999999999999998,0.87,2.0,18.0,-0.009703156102388906,0.015602006386883908,-0.017048474126025462,0.035325127749446385
+11.999999999999998,0.93,2.0,33.0,-0.0050096507002904645,0.005028365470470795,-0.010311617023007529,0.009664218051899817
+11.999999999999998,0.99,2.0,27.0,-0.005569283948331427,0.005309918988808098,-0.01086471282401124,0.010367749699106229
+0.1000000000001049,0.27,3.0,8.0,-2.2973680359750226e-05,2.7089002686983554e-05,-4.426534626481016e-05,5.379178252905292e-05
+0.1000000000001049,0.33,3.0,21.0,-1.6825816854807074e-05,1.3909604812801465e-05,-3.450159644193246e-05,2.643791854847344e-05
+0.1000000000001049,0.39,3.0,35.0,-1.0869585800801404e-05,1.0783418009982558e-05,-2.1107961986428243e-05,2.036912663737908e-05
+0.1000000000001049,0.45,3.0,40.0,-9.344555010024232e-06,8.294865656102929e-06,-1.9424961654591122e-05,1.5539709165578306e-05
+0.1000000000001049,0.51,3.0,54.0,-6.458088853653718e-06,5.99221704711544e-06,-1.2617412403632916e-05,1.1888874895695386e-05
+0.1000000000001049,0.57,3.0,53.0,-3.931850362718054e-06,3.880364120869959e-06,-7.646807839036618e-06,7.673768968893545e-06
+0.1000000000001049,0.63,3.0,49.0,-6.349421275539244e-06,1.0621567557556944e-05,-1.164082465441741e-05,2.3081555694490756e-05
+0.1000000000001049,0.69,3.0,55.0,-9.548287144051404e-06,1.2542533017588311e-05,-1.7296042060089608e-05,2.7551531323224263e-05
+0.1000000000001049,0.75,3.0,46.0,-9.93390485600527e-06,1.4246051263135469e-05,-1.771435204504617e-05,3.0183381214315993e-05
+0.1000000000001049,0.81,3.0,37.0,-1.4226294077724461e-05,1.960738455568227e-05,-2.6988065056160437e-05,3.970746377156518e-05
+0.1000000000001049,0.87,3.0,43.0,-1.795505045158087e-05,1.832874677742199e-05,-3.576556440434069e-05,3.627692603233057e-05
+0.1000000000001049,0.93,3.0,42.0,-3.9279811772543435e-07,3.2446936255514037e-07,-8.923121966660788e-07,5.844268586778126e-07
+0.1000000000001049,0.99,3.0,17.0,-2.719129900136178e-07,1.6072519294269615e-07,-5.781385631782634e-07,2.999263000711352e-07
+0.1270454343316895,0.27,3.0,8.0,-3.2564936573137304e-05,3.430654142182188e-05,-5.956801713642712e-05,7.063421127801158e-05
+0.1270454343316895,0.33,3.0,21.0,-2.291546366394254e-05,1.9514719323356864e-05,-4.831998418659395e-05,3.494028642279555e-05
+0.1270454343316895,0.39,3.0,35.0,-1.4182171557448802e-05,1.4091542841988699e-05,-2.7644850878808443e-05,2.7816592509199896e-05
+0.1270454343316895,0.45,3.0,40.0,-1.2760131147842531e-05,1.09082226750347e-05,-2.58206144631327e-05,2.0143044646354576e-05
+0.1270454343316895,0.51,3.0,53.0,-8.435579605153455e-06,7.926627332711396e-06,-1.6932537642771283e-05,1.5045116446443422e-05
+0.1270454343316895,0.57,3.0,54.0,-4.858082691315778e-06,4.797306457091943e-06,-9.762704103756069e-06,8.866359694708807e-06
+0.1270454343316895,0.63,3.0,49.0,-7.1046845973379135e-06,1.0522025066352477e-05,-1.2614625154548938e-05,2.2638238107673958e-05
+0.1270454343316895,0.69,3.0,55.0,-9.3456921478857e-06,1.2845322849286755e-05,-1.739491992817607e-05,2.6095162719468528e-05
+0.1270454343316895,0.75,3.0,46.0,-1.0019533854227508e-05,1.4123481263959159e-05,-1.7875411285919514e-05,3.0287347824832626e-05
+0.1270454343316895,0.81,3.0,37.0,-1.5274333779081017e-05,1.8929131137262573e-05,-2.8636416975874695e-05,3.8817725296993313e-05
+0.1270454343316895,0.87,3.0,43.0,-1.7886134469668034e-05,1.90750692378405e-05,-3.661506979509689e-05,3.8352392707137745e-05
+0.1270454343316895,0.93,3.0,42.0,-5.517646005714081e-07,4.527030251620849e-07,-1.215927703776088e-06,8.29434043099212e-07
+0.1270454343316895,0.99,3.0,17.0,-3.960824742683254e-07,2.2770289497405636e-07,-8.952433323651167e-07,3.8716097306306003e-07
+0.1614054238464021,0.27,3.0,8.0,-4.1328237844195925e-05,4.94034268087723e-05,-8.21439480726391e-05,9.601301640256577e-05
+0.1614054238464021,0.33,3.0,21.0,-3.524339308559759e-05,2.9267137718966185e-05,-7.293084664416261e-05,5.2632774995681576e-05
+0.1614054238464021,0.39,3.0,35.0,-2.1224816398244003e-05,2.027559879693592e-05,-4.307006187216982e-05,3.9539869637036416e-05
+0.1614054238464021,0.45,3.0,40.0,-1.8930014153845583e-05,1.5492058228495546e-05,-3.720305312719439e-05,3.0465913771131167e-05
+0.1614054238464021,0.51,3.0,53.0,-1.2063449010098706e-05,1.1122991353225914e-05,-2.3948153466090057e-05,2.1351750785753804e-05
+0.1614054238464021,0.57,3.0,55.0,-6.656097544033474e-06,6.654737811594905e-06,-1.3637779093219875e-05,1.2902736981702405e-05
+0.1614054238464021,0.63,3.0,48.0,-8.36982096021974e-06,1.1301467796938355e-05,-1.5451353014227613e-05,2.386983866094979e-05
+0.1614054238464021,0.69,3.0,55.0,-1.0108659264996307e-05,1.3001237905933338e-05,-1.8924137461171925e-05,2.760633391087655e-05
+0.1614054238464021,0.75,3.0,46.0,-1.0134548136501766e-05,1.4820299954107981e-05,-1.904324528714946e-05,3.067541389639525e-05
+0.1614054238464021,0.81,3.0,37.0,-1.540669964647618e-05,1.875588870094933e-05,-2.964738747868993e-05,3.9480305930618256e-05
+0.1614054238464021,0.87,3.0,43.0,-1.852251676950285e-05,1.8607322337757255e-05,-3.608845803382457e-05,3.685628957305222e-05
+0.1614054238464021,0.93,3.0,42.0,-7.399161109960901e-07,5.943650126052866e-07,-1.5364786318158578e-06,1.1167367840586918e-06
+0.1614054238464021,0.99,3.0,17.0,-4.705338040671308e-07,2.7242849019235275e-07,-1.019596678143699e-06,4.931220539252771e-07
+0.2050582217608584,0.27,3.0,8.0,-6.406357198952828e-05,7.063377754172595e-05,-0.00012072177177841993,0.00014445283244516805
+0.2050582217608584,0.33,3.0,21.0,-6.04538997200905e-05,4.7080114130798084e-05,-0.00011947727177417296,8.959188392524137e-05
+0.2050582217608584,0.39,3.0,35.0,-3.558629381539524e-05,3.475819855402918e-05,-7.062369281730082e-05,6.711379065180785e-05
+0.2050582217608584,0.45,3.0,40.0,-3.1678495360512684e-05,2.689572259304384e-05,-6.318266140400437e-05,5.2014067843966936e-05
+0.2050582217608584,0.51,3.0,53.0,-2.060437675595964e-05,1.7184465043754892e-05,-3.963081096981418e-05,3.460695913569062e-05
+0.2050582217608584,0.57,3.0,55.0,-1.1644863459835012e-05,1.0758176412183645e-05,-2.3135435173612512e-05,2.1427724242724156e-05
+0.2050582217608584,0.63,3.0,48.0,-1.2004393472536812e-05,1.3241138339190896e-05,-2.293344933243188e-05,2.7680151335473903e-05
+0.2050582217608584,0.69,3.0,55.0,-1.2472210725576552e-05,1.574480487731181e-05,-2.4232876353984942e-05,3.1908396914538786e-05
+0.2050582217608584,0.75,3.0,46.0,-1.1405565205176005e-05,1.7495505809676103e-05,-2.2387405654424413e-05,3.5053176820009695e-05
+0.2050582217608584,0.81,3.0,37.0,-1.7389005276603328e-05,2.1469851522701855e-05,-3.1849992960538384e-05,4.488593255507616e-05
+0.2050582217608584,0.87,3.0,43.0,-2.1118761472915694e-05,2.146115568115977e-05,-4.0230164971055025e-05,4.14716449166236e-05
+0.2050582217608584,0.93,3.0,42.0,-1.0597856235022408e-06,9.306387406991125e-07,-2.2161863771578637e-06,1.7665402716749906e-06
+0.2050582217608584,0.99,3.0,17.0,-6.304144121115409e-07,4.2331875492317214e-07,-1.373789414362267e-06,7.606869335986913e-07
+0.2605171084698608,0.27,3.0,8.0,-0.0001228772799475751,0.00012310586919662584,-0.00023397429335511588,0.00024496336741879895
+0.2605171084698608,0.33,3.0,21.0,-0.00010780823740430189,9.15724990577443e-05,-0.00022470959101793047,0.00016825559225298794
+0.2605171084698608,0.39,3.0,35.0,-6.763598420363512e-05,6.413012662698846e-05,-0.00013174638325828798,0.00012391284810978363
+0.2605171084698608,0.45,3.0,40.0,-5.813237499484397e-05,4.8824579909292264e-05,-0.0001208257257838798,9.210933593837359e-05
+0.2605171084698608,0.51,3.0,53.0,-3.682126621889727e-05,3.409788759471446e-05,-7.208176891468948e-05,6.35576938522344e-05
+0.2605171084698608,0.57,3.0,55.0,-2.037119466687104e-05,2.0337289405744868e-05,-4.200739945371517e-05,3.8782539126756756e-05
+0.2605171084698608,0.63,3.0,48.0,-2.1270777486785762e-05,2.0700123735012774e-05,-4.218410551743485e-05,4.263348950020382e-05
+0.2605171084698608,0.69,3.0,55.0,-1.8716299834415283e-05,2.3503125412602956e-05,-3.6783898706269956e-05,4.70648669472611e-05
+0.2605171084698608,0.75,3.0,46.0,-1.746100784206705e-05,2.3312826723438696e-05,-3.177635969590338e-05,5.037245724421581e-05
+0.2605171084698608,0.81,3.0,37.0,-2.4462843892220508e-05,3.1178827923480484e-05,-4.554864216258576e-05,6.211177007095976e-05
+0.2605171084698608,0.87,3.0,43.0,-2.9320840724427078e-05,2.9540779795509006e-05,-5.704137455435616e-05,5.824789715659104e-05
+0.2605171084698608,0.93,3.0,42.0,-1.893293442557634e-06,1.610244960956499e-06,-3.8431303970781e-06,3.0961469095253456e-06
+0.2605171084698608,0.99,3.0,17.0,-1.1932896509295878e-06,7.20988678899061e-07,-2.6329349932548307e-06,1.253266915063904e-06
+0.3309750919645017,0.27,3.0,8.0,-0.00021061160870647355,0.0001860404453095238,-0.00041621134153270456,0.00036602415719996784
+0.3309750919645017,0.33,3.0,21.0,-0.00018483008406171232,0.000150882089386211,-0.00037483814520427125,0.00029234139576831704
+0.3309750919645017,0.39,3.0,35.0,-0.00011371488181984103,0.00011224608017371605,-0.00023034079079249886,0.00020823159024463156
+0.3309750919645017,0.45,3.0,40.0,-0.00010489977402952475,8.771562792881724e-05,-0.00021237947717391606,0.00016868937795874907
+0.3309750919645017,0.51,3.0,54.0,-6.386500447785058e-05,5.597582405995969e-05,-0.00012281958751656435,0.00011215975546080643
+0.3309750919645017,0.57,3.0,55.0,-3.620204968977525e-05,3.489472626103502e-05,-7.279584058240686e-05,6.748968410880247e-05
+0.3309750919645017,0.63,3.0,47.0,-3.520996049740382e-05,3.441603358548227e-05,-7.22435790475579e-05,6.719497998452205e-05
+0.3309750919645017,0.69,3.0,55.0,-2.8444628158789077e-05,3.1308797699392834e-05,-5.462025599572672e-05,6.292847365928618e-05
+0.3309750919645017,0.75,3.0,46.0,-2.24014077201459e-05,3.142184765039703e-05,-4.1021101814608386e-05,6.607783259523916e-05
+0.3309750919645017,0.81,3.0,37.0,-3.124690256408857e-05,3.920705084620388e-05,-5.8872555926674413e-05,8.138969151235727e-05
+0.3309750919645017,0.87,3.0,43.0,-3.804023191380505e-05,3.607897937398858e-05,-7.065387633331354e-05,7.470153367834883e-05
+0.3309750919645017,0.93,3.0,42.0,-3.89772200094092e-06,3.161578392487887e-06,-8.508959205052249e-06,5.777679908617708e-06
+0.3309750919645017,0.99,3.0,17.0,-1.6503069792593406e-06,1.1035398906804279e-06,-3.7344057564965946e-06,1.9466404733542668e-06
+0.4204887431175216,0.27,3.0,8.0,-0.00038194546189153356,0.00028083354527611015,-0.0007500837872682701,0.0005426070628050515
+0.4204887431175216,0.33,3.0,22.0,-0.00027618313394294023,0.0002525829060861656,-0.0005736793771448881,0.00048367723552763186
+0.4204887431175216,0.39,3.0,34.0,-0.00019786758967399072,0.00017820402056151574,-0.00038288830513564907,0.00035302758875738373
+0.4204887431175216,0.45,3.0,40.0,-0.0001721037939796738,0.00015035128018334951,-0.0003689713877218063,0.0002700466287394445
+0.4204887431175216,0.51,3.0,55.0,-0.00010338842911161838,9.470725888451234e-05,-0.00020341722833348684,0.00018698007386583714
+0.4204887431175216,0.57,3.0,54.0,-6.279059414124449e-05,5.9560443625358696e-05,-0.0001251350933100213,0.00011477346240185925
+0.4204887431175216,0.63,3.0,46.0,-6.0901774960063086e-05,4.7898508868570966e-05,-0.00011924598638156783,9.62917122152522e-05
+0.4204887431175216,0.69,3.0,56.0,-4.086491628500337e-05,4.3997734690050034e-05,-8.053821080335109e-05,8.994355017627385e-05
+0.4204887431175216,0.75,3.0,46.0,-2.9116722501102925e-05,4.0865812559930985e-05,-5.312118776539405e-05,8.64737554777751e-05
+0.4204887431175216,0.81,3.0,37.0,-3.8335796905323704e-05,5.0934190207922686e-05,-7.663815436387538e-05,0.00010243124102820038
+0.4204887431175216,0.87,3.0,43.0,-4.5533711774171747e-05,4.381822098831732e-05,-8.619738028460744e-05,9.166283282307278e-05
+0.4204887431175216,0.93,3.0,42.0,-6.4813359980714765e-06,5.294391077746167e-06,-1.3778800760839182e-05,9.782311201468866e-06
+0.4204887431175216,0.99,3.0,17.0,-2.758019178974522e-06,1.8266674280179537e-06,-5.968550625350291e-06,3.2097557076361053e-06
+0.5342117500109141,0.27,3.0,8.0,-0.0006282062112615283,0.0005350891372146865,-0.0013219644957250636,0.000978812713949423
+0.5342117500109141,0.33,3.0,22.0,-0.0004962367586057506,0.0004196950924565212,-0.0009717708820362428,0.0008152318875657461
+0.5342117500109141,0.39,3.0,34.0,-0.0003325388137086336,0.00029413848086800226,-0.0006661013593291492,0.0005721692597052876
+0.5342117500109141,0.45,3.0,40.0,-0.0002831675127311597,0.0002384560750515717,-0.0005545628128867194,0.0004640441847384129
+0.5342117500109141,0.51,3.0,55.0,-0.00016447749000192576,0.00015831590305405375,-0.00033355930522071555,0.00030620058481739234
+0.5342117500109141,0.57,3.0,54.0,-0.00010707080959229426,9.386905139795227e-05,-0.00020718230688025285,0.0001833160288628686
+0.5342117500109141,0.63,3.0,46.0,-9.591640873059385e-05,7.787610612661106e-05,-0.00018777790342963533,0.0001486203937238493
+0.5342117500109141,0.69,3.0,56.0,-6.2725891382228e-05,6.0660105673543455e-05,-0.00012083661238776137,0.00011884946823959942
+0.5342117500109141,0.75,3.0,47.0,-3.787489333263431e-05,5.286026934592116e-05,-7.078127169332287e-05,0.00010454168332688928
+0.5342117500109141,0.81,3.0,35.0,-5.127610265180513e-05,6.48800962619971e-05,-9.635754639669823e-05,0.00013573732077187077
+0.5342117500109141,0.87,3.0,44.0,-5.443468137572637e-05,5.468791856765194e-05,-0.00011048311278981685,0.00010909650432149781
+0.5342117500109141,0.93,3.0,42.0,-9.892206489675232e-06,7.776743686190854e-06,-2.1398202585592413e-05,1.4524839238648882e-05
+0.5342117500109141,0.99,3.0,17.0,-5.0871058285605956e-06,2.873766570462506e-06,-1.2209376276512433e-05,4.959923360347835e-06
+0.6786916380543008,0.27,3.0,8.0,-0.0010060818562371426,0.0008635419613165158,-0.0020796480488921854,0.001589117871359097
+0.6786916380543008,0.33,3.0,22.0,-0.0007264737514713482,0.0006973436331479505,-0.0014601914456504573,0.0013387813539676133
+0.6786916380543008,0.39,3.0,34.0,-0.0005267446741612284,0.000494986353730104,-0.001085685138302088,0.0009166327245077061
+0.6786916380543008,0.45,3.0,40.0,-0.00042201036715451714,0.0004076564506716489,-0.0008845441380701546,0.0007608914540340269
+0.6786916380543008,0.51,3.0,55.0,-0.00026795799603104094,0.00024330334964536564,-0.0005316786249594768,0.0004762314152003412
+0.6786916380543008,0.57,3.0,55.0,-0.00016809586208217647,0.0001548352880150653,-0.0003260755625498239,0.0002999544169453885
+0.6786916380543008,0.63,3.0,44.0,-0.00015685681157465305,0.00012726259451679506,-0.0003256374203104924,0.0002449227879843111
+0.6786916380543008,0.69,3.0,57.0,-9.691410202091625e-05,8.111967949966488e-05,-0.000181550650317171,0.00016606110860291362
+0.6786916380543008,0.75,3.0,47.0,-5.0508874452377016e-05,6.683104238185326e-05,-9.380675857822083e-05,0.0001374525612018798
+0.6786916380543008,0.81,3.0,35.0,-6.540081027337845e-05,8.974047009589321e-05,-0.00012549525896115869,0.00017708991004660587
+0.6786916380543008,0.87,3.0,44.0,-6.972012680836462e-05,7.206506073621475e-05,-0.0001411691856453435,0.00014117334747991528
+0.6786916380543008,0.93,3.0,42.0,-1.6442670166222998e-05,1.1766342351243107e-05,-3.441564081101597e-05,2.2066794046443735e-05
+0.6786916380543008,0.99,3.0,17.0,-9.597050799092685e-06,5.641062944636462e-06,-2.21472093135493e-05,9.791230977944799e-06
+0.862246739341403,0.27,3.0,8.0,-0.0014428548518069517,0.0012764055813468955,-0.002952308421923927,0.002298013719359032
+0.862246739341403,0.33,3.0,22.0,-0.0011176114157450136,0.0011033666943245615,-0.0022053844099783697,0.0020349661782177774
+0.862246739341403,0.39,3.0,34.0,-0.0008395599643458585,0.0007240816994684166,-0.001711409319036401,0.0014436210662543685
+0.862246739341403,0.45,3.0,40.0,-0.0006940857959252347,0.000625889026248309,-0.0013507082623788237,0.0012499960637193134
+0.862246739341403,0.51,3.0,55.0,-0.00043683840988073514,0.000396609092629786,-0.0008752123834295929,0.0007503763006079664
+0.862246739341403,0.57,3.0,55.0,-0.00027424258618050616,0.00025073429415913175,-0.0005484915967940689,0.000491027982563667
+0.862246739341403,0.63,3.0,44.0,-0.00024167388111457453,0.00021576545117223342,-0.0005392404864542755,0.0003902197803041608
+0.862246739341403,0.69,3.0,57.0,-0.00014586770076693858,0.00012294078431582047,-0.0003028307707969693,0.00023825443789107683
+0.862246739341403,0.75,3.0,47.0,-7.285807158849576e-05,8.627838580453131e-05,-0.00013451309218502283,0.00018177278950494007
+0.862246739341403,0.81,3.0,35.0,-9.184075179351115e-05,0.00012205951679797824,-0.00017146700021282037,0.00023699018771576214
+0.862246739341403,0.87,3.0,44.0,-8.890234621353477e-05,9.25321766782288e-05,-0.000170816000335809,0.0001800973438376726
+0.862246739341403,0.93,3.0,42.0,-2.6385688380949877e-05,1.643686915947932e-05,-5.529181987372274e-05,3.0230218838544274e-05
+0.862246739341403,0.99,3.0,17.0,-1.4090958792611663e-05,8.494575855210617e-06,-3.0019256030666037e-05,1.5911905158478234e-05
+1.0954451150102975,0.27,3.0,8.0,-0.0019278997488018784,0.0016651730827805132,-0.004046841132971363,0.0030447560599762974
+1.0954451150102975,0.33,3.0,23.0,-0.001563941167841313,0.0014620960671345871,-0.003142097787831093,0.0029253459148096276
+1.0954451150102975,0.39,3.0,33.0,-0.00129657396107506,0.0012190395149821866,-0.002623409081972516,0.002322609440804587
+1.0954451150102975,0.45,3.0,40.0,-0.0010504081617411737,0.0009557266620117848,-0.002110169184063335,0.0019095683922472327
+1.0954451150102975,0.51,3.0,55.0,-0.0006617772920258598,0.0006352990224171977,-0.0013286188079426186,0.0012341035578863637
+1.0954451150102975,0.57,3.0,55.0,-0.0004361288767798145,0.00040290475920428466,-0.00085454032783606,0.0008056692899694369
+1.0954451150102975,0.63,3.0,44.0,-0.00042729132671180843,0.0003547077326411353,-0.0008871948639933826,0.0006768586060652467
+1.0954451150102975,0.69,3.0,58.0,-0.00023368410911285924,0.00020118775044664276,-0.0004639408729544366,0.0003847995346613321
+1.0954451150102975,0.75,3.0,47.0,-0.00010425646051552561,0.00012714971091604572,-0.0002111277013091816,0.0002467684504952613
+1.0954451150102975,0.81,3.0,33.0,-0.00014406250547779466,0.00017188159178630863,-0.0002676407502422417,0.0003664001610048201
+1.0954451150102975,0.87,3.0,45.0,-0.00011420351329298757,0.00011405126352909572,-0.00021276806154913488,0.0002358194788191082
+1.0954451150102975,0.93,3.0,42.0,-3.962916947906195e-05,2.7647701700927566e-05,-8.550691389291741e-05,5.0769649091951434e-05
+1.0954451150102975,0.99,3.0,17.0,-1.4615164233719568e-05,1.3277472691555401e-05,-3.06061358712287e-05,2.4939739721780177e-05
+1.3917130042342087,0.27,3.0,8.0,-0.0022307844554079245,0.0018344515345307122,-0.004462449531338566,0.0035226524986117086
+1.3917130042342087,0.33,3.0,23.0,-0.0018859990522611361,0.0019469179182298973,-0.003756796912201982,0.0038157725815664953
+1.3917130042342087,0.39,3.0,33.0,-0.0018731592275988813,0.0015782076480002163,-0.0035707869545017444,0.003202923549395921
+1.3917130042342087,0.45,3.0,40.0,-0.0014880807194111428,0.0013803289470139342,-0.0030401557751404324,0.0026426957626040984
+1.3917130042342087,0.51,3.0,54.0,-0.0010021498348866352,0.0009779348268181326,-0.002101836373097328,0.001785651968750306
+1.3917130042342087,0.57,3.0,53.0,-0.0007159176278932089,0.0006438216231321423,-0.0013640124793489943,0.0012949704331528878
+1.3917130042342087,0.63,3.0,47.0,-0.0006596475175172274,0.0005751291849624528,-0.0013668393042068458,0.0010488774456807837
+1.3917130042342087,0.69,3.0,57.0,-0.0003599360805782721,0.00030030798324663394,-0.0007611852069790928,0.0005725162291014137
+1.3917130042342087,0.75,3.0,46.0,-0.00016701656140520843,0.00017180525941954964,-0.0003210930307237331,0.00032912986983257023
+1.3917130042342087,0.81,3.0,34.0,-0.00017598816638100684,0.00021083326402571766,-0.0003501690608628863,0.0004214510872620851
+1.3917130042342087,0.87,3.0,43.0,-0.00012598565302750854,0.0001375737393636194,-0.00024006914112957686,0.00028009343655734776
+1.3917130042342087,0.93,3.0,45.0,-7.83603865939905e-05,5.764869270249392e-05,-0.00016253921971608697,0.00010366045869003612
+1.3917130042342087,0.99,3.0,17.0,-3.144661082634983e-05,2.619880165773343e-05,-6.299107923915003e-05,5.0041370878626425e-05
+1.768107830885,0.27,3.0,8.0,-0.002078969829527863,0.0017375293620688625,-0.004164647670922028,0.003241227891496834
+1.768107830885,0.33,3.0,23.0,-0.0020219702880653052,0.0021300956814373478,-0.003855565980406592,0.004194890423137712
+1.768107830885,0.39,3.0,31.0,-0.002049374511776193,0.001952650106040111,-0.004075276679535856,0.00359579042161754
+1.768107830885,0.45,3.0,41.0,-0.001958151479041185,0.0016549924596343825,-0.0037362399928984355,0.003345317546133378
+1.768107830885,0.51,3.0,56.0,-0.0012665261643322006,0.0012002122873025097,-0.0025685295204943594,0.0023685385599946864
+1.768107830885,0.57,3.0,52.0,-0.0009834917127954103,0.000950706084080799,-0.0019507110619245084,0.0018296341515860936
+1.768107830885,0.63,3.0,48.0,-0.000884206021279105,0.0008013195053320173,-0.001898830138289162,0.001542085040629152
+1.768107830885,0.69,3.0,55.0,-0.0005465621557365979,0.0004207129252576413,-0.0011337657123557797,0.0008239528715848261
+1.768107830885,0.75,3.0,44.0,-0.0002024971376735384,0.00020944211191126222,-0.000375607283849174,0.0004326366597089736
+1.768107830885,0.81,3.0,36.0,-0.000277409909043094,0.0002745538955964724,-0.0005512488599337425,0.0005236890350311955
+1.768107830885,0.87,3.0,42.0,-0.00016194481149673824,0.00015985700127314336,-0.00034274455352703033,0.0003034948227526702
+1.768107830885,0.93,3.0,47.0,-0.0001444436505812634,9.970391892762394e-05,-0.0003080378807088371,0.00018756939838296326
+1.768107830885,0.99,3.0,17.0,-6.274282034182221e-05,4.9694324410393e-05,-0.00012755279965012768,9.48075238772981e-05
+2.246300273206961,0.27,3.0,7.0,-0.0018216653383623656,0.0018150641601731255,-0.0038559438084172022,0.00337033084332507
+2.246300273206961,0.33,3.0,24.0,-0.0017966954636584726,0.0018728748054624518,-0.0033660460427740475,0.0041757159515354424
+2.246300273206961,0.39,3.0,31.0,-0.002000751002562409,0.001996131725020678,-0.004020237926446518,0.0037536426813664834
+2.246300273206961,0.45,3.0,39.0,-0.0021040203277283556,0.0019785416783477147,-0.004260013548449823,0.003720783179365456
+2.246300273206961,0.51,3.0,58.0,-0.0014833703897231293,0.0013980891386897554,-0.0029620162642925983,0.0027217701787694295
+2.246300273206961,0.57,3.0,52.0,-0.0012423132739439804,0.001198236166271414,-0.0024122518927510647,0.0023617245013035216
+2.246300273206961,0.63,3.0,48.0,-0.0011776284966708345,0.0010821331575314233,-0.0025090776083013604,0.0019684288198686313
+2.246300273206961,0.69,3.0,55.0,-0.0007686521253623095,0.0006006018268462571,-0.0015763997326112022,0.0011049415489310863
+2.246300273206961,0.75,3.0,42.0,-0.0002754602913965191,0.00027958448762219494,-0.0005386279834809317,0.000553214826458686
+2.246300273206961,0.81,3.0,37.0,-0.0004190001825316725,0.00037567051644472454,-0.0009064387359233046,0.00070102477772186
+2.246300273206961,0.87,3.0,42.0,-0.00031718821165414905,0.0002410859255757331,-0.0006722263250664917,0.00044208372539431706
+2.246300273206961,0.93,3.0,48.0,-0.0002361272445284878,0.00018883148962198936,-0.0004960367342800374,0.0003427322858114838
+2.246300273206961,0.99,3.0,17.0,-7.553957979692263e-05,7.777833767599872e-05,-0.0001492449324996472,0.000153259155006131
+2.853821938497916,0.27,3.0,7.0,-0.001708566259696636,0.0018278841119301493,-0.0032405279600583124,0.0036669916652095455
+2.853821938497916,0.33,3.0,24.0,-0.0014653078104934869,0.001698251576183839,-0.002791930301770165,0.0033792588486132734
+2.853821938497916,0.39,3.0,31.0,-0.0016377670416685946,0.001594073417407942,-0.0032515791847280645,0.0030902227615303107
+2.853821938497916,0.45,3.0,38.0,-0.001480933588710211,0.0013762901227080662,-0.0028514885912766475,0.0028023720352451037
+2.853821938497916,0.51,3.0,59.0,-0.0014654274055858718,0.001362859766840731,-0.002931177806357387,0.002671851941863068
+2.853821938497916,0.57,3.0,52.0,-0.0013199206482228476,0.0012630747658277446,-0.0025216055374163017,0.002602203802276673
+2.853821938497916,0.63,3.0,50.0,-0.001159420079371285,0.001125920575853557,-0.002362715568145985,0.002152454849781831
+2.853821938497916,0.69,3.0,51.0,-0.0009497487222027137,0.0007144295877077146,-0.0019882354731506164,0.001374807481125562
+2.853821938497916,0.75,3.0,44.0,-0.00041747687013121595,0.00044437298443623225,-0.0007908914281259205,0.0009181019067782351
+2.853821938497916,0.81,3.0,36.0,-0.0006234893911956236,0.000542165650081111,-0.001294516046083057,0.0010195898246063502
+2.853821938497916,0.87,3.0,39.0,-0.0005221688247260685,0.000400344827956166,-0.0011776457528260083,0.0007242877955837106
+2.853821938497916,0.93,3.0,49.0,-0.0004790811206245413,0.0003947863608725071,-0.0010136721587401711,0.0007285032287180056
+2.853821938497916,0.99,3.0,20.0,-0.00015224863993133954,0.00014268086887447466,-0.0003065233171324725,0.0002840203389812674
+3.6256504768281457,0.27,3.0,6.0,-0.0017599640184946532,0.00197825908746782,-0.0034101712930111514,0.003931397368360919
+3.6256504768281457,0.33,3.0,24.0,-0.0013760316186676813,0.0015568633043727448,-0.0025561875279126478,0.0031924392336062824
+3.6256504768281457,0.39,3.0,32.0,-0.001368975928169301,0.001185561615608544,-0.002584254090734626,0.002539970195578692
+3.6256504768281457,0.45,3.0,38.0,-0.0011373247278843553,0.0010923688253234181,-0.0022711538686767964,0.0020729888079901657
+3.6256504768281457,0.51,3.0,60.0,-0.0012091378816715774,0.0011424108310469907,-0.002359542200404529,0.002170867062660042
+3.6256504768281457,0.57,3.0,53.0,-0.0010573867539810163,0.001043898851452678,-0.0021244134580621073,0.002062374756157588
+3.6256504768281457,0.63,3.0,48.0,-0.0010846926419720293,0.0010447204677974304,-0.0021961485266045796,0.0020313105159144263
+3.6256504768281457,0.69,3.0,49.0,-0.0008922065992951892,0.0007712832490933431,-0.0017852300349824593,0.0014265088664836979
+3.6256504768281457,0.75,3.0,47.0,-0.0004905160494497841,0.0005585667235091236,-0.0009723264590249511,0.0010949256404026806
+3.6256504768281457,0.81,3.0,31.0,-0.0008460948215212907,0.0008525620558835663,-0.0017473350194201326,0.0015657258474457917
+3.6256504768281457,0.87,3.0,37.0,-0.0006657966707542515,0.0005837247304954441,-0.001387512334881927,0.0011233435764443026
+3.6256504768281457,0.93,3.0,53.0,-0.0007150040046367142,0.0006352398465712454,-0.0014701356190026608,0.0012354160259628291
+3.6256504768281457,0.99,3.0,22.0,-0.0005147085774865687,0.0003868000223294953,-0.0011210207464665055,0.0006923886861799337
+4.606223395648541,0.27,3.0,6.0,-0.0018006787635424881,0.002221135946655925,-0.0034442495620966747,0.004330274045620013
+4.606223395648541,0.33,3.0,23.0,-0.0012559228991782224,0.0013823406120914983,-0.0023761082691245994,0.0027906477095027346
+4.606223395648541,0.39,3.0,31.0,-0.0011269309715927246,0.0010470887154833035,-0.002275480892267873,0.002003547979233333
+4.606223395648541,0.45,3.0,45.0,-0.0009640935341945523,0.0009219135208694539,-0.0019933734032670752,0.0017889056689657688
+4.606223395648541,0.51,3.0,61.0,-0.0008398128422731632,0.0008554565849521597,-0.0016912057475179348,0.0015588964928814665
+4.606223395648541,0.57,3.0,58.0,-0.0007769631836870414,0.0007897944847352814,-0.001580607809976496,0.0015343719400446921
+4.606223395648541,0.63,3.0,50.0,-0.0009450095888793725,0.0009159146856705485,-0.0018117738779119285,0.0018656866087791266
+4.606223395648541,0.69,3.0,40.0,-0.0008005388491194064,0.0007311562320556287,-0.0016636474969621644,0.001420058376960811
+4.606223395648541,0.75,3.0,46.0,-0.0006054992325836587,0.0006705779818501095,-0.0012934800318193,0.0012368697754161202
+4.606223395648541,0.81,3.0,28.0,-0.001086966839107152,0.0010363685350082586,-0.0020519701653507606,0.00208096907858532
+4.606223395648541,0.87,3.0,32.0,-0.0014243381548469552,0.0013757317269873642,-0.003002137453113514,0.0025141298555183197
+4.606223395648541,0.93,3.0,49.0,-0.001056148039507978,0.0009334876705626538,-0.0021262438501744503,0.0019281666686858472
+4.606223395648541,0.99,3.0,31.0,-0.0005805004530321885,0.0005202031395310775,-0.0011737344328842402,0.0009909743288867086
+5.851996519306448,0.27,3.0,7.0,-0.001899309528711836,0.001776885004965852,-0.003780739023795941,0.003484004171549339
+5.851996519306448,0.33,3.0,19.0,-0.0010340956061193716,0.0011086193279489418,-0.0020518995218035477,0.0021635521472002863
+5.851996519306448,0.39,3.0,36.0,-0.001026835486660415,0.0010993563380910358,-0.0020506346924322404,0.0020669430600099336
+5.851996519306448,0.45,3.0,45.0,-0.0009101314928189104,0.0008597245899224559,-0.0018752066208068238,0.0016954590413716592
+5.851996519306448,0.51,3.0,69.0,-0.0007328677840154888,0.000755985260214716,-0.0015006509197159049,0.0014815725785261543
+5.851996519306448,0.57,3.0,63.0,-0.0009350971780490306,0.0009458880995272151,-0.0018599946985311635,0.0018919586403703043
+5.851996519306448,0.63,3.0,51.0,-0.0011126939030098907,0.000971146586023917,-0.0021091122806172207,0.0019183445165456392
+5.851996519306448,0.69,3.0,39.0,-0.001120297250008915,0.0010396891991265628,-0.0022716465638285524,0.0019795436557573844
+5.851996519306448,0.75,3.0,32.0,-0.0007247424683664763,0.0008426855983348366,-0.0013592925761448024,0.0017978872285443702
+5.851996519306448,0.81,3.0,27.0,-0.0020103148139587424,0.0016151780205339622,-0.004254893697351335,0.002952912379901546
+5.851996519306448,0.87,3.0,25.0,-0.003432071101384164,0.003308136395085502,-0.00659097290189513,0.0066616781944952965
+5.851996519306448,0.93,3.0,50.0,-0.0014023266132305978,0.0014968566274941317,-0.00281863631061146,0.002893461164557368
+5.851996519306448,0.99,3.0,37.0,-0.0010578882829834645,0.0009298559263757612,-0.0022590273118777543,0.0017295752404434491
+7.434694395049622,0.27,3.0,6.0,-0.0020293111493993043,0.00200164119080846,-0.004594820027628492,0.0035677531486678995
+7.434694395049622,0.33,3.0,16.0,-0.0010531065567722867,0.001084709709203002,-0.0019984839833431397,0.002139281129279587
+7.434694395049622,0.39,3.0,36.0,-0.0008408202368040814,0.0009871960707197014,-0.0017156769484904773,0.001949949938332423
+7.434694395049622,0.45,3.0,51.0,-0.000915935538682831,0.0009333805387974339,-0.0018016927223244127,0.0018314040137017995
+7.434694395049622,0.51,3.0,71.0,-0.0009537400483113446,0.0009785350387951223,-0.0018228473754633347,0.001937492925514855
+7.434694395049622,0.57,3.0,64.0,-0.0010732445038783957,0.001131110190965714,-0.0021589228419056413,0.00217540351182954
+7.434694395049622,0.63,3.0,53.0,-0.0012019138784231601,0.0010797792215846644,-0.002152374521755083,0.002235608753689509
+7.434694395049622,0.69,3.0,38.0,-0.0014114060100060848,0.0012736623316840496,-0.0029974832933093148,0.0024045313259979805
+7.434694395049622,0.75,3.0,30.0,-0.0009879987152134951,0.00114217481964334,-0.001905179010870482,0.002193355502117846
+7.434694395049622,0.81,3.0,23.0,-0.0031416014950900557,0.002071441898424287,-0.007334526540970917,0.0036608801783124144
+7.434694395049622,0.87,3.0,21.0,-0.006002632394462537,0.006113127042725382,-0.01240395134423472,0.010855903000397396
+7.434694395049622,0.93,3.0,44.0,-0.001789592811756613,0.002164036341748078,-0.003478048099258258,0.004315351662614705
+7.434694395049622,0.99,3.0,47.0,-0.0017383045068435552,0.0014032294759450102,-0.0034902500559544003,0.0027200741332510034
+9.445439785451796,0.33,3.0,21.0,-0.0017348916067165122,0.0011916343363365728,-0.003528837195625352,0.0022346760857378327
+9.445439785451796,0.39,3.0,35.0,-0.0014068023977614806,0.0013351919813532904,-0.0027600990099221007,0.0026060308522730105
+9.445439785451796,0.45,3.0,47.0,-0.0012801964448349186,0.0014640222912607479,-0.0025173845681579245,0.0027758884939983416
+9.445439785451796,0.51,3.0,69.0,-0.0013430474798375692,0.0012860900568114815,-0.002644725976709091,0.0026824256705866778
+9.445439785451796,0.57,3.0,63.0,-0.0013857460312217851,0.0014496718648382085,-0.002798143689864514,0.0028186785015865542
+9.445439785451796,0.63,3.0,58.0,-0.0013035129800027239,0.0012880569944944372,-0.002770121533877304,0.0023284340650324463
+9.445439785451796,0.69,3.0,39.0,-0.001882277078179238,0.0017573030413467066,-0.003647527418980282,0.003455475610815496
+9.445439785451796,0.75,3.0,30.0,-0.0017298974469202822,0.001658456842370959,-0.003512232368858836,0.0031514308847485394
+9.445439785451796,0.81,3.0,23.0,-0.004653582222284905,0.0027592930060096332,-0.010984991720715431,0.004689500084462536
+9.445439785451796,0.87,3.0,21.0,-0.009683311905476753,0.009132475083916928,-0.01922633953899343,0.017787388613427494
+9.445439785451796,0.93,3.0,41.0,-0.0021714243967562944,0.003422558254865944,-0.004050912891687705,0.007383946901335997
+9.445439785451796,0.99,3.0,50.0,-0.0019110298473476726,0.0018881104264499749,-0.004130345729781477,0.003452059438210881
+11.999999999999996,0.33,3.0,15.0,-0.0021847921516526393,0.0023379339690507727,-0.004390556854097376,0.004259871029930712
+11.999999999999996,0.39,3.0,22.0,-0.002015404096951997,0.002000642656637259,-0.0041507394905707165,0.0037445849984451933
+11.999999999999996,0.45,3.0,56.0,-0.001544819538603517,0.0015934918779853969,-0.0031964805237037915,0.0029608432983288194
+11.999999999999996,0.51,3.0,50.0,-0.0020882645932303223,0.001973271951004862,-0.004091357785906672,0.003860576726938648
+11.999999999999996,0.57,3.0,73.0,-0.0016952062265095786,0.0017243092163557493,-0.003458893871793834,0.0033626345199526623
+11.999999999999996,0.63,3.0,67.0,-0.0018588486628730832,0.001723379305044924,-0.0035702691654413855,0.00330110383005343
+11.999999999999996,0.69,3.0,45.0,-0.002654151562662259,0.002265679059565221,-0.0051994091249972845,0.004481582076176137
+11.999999999999996,0.75,3.0,31.0,-0.0026748013911678677,0.0026751384003835133,-0.0051363273067093155,0.0053429746298067566
+11.999999999999996,0.81,3.0,21.0,-0.002033708776398645,0.0019468609775796734,-0.004161509258950394,0.003712079024928686
+11.999999999999996,0.87,3.0,24.0,-0.014279806757392089,0.012362963326430745,-0.028653326888172747,0.02282287906936443
+11.999999999999996,0.93,3.0,26.0,-0.006236838029919955,0.010227950906720617,-0.011219816984618115,0.022396214946390734
+11.999999999999996,0.99,3.0,55.0,-0.0024549613698444735,0.0024716745407200973,-0.004728363642226435,0.004857973115034344
+11.999999999999996,1.05,3.0,13.0,-0.0028497851370841956,0.0017330131399254927,-0.0056722212841414975,0.0032950778920685982
```

### Comparing `pyspk-1.3/pyspk/stat_errors_500.csv` & `pyspk-1.4/pyspk/stat_errors_500.csv`

 * *Files 4% similar despite different names*

```diff
@@ -1,1472 +1,1467 @@
 k,f_b,z,n,error_68_m,error_68_p,error_95_m,error_95_p
-0.1000000000000021,0.33,0.0,24.0,-0.00018769284204510437,0.00018205085097340004,-0.0003446440936250003,0.00037490214667433775
-0.1000000000000021,0.39,0.0,37.0,-0.00013337218573796137,0.00014358244076190815,-0.0002550431017908064,0.00029331130881636954
-0.1000000000000021,0.45,0.0,34.0,-0.00010947162457476912,0.00013844908994619577,-0.00020337002141841018,0.0003015320246287809
-0.1000000000000021,0.51,0.0,53.0,-0.00012162512844698528,0.00014215615188549363,-0.00023282891752416908,0.00028908844743573257
-0.1000000000000021,0.57,0.0,45.0,-8.654978112272943e-05,0.00011977377987562702,-0.00015465067911850684,0.00024527375308249194
-0.1000000000000021,0.63,0.0,62.0,-9.092424729187987e-05,0.00010797305636131009,-0.0001733575111498774,0.000216151167791583
-0.1000000000000021,0.69,0.0,98.0,-8.081898638290348e-05,8.003166721852698e-05,-0.00015424963116147903,0.00015806914390899504
-0.1000000000000021,0.75,0.0,96.0,-9.730604218878523e-05,0.00010294794029572755,-0.00019038262586138613,0.00020490273729104562
-0.1000000000000021,0.81,0.0,45.0,-0.00015375406574542235,0.00011404977863856251,-0.00032317215109724446,0.0002149506758409981
-0.1270454343320594,0.33,0.0,24.0,-0.000266032074774732,0.00028158686310602704,-0.0005074725025186622,0.0005767292315436971
-0.1270454343320594,0.39,0.0,37.0,-0.00018498304472377286,0.00017646588376228284,-0.00035704357547158155,0.00036279990552981424
-0.1270454343320594,0.45,0.0,35.0,-0.00015437647146017178,0.00018574071701869045,-0.0002890587870124715,0.0003908914645389462
-0.1270454343320594,0.51,0.0,53.0,-0.0001410772755458766,0.00017004351514055658,-0.00026470689018637006,0.00033896440077166426
-0.1270454343320594,0.57,0.0,44.0,-9.768381867176058e-05,0.00013753774749994377,-0.00018852025129213225,0.00028225888051085517
-0.1270454343320594,0.63,0.0,62.0,-0.0001003945778837759,0.00011320974665449579,-0.00018293308343787052,0.00023732779048693807
-0.1270454343320594,0.69,0.0,99.0,-7.987293749367045e-05,8.098315024121748e-05,-0.0001621277121708426,0.00016159263546936445
-0.1270454343320594,0.75,0.0,98.0,-9.95973936301183e-05,0.00010354615347531953,-0.0001907757842479474,0.00021073890300679854
-0.1270454343320594,0.81,0.0,42.0,-0.00016214578908185158,0.00011399901536816958,-0.0003360691378006312,0.0002173354701468812
-0.161405423846202,0.27,0.0,6.0,-0.0009499325843105866,0.0009035840782288438,-0.0017834200517212922,0.001835371607400364
-0.161405423846202,0.33,0.0,23.0,-0.0004135343335908774,0.0004605507363766635,-0.0008052836348953743,0.0008952932513984539
-0.161405423846202,0.39,0.0,37.0,-0.0002494011113874923,0.0002619962987114482,-0.0004998994103531723,0.0005035194535021214
-0.161405423846202,0.45,0.0,35.0,-0.00022103632467829041,0.00023918849838106072,-0.00040270273323255384,0.0005167829522165535
-0.161405423846202,0.51,0.0,53.0,-0.00019392444426613305,0.00021140947715602435,-0.00036700581408341515,0.0004401526042030354
-0.161405423846202,0.57,0.0,44.0,-0.00013270607622637692,0.00017276211873946956,-0.0002411243334698783,0.0003561316483691542
-0.161405423846202,0.63,0.0,61.0,-0.0001212091202543677,0.00013576374620058175,-0.00023805431673934625,0.0002692735402952229
-0.161405423846202,0.69,0.0,101.0,-0.00010755062684258095,8.842614077759231e-05,-0.0002142264191713645,0.00017540119206871117
-0.161405423846202,0.75,0.0,97.0,-0.00011699523397204381,0.00011934204289754233,-0.00022639341490777177,0.0002404522413638474
-0.161405423846202,0.81,0.0,41.0,-0.00017569012021319223,0.00012541354589196973,-0.00037979046278293515,0.00023535120712012828
-0.2050582217609139,0.27,0.0,6.0,-0.0013759513151777591,0.0013554808620466947,-0.002622816382370626,0.0027485855679769875
-0.2050582217609139,0.33,0.0,24.0,-0.0006396941949833165,0.0006880202715783586,-0.0011371063505565288,0.0014590774847147213
-0.2050582217609139,0.39,0.0,36.0,-0.00037744816687788603,0.0003722670839008862,-0.0008026566616784475,0.0007339770047671908
-0.2050582217609139,0.45,0.0,37.0,-0.00031828485930382,0.00036624156720352656,-0.0006164155554301149,0.0007404914162257031
-0.2050582217609139,0.51,0.0,53.0,-0.00025018206061742384,0.00028654015856102716,-0.0004949623206874299,0.0005609800515643842
-0.2050582217609139,0.57,0.0,43.0,-0.00019602716762524082,0.00023907223272386267,-0.000375798922325369,0.0004761420704291834
-0.2050582217609139,0.63,0.0,60.0,-0.0001551371533909057,0.00017436185337551174,-0.00030504020764730096,0.00032603449817975825
-0.2050582217609139,0.69,0.0,105.0,-0.00018946693338341752,0.00013124824298119044,-0.00038048428439743973,0.0002456954094263947
-0.2050582217609139,0.75,0.0,93.0,-0.00018194588333809102,0.00015704845200524496,-0.00036298679904928977,0.0003024980852883145
-0.2050582217609139,0.81,0.0,41.0,-0.00020799190792891235,0.00015199094652098012,-0.0004490053678476185,0.00026515607742850236
-0.2605171084697324,0.27,0.0,8.0,-0.0014983339131963286,0.0016807327469188504,-0.0026938302168708905,0.0035385799484037275
-0.2605171084697324,0.33,0.0,22.0,-0.000976967978107394,0.001143359079596154,-0.001872364134281339,0.0022873833780735517
-0.2605171084697324,0.39,0.0,36.0,-0.0005863984278192182,0.0005097938556690499,-0.0011713384777466533,0.0010090170855542742
-0.2605171084697324,0.45,0.0,43.0,-0.0003870117651855522,0.000384913654322984,-0.0007481863575068004,0.0008216392569453865
-0.2605171084697324,0.51,0.0,48.0,-0.00038660064278320987,0.00039993617309401654,-0.0007236798793924663,0.000784475490796759
-0.2605171084697324,0.57,0.0,46.0,-0.00025711861750977956,0.0002925620464446355,-0.0004908545624970028,0.0005948215295003507
-0.2605171084697324,0.63,0.0,57.0,-0.00019051807829188346,0.00020696462331637407,-0.00037358252189774617,0.0003992192983455784
-0.2605171084697324,0.69,0.0,106.0,-0.00027146878533207446,0.0001806804383463604,-0.0005946890382157009,0.00032018037913328975
-0.2605171084697324,0.75,0.0,92.0,-0.0002240724829499484,0.00018287409162675382,-0.00046888522872452364,0.0003511773195148404
-0.2605171084697324,0.81,0.0,40.0,-0.00024536805955760666,0.0001780822747319075,-0.0005298130481532392,0.0003075502809064339
-0.3309750919646959,0.27,0.0,10.0,-0.0022192239551329404,0.0029001112119320053,-0.004107254617788137,0.006152307849755547
-0.3309750919646959,0.33,0.0,22.0,-0.0012174309491878865,0.0013757828926315825,-0.002242378100039757,0.0028469075224824792
-0.3309750919646959,0.39,0.0,34.0,-0.0008901448152324169,0.00076464489315455,-0.0017400560039869588,0.0014678449870880244
-0.3309750919646959,0.45,0.0,44.0,-0.0005156614552910392,0.0005424766682075307,-0.0010341831076750962,0.0011256556936702522
-0.3309750919646959,0.51,0.0,49.0,-0.0005054317147007545,0.0005145021836958186,-0.0009883704907076778,0.0010163801322939938
-0.3309750919646959,0.57,0.0,48.0,-0.0003572575856638894,0.00036923357890716077,-0.0006679461807350683,0.0007076141270972122
-0.3309750919646959,0.63,0.0,56.0,-0.0002682200800853717,0.0002783568885189369,-0.0005101027229742769,0.0005416709994029191
-0.3309750919646959,0.69,0.0,107.0,-0.00027224587942196234,0.0001960292912755513,-0.0005673504507005015,0.0003774481621068904
-0.3309750919646959,0.75,0.0,91.0,-0.00029860949536486114,0.00023836657822783175,-0.0006180395044843346,0.00043015558595010424
-0.3309750919646959,0.81,0.0,36.0,-0.00029840973196492934,0.00020499743042425595,-0.0006252699101858039,0.00036780020874927177
-0.4204887431174607,0.27,0.0,11.0,-0.0027167877885549284,0.0037801196281005535,-0.005299719590627841,0.00793914660169517
-0.4204887431174607,0.33,0.0,26.0,-0.0015768662425799697,0.001720517862987916,-0.003230287455754072,0.0033303533117373723
-0.4204887431174607,0.39,0.0,30.0,-0.001112860367541176,0.0009900381109370566,-0.002129666043472076,0.001975888828406151
-0.4204887431174607,0.45,0.0,46.0,-0.0007156008641226503,0.0007398264139697633,-0.0013986574211597282,0.0014828168707667134
-0.4204887431174607,0.51,0.0,48.0,-0.0006982847691899483,0.0007382071421895944,-0.0014018020839281845,0.0014028318262493144
-0.4204887431174607,0.57,0.0,48.0,-0.0004711186810556687,0.000443669360672931,-0.0008692541446340272,0.000933902061646387
-0.4204887431174607,0.63,0.0,57.0,-0.0003493398838923485,0.0003567352065478842,-0.0006988397517265723,0.0007333532240745675
-0.4204887431174607,0.69,0.0,109.0,-0.0002560635990678372,0.00023512604160862464,-0.0005128493811352722,0.0004621016141204739
-0.4204887431174607,0.75,0.0,87.0,-0.00039735516117552275,0.00030024036019000533,-0.000847911214521776,0.0005825815947331058
-0.4204887431174607,0.81,0.0,35.0,-0.00032638365194473623,0.0001921881567261741,-0.0007108775344666341,0.00035756076289233105
-0.5342117500109698,0.27,0.0,13.0,-0.003264299648402049,0.004023262118794957,-0.006046449802256521,0.008697026037549887
-0.5342117500109698,0.33,0.0,25.0,-0.0020608993989187988,0.002222952123266523,-0.004133073653125044,0.004410626768129221
-0.5342117500109698,0.39,0.0,33.0,-0.0014041109680170403,0.001346231558635719,-0.002865967049264134,0.0026868479947527576
-0.5342117500109698,0.45,0.0,46.0,-0.0009747240112982997,0.0009920646407340094,-0.0019294598725899913,0.0019443142313165422
-0.5342117500109698,0.51,0.0,46.0,-0.0009742595983229844,0.0009498480602928522,-0.0019499880838829604,0.00191292177395386
-0.5342117500109698,0.57,0.0,48.0,-0.0005901277223748852,0.000632744859592604,-0.0011544488321487908,0.0012495315629102804
-0.5342117500109698,0.63,0.0,60.0,-0.0004917714713949818,0.0004917096144409222,-0.0009878434963391865,0.0009735960721110925
-0.5342117500109698,0.69,0.0,111.0,-0.0003893197051075523,0.00032820257405784763,-0.0008661599013891382,0.0005996832341560478
-0.5342117500109698,0.75,0.0,82.0,-0.00031885137285074126,0.0003488040681683532,-0.0006107335354543312,0.0006714256082433787
-0.5342117500109698,0.81,0.0,33.0,-0.0003423843364428789,0.000199840540041141,-0.00079986549529153,0.0003536024799825895
-0.6786916380543103,0.27,0.0,17.0,-0.0036396062306992545,0.004303568870493571,-0.006729713583359759,0.008723865698800261
-0.6786916380543103,0.33,0.0,22.0,-0.0021805647863688163,0.0023253356823901943,-0.0043321896575298,0.004758025005932716
-0.6786916380543103,0.39,0.0,36.0,-0.0017726185093430173,0.0016582452170111068,-0.003393956318393297,0.0033698150668574835
-0.6786916380543103,0.45,0.0,45.0,-0.0011474973349459878,0.0011979284272760913,-0.0023034151292783407,0.002267409156052929
-0.6786916380543103,0.51,0.0,46.0,-0.0012594237524538709,0.0012096650247263843,-0.0024852565893582735,0.0023488428478610863
-0.6786916380543103,0.57,0.0,54.0,-0.0006798862505946416,0.0006455062847667281,-0.0012838833259711778,0.0013186205239354987
-0.6786916380543103,0.63,0.0,55.0,-0.0006263116259448512,0.0006520251023487153,-0.001256032297761727,0.0012078958072618971
-0.6786916380543103,0.69,0.0,115.0,-0.0004895562601644292,0.0003752820217719017,-0.0010703999238535532,0.0007391270542215957
-0.6786916380543103,0.75,0.0,75.0,-0.0004268178832519772,0.0004278768255059349,-0.000801438190388954,0.0008448499753240415
-0.6786916380543103,0.81,0.0,32.0,-0.0004060495457553171,0.00025578658109027993,-0.0009182686890562857,0.00045347277272181244
-0.8622467393414583,0.27,0.0,18.0,-0.003448888698910725,0.004323268946255998,-0.006808666935655093,0.008464103866416502
-0.8622467393414583,0.33,0.0,20.0,-0.0024494696460405805,0.0029980328058036836,-0.004875998679765536,0.00582400625985819
-0.8622467393414583,0.39,0.0,41.0,-0.001910173905124113,0.00197636067241955,-0.003888638670325579,0.0037118907309150752
-0.8622467393414583,0.45,0.0,53.0,-0.0013825217282135765,0.0013001132893468474,-0.002671905010574555,0.002533028254446924
-0.8622467393414583,0.51,0.0,38.0,-0.0014844449919894605,0.0014390374477586923,-0.0029518683073174634,0.00286081726675626
-0.8622467393414583,0.57,0.0,53.0,-0.000896578146443419,0.0008226958131882084,-0.0016762283527914938,0.0016593171270355208
-0.8622467393414583,0.63,0.0,52.0,-0.0007213231721679033,0.0007478112175611955,-0.001446293508180609,0.0013894573760844943
-0.8622467393414583,0.69,0.0,119.0,-0.0005397933446402599,0.0004817542806769079,-0.0011308517291985017,0.0009028533343975666
-0.8622467393414583,0.75,0.0,71.0,-0.000565841540719676,0.0005636350596686728,-0.001129708017411087,0.0011182640336779056
-0.8622467393414583,0.81,0.0,31.0,-0.0005384325689057251,0.00034727521199971734,-0.001215010484222482,0.0006355770206707203
-1.095445115010325,0.21,0.0,6.0,-0.0033900840850794403,0.0037634953830690994,-0.00632710974279797,0.008744453718213174
-1.095445115010325,0.27,0.0,18.0,-0.0029735538305630735,0.0039505326952664925,-0.005639244839036045,0.00807998919030684
-1.095445115010325,0.33,0.0,20.0,-0.002532022579638689,0.0030374768839695324,-0.004847661651633942,0.006017423038776128
-1.095445115010325,0.39,0.0,44.0,-0.0021401628037625554,0.0021501304984219167,-0.004069595566990109,0.00415231875218557
-1.095445115010325,0.45,0.0,50.0,-0.0016250734656478045,0.0015660728463811806,-0.0031981315749572215,0.0031668468902135744
-1.095445115010325,0.51,0.0,39.0,-0.0018061091213828699,0.0018228826201414044,-0.0036447712636610446,0.0034779264315302977
-1.095445115010325,0.57,0.0,50.0,-0.0009972024389191191,0.0009302802015699775,-0.0019630977156131634,0.0018821701202960137
-1.095445115010325,0.63,0.0,53.0,-0.0009006249842642826,0.0009217166946473662,-0.0017827618865160853,0.0017750443495529184
-1.095445115010325,0.69,0.0,123.0,-0.0005915432161724497,0.0005796394819339661,-0.0012246772170793371,0.0010935896789891976
-1.095445115010325,0.75,0.0,68.0,-0.000759212056974965,0.0008142805165697845,-0.001510675909092568,0.0015521148178589033
-1.095445115010325,0.81,0.0,28.0,-0.0005752520876809482,0.0003482425192553906,-0.00135296339020036,0.0006000934777926437
-1.3917130042341677,0.21,0.0,7.0,-0.0036298824447751976,0.0043972468350284896,-0.006807785334061345,0.008599339335179137
-1.3917130042341677,0.27,0.0,18.0,-0.002493269027680245,0.0035188802519416904,-0.004839008995348155,0.007367556585389766
-1.3917130042341677,0.33,0.0,21.0,-0.0024019489661461254,0.0028856777396969436,-0.004553439584444485,0.005832798008451723
-1.3917130042341677,0.39,0.0,43.0,-0.002175528780300283,0.002085700228775192,-0.004189443576936362,0.0040719573270707144
-1.3917130042341677,0.45,0.0,51.0,-0.0016739399722876414,0.0016019261515473697,-0.0031264222981420785,0.0031716779404426143
-1.3917130042341677,0.51,0.0,39.0,-0.0018423781920801506,0.0018937799493861174,-0.003779552524978978,0.0036048211390986747
-1.3917130042341677,0.57,0.0,48.0,-0.0011198349963706137,0.0011371194462249956,-0.002308362649208968,0.0021264005806232882
-1.3917130042341677,0.63,0.0,56.0,-0.000970897013559826,0.0008809630444212856,-0.0019242074254179813,0.0018089634709102201
-1.3917130042341677,0.69,0.0,117.0,-0.0006725578419286985,0.0006536956975899843,-0.0013830958440639767,0.0012069669403924543
-1.3917130042341677,0.75,0.0,72.0,-0.0007514636677501287,0.0007123558407564403,-0.001477360684947757,0.0014702904571185194
-1.3917130042341677,0.81,0.0,27.0,-0.0005986778648247424,0.0004217121575556041,-0.0013549867050294056,0.0007310627143465064
-1.7681078308849805,0.21,0.0,6.0,-0.004302542328159242,0.0038809104524695215,-0.008183452780628764,0.007913414875222236
-1.7681078308849805,0.27,0.0,20.0,-0.001960803123102603,0.002306585212934795,-0.0037423409691259126,0.004793477960979243
-1.7681078308849805,0.33,0.0,25.0,-0.0023142730256353983,0.00248523621640236,-0.004466577527821909,0.004859908197405647
-1.7681078308849805,0.39,0.0,36.0,-0.0021180049386616156,0.0022312514847286752,-0.0041165991538178485,0.004445791300556437
-1.7681078308849805,0.45,0.0,53.0,-0.0014396703310929858,0.0015429769075017501,-0.0030247676388336607,0.0027839615211853875
-1.7681078308849805,0.51,0.0,37.0,-0.0016232280090788024,0.0017426281475972263,-0.0034069358567050366,0.003229894329933297
-1.7681078308849805,0.57,0.0,41.0,-0.0012584855540358861,0.0013521019319954414,-0.0027128630237871184,0.002460753030364049
-1.7681078308849805,0.63,0.0,71.0,-0.0009494476886721169,0.0009449052204992224,-0.0020055532211690095,0.001802394641945104
-1.7681078308849805,0.69,0.0,113.0,-0.0007861402625013878,0.0007448077913295646,-0.001578028001903184,0.0014232705435180861
-1.7681078308849805,0.75,0.0,74.0,-0.0008136519618745873,0.0008190648985244352,-0.0016721259873897119,0.001547150557337504
-1.7681078308849805,0.81,0.0,23.0,-0.0008149576799110496,0.0006312968470673155,-0.0018223038440651853,0.0011292734184665404
-2.246300273206927,0.21,0.0,7.0,-0.004231566917721546,0.0032574411583417636,-0.008774840469060127,0.005925943522898609
-2.246300273206927,0.27,0.0,21.0,-0.0023340248748411232,0.0021451147613360134,-0.004503601667047855,0.004236097525425835
-2.246300273206927,0.33,0.0,32.0,-0.002218626664557278,0.0021956225430147963,-0.004425595138218549,0.004213586320087367
-2.246300273206927,0.39,0.0,33.0,-0.001957909558149439,0.002176284901542067,-0.003937326871088928,0.0039455175783555015
-2.246300273206927,0.45,0.0,50.0,-0.0015331275387272401,0.0014657509799117197,-0.0028315497033351384,0.0031899535319658543
-2.246300273206927,0.51,0.0,38.0,-0.0015619345738477027,0.0016367540476742851,-0.003182041786090112,0.003087165070650648
-2.246300273206927,0.57,0.0,37.0,-0.0015426179926531602,0.0014964232342240347,-0.002947041289618653,0.0030304661472463092
-2.246300273206927,0.63,0.0,73.0,-0.0011561785568487506,0.0011055126333352648,-0.002385030221707084,0.0021706154541860883
-2.246300273206927,0.69,0.0,104.0,-0.0010368475168210784,0.0010120152824757262,-0.0020718134143505296,0.0019725277129465954
-2.246300273206927,0.75,0.0,85.0,-0.0011694324200034717,0.0010847498699755034,-0.0023495119851263285,0.0021435949097078893
-2.246300273206927,0.81,0.0,18.0,-0.0014953903647618937,0.0011135143511464536,-0.0031647173762222387,0.0020575059044367584
-2.85382193849788,0.21,0.0,11.0,-0.002619098561167482,0.0025129207916002286,-0.005169762953543069,0.0048359157101139725
-2.85382193849788,0.27,0.0,24.0,-0.0023406205033410315,0.002279107741674032,-0.004513004789269671,0.0044319268786555364
-2.85382193849788,0.33,0.0,31.0,-0.002248497252684725,0.002282691321526147,-0.004333652809898209,0.004466543220581904
-2.85382193849788,0.39,0.0,43.0,-0.0019521898309603197,0.0018801769268216072,-0.00406575412977752,0.0036537605966204347
-2.85382193849788,0.45,0.0,41.0,-0.0015663508684372915,0.0016901500977420042,-0.0031618965617748883,0.0033013315459479524
-2.85382193849788,0.51,0.0,42.0,-0.001709571268665799,0.0016487737814399562,-0.0035142649178562823,0.0032587114702584317
-2.85382193849788,0.57,0.0,47.0,-0.0015673413243142203,0.001369755848473555,-0.003012136553580077,0.0027713579069166385
-2.85382193849788,0.63,0.0,70.0,-0.0012547779755959071,0.0012529204380967713,-0.002425992787095217,0.002356343471918502
-2.85382193849788,0.69,0.0,109.0,-0.001163113441323726,0.0010558080020945382,-0.0022033630367435373,0.002132131496381675
-2.85382193849788,0.75,0.0,69.0,-0.0010901339782465253,0.0010130234550782126,-0.0021961294668582042,0.0019217523885726175
-2.85382193849788,0.81,0.0,11.0,-0.001180275444576678,0.001101484434325529,-0.002297214588163435,0.002123182170369214
-3.625650476828121,0.21,0.0,15.0,-0.0027138950161829643,0.0032737410555710084,-0.005060244788758796,0.007033948431976265
-3.625650476828121,0.27,0.0,26.0,-0.002172526156112487,0.0023626268792154774,-0.004139531990617596,0.004718627939682331
-3.625650476828121,0.33,0.0,39.0,-0.00230216596867965,0.002444653104455972,-0.004538459337515227,0.004684352993870234
-3.625650476828121,0.39,0.0,48.0,-0.002203650833424668,0.0022143052352051646,-0.00448168189501315,0.004392878610335784
-3.625650476828121,0.45,0.0,54.0,-0.0020744515481775374,0.0020303896770765607,-0.0038990284237471464,0.004163793897692574
-3.625650476828121,0.51,0.0,50.0,-0.002415269227904982,0.002235844927073135,-0.004922956702367579,0.004333817936153857
-3.625650476828121,0.57,0.0,42.0,-0.002482924601253074,0.0025770017689906765,-0.004867299836357295,0.005280954795438493
-3.625650476828121,0.63,0.0,91.0,-0.001250442029902202,0.0011843482160521024,-0.0023900052187236804,0.002351998157888623
-3.625650476828121,0.69,0.0,86.0,-0.0010843152074063902,0.0010960423001592438,-0.002094356388489281,0.0022052601886704405
-3.625650476828121,0.75,0.0,42.0,-0.0008531984036474537,0.0008614763488005513,-0.0016775959543012268,0.0016693751651354583
-4.606223395648531,0.15,0.0,5.0,-0.0017554588768616372,0.0023260398109516745,-0.003364749648747778,0.004108711079992622
-4.606223395648531,0.21,0.0,20.0,-0.0017718041728222674,0.0019132121603967094,-0.0036138216606928283,0.0035416962426544573
-4.606223395648531,0.27,0.0,33.0,-0.0017449438930114227,0.0019369470545600076,-0.0033571747709806726,0.0037564167393783106
-4.606223395648531,0.33,0.0,53.0,-0.00195183728627124,0.002095006598121528,-0.004022404413719496,0.0038969796015931595
-4.606223395648531,0.39,0.0,52.0,-0.002360129718561866,0.002341221592180908,-0.004758757088625744,0.004502260535227255
-4.606223395648531,0.45,0.0,47.0,-0.0028620760772513866,0.002669624075161156,-0.005954600888070412,0.005032987709010408
-4.606223395648531,0.51,0.0,48.0,-0.0029424603854235217,0.0026315589559249477,-0.005943941047362605,0.005104122113061581
-4.606223395648531,0.57,0.0,46.0,-0.003286971620952815,0.0028756154352339203,-0.006448636499619769,0.005755821359723225
-4.606223395648531,0.63,0.0,90.0,-0.0015069961305212893,0.001397343022546636,-0.002982591087625021,0.0028426552518491335
-4.606223395648531,0.69,0.0,81.0,-0.0013701703577081077,0.0013868003982122955,-0.0026867922714108225,0.0027602838563691033
-4.606223395648531,0.75,0.0,25.0,-0.0018936746784975066,0.001956377231575393,-0.0037684126525979493,0.0037276740266356198
-5.851996519306438,0.15,0.0,8.0,-0.003948844209009622,0.004716987595847294,-0.0076044208308067435,0.00971286283523587
-5.851996519306438,0.21,0.0,26.0,-0.002336500566313065,0.0021688270178904985,-0.004979798718984147,0.003885496600734576
-5.851996519306438,0.27,0.0,39.0,-0.0020344067850096557,0.0021073895439881344,-0.003986639969197702,0.004226306262064493
-5.851996519306438,0.33,0.0,55.0,-0.001903799499470925,0.00184285380526415,-0.0037923814668022154,0.003535944649641395
-5.851996519306438,0.39,0.0,54.0,-0.0027709421155228645,0.002587129746922397,-0.005346127086747613,0.004954447033080894
-5.851996519306438,0.45,0.0,49.0,-0.003017941050311521,0.0030851344978660594,-0.0061994823266022904,0.005705180936182353
-5.851996519306438,0.51,0.0,41.0,-0.0037193768853385927,0.0032220440160769005,-0.007854911067464517,0.0062692923526469334
-5.851996519306438,0.57,0.0,53.0,-0.002816041554047216,0.0024477668657831068,-0.005663104016391156,0.00474692215594045
-5.851996519306438,0.63,0.0,97.0,-0.001744909275853916,0.0017264600285767935,-0.0034062641211470186,0.0032657542023048934
-5.851996519306438,0.69,0.0,64.0,-0.0018998484947766285,0.0018647760282235661,-0.00357745393917772,0.003699085946598583
-5.851996519306438,0.75,0.0,14.0,-0.0031351798932984175,0.002970047860526798,-0.006057902064485834,0.005908922644296077
-7.434694395049632,0.15,0.0,12.0,-0.004173508246142233,0.0042269891273957584,-0.00813097074930627,0.007935476089210688
-7.434694395049632,0.21,0.0,32.0,-0.0027946996103472566,0.0024643187398064987,-0.005649357744670329,0.004714163790654898
-7.434694395049632,0.27,0.0,54.0,-0.002176819219804924,0.0019958058947516727,-0.0041680753619185865,0.004105542358537151
-7.434694395049632,0.33,0.0,54.0,-0.0028360820157788,0.0026930439637039994,-0.005569857051021571,0.00525991513815273
-7.434694395049632,0.39,0.0,60.0,-0.003167143394705923,0.002858054010147536,-0.006007156549686583,0.005495836824585277
-7.434694395049632,0.45,0.0,49.0,-0.003994325080451069,0.0035520876320890146,-0.008142662045567071,0.007166777093470107
-7.434694395049632,0.51,0.0,47.0,-0.0036335853718222886,0.0030773925437091636,-0.007160030415160063,0.005751298823456349
-7.434694395049632,0.57,0.0,66.0,-0.0029783156881280385,0.002551001709711893,-0.005921677820367602,0.004862729297876228
-7.434694395049632,0.63,0.0,80.0,-0.0027160827427272845,0.002648823130623067,-0.0054786455673769534,0.005117143811242345
-7.434694395049632,0.69,0.0,39.0,-0.0031897364686700094,0.003960982832210318,-0.006472507956027235,0.007596551856798625
-7.434694395049632,0.75,0.0,7.0,-0.005482261627490668,0.004435648006469117,-0.011480643516065545,0.007817919885167588
-9.445439785451793,0.15,0.0,20.0,-0.0037067471940159624,0.003708242583843351,-0.0073769165936424025,0.007034444608407299
-9.445439785451793,0.21,0.0,29.0,-0.0027244425682248297,0.0024691194463654876,-0.0054210881511630084,0.004879981433197511
-9.445439785451793,0.27,0.0,63.0,-0.0022586517891448805,0.002246015190903477,-0.004302704287270436,0.004477499840215965
-9.445439785451793,0.33,0.0,71.0,-0.0029399985514540925,0.002839240156913923,-0.005619380589973068,0.00569909635758005
-9.445439785451793,0.39,0.0,57.0,-0.004069324776499836,0.003563668548746034,-0.008009345751599485,0.0071016035264186315
-9.445439785451793,0.45,0.0,52.0,-0.0036550968294192295,0.0033774956049257114,-0.007396272105426044,0.006473279697771369
-9.445439785451793,0.51,0.0,56.0,-0.003551109283022462,0.0031569748482000574,-0.007144926590448721,0.005927769225330833
-9.445439785451793,0.57,0.0,65.0,-0.003540591666579925,0.0034842895622611853,-0.0073649887815952966,0.006452096522026621
-9.445439785451793,0.63,0.0,61.0,-0.003487077569220376,0.0033855645353990976,-0.006962354038671056,0.006890794371852395
-9.445439785451793,0.69,0.0,22.0,-0.005663879138033456,0.00618125784117393,-0.011080925807725395,0.012064949037246833
-12.0,0.15,0.0,18.0,-0.004081658054631096,0.003660522608042719,-0.00784961727524956,0.007329844067785283
-12.0,0.21,0.0,50.0,-0.0030145183516788895,0.002792862195268502,-0.00592676291699611,0.005729038044058071
-12.0,0.27,0.0,62.0,-0.0032792988307710643,0.003352653920336765,-0.006541141249696474,0.006515845632053402
-12.0,0.33,0.0,79.0,-0.0030377229952963853,0.0031173727113454537,-0.0058109976281050186,0.0063178636135901006
-12.0,0.39,0.0,63.0,-0.003371707068912893,0.0034370330493141616,-0.007001172336381656,0.006454168795673562
-12.0,0.45,0.0,63.0,-0.003996715355391686,0.003423548109289615,-0.00815852641285359,0.00668197796995074
-12.0,0.51,0.0,58.0,-0.0048220288900474315,0.00468483571415951,-0.009574559991890294,0.008862003980324896
-12.0,0.57,0.0,59.0,-0.00527105307021714,0.0050545826296526245,-0.010645523984967724,0.009575140200591822
-12.0,0.63,0.0,33.0,-0.004844621634146876,0.005466836338477124,-0.009863859666201617,0.010748495872852532
-12.0,0.69,0.0,10.0,-0.011789631915749645,0.011812288526394854,-0.021791323185459604,0.023958572315044398
-0.0999999999999921,0.27,0.125,14.0,-0.0001384309360201758,0.00018952177151572945,-0.0002604018003513404,0.00038637642569131837
-0.0999999999999921,0.33,0.125,23.0,-0.00013396293887023923,0.00011345518434152726,-0.0002786053290909354,0.00021263940471897929
-0.0999999999999921,0.39,0.125,32.0,-0.00012920978391256388,0.00016011401536675723,-0.0002351690898397727,0.0003479684160794638
-0.0999999999999921,0.45,0.125,45.0,-0.0001061748640189739,0.00012729383953996308,-0.00020013791580406556,0.000258487473077266
-0.0999999999999921,0.51,0.125,50.0,-9.828027630178993e-05,0.00012501403396066144,-0.00018834187843860868,0.0002533830336809826
-0.0999999999999921,0.57,0.125,55.0,-9.168675457831974e-05,0.00011081261046824955,-0.0001769406205166373,0.00023757075127328942
-0.0999999999999921,0.63,0.125,69.0,-8.417139352412e-05,9.771776464272976e-05,-0.0001547059639995854,0.00020503182681595492
-0.0999999999999921,0.69,0.125,103.0,-5.83104410239974e-05,6.297039625300719e-05,-0.00010861465924265642,0.0001402977913213357
-0.0999999999999921,0.75,0.125,76.0,-0.00010924552579336623,0.00011510704942090404,-0.00021102959876086506,0.00023564587197005122
-0.0999999999999921,0.81,0.125,29.0,-0.00015966194634701848,8.63868813604951e-05,-0.00038960610810628556,0.0001640768178087242
-0.1270454343320576,0.27,0.125,14.0,-0.0002143256793517733,0.00030190145243252003,-0.00040750345070808514,0.0006338398079004263
-0.1270454343320576,0.33,0.125,24.0,-0.0001910755940712743,0.00016010117947016112,-0.00040109987943650065,0.0002990678733803945
-0.1270454343320576,0.39,0.125,31.0,-0.00017750187226446074,0.00019692214849323473,-0.0003214002783040461,0.00042208879368076975
-0.1270454343320576,0.45,0.125,50.0,-0.00013844555228529774,0.0001508679539004184,-0.00025577404584564467,0.0002989074030668314
-0.1270454343320576,0.51,0.125,46.0,-0.00011853740093367831,0.00014897644142181405,-0.00022434348209368648,0.00030074400555374955
-0.1270454343320576,0.57,0.125,54.0,-0.00010692710935719995,0.00012813195992894205,-0.00020789349070179347,0.0002580177171323205
-0.1270454343320576,0.63,0.125,68.0,-9.047730243368548e-05,0.00010159109613392584,-0.00017223139749844113,0.00021652196467269417
-0.1270454343320576,0.69,0.125,104.0,-5.7525448325854714e-05,7.000696859493262e-05,-0.00011592320626334929,0.00014059709329981423
-0.1270454343320576,0.75,0.125,76.0,-0.00011034089435259719,0.00011834115077948487,-0.00021979447477159825,0.00023366731741231966
-0.1270454343320576,0.81,0.125,29.0,-0.000165326096534499,8.781120894953888e-05,-0.0003968267548058277,0.0001693083596337495
-0.1614054238462,0.27,0.125,14.0,-0.00034898749777242396,0.0004425955265183073,-0.0006632046507736132,0.0009302571339893933
-0.1614054238462,0.33,0.125,26.0,-0.00029976965605492135,0.0002476201509123745,-0.0005900031795953517,0.0004875433142972645
-0.1614054238462,0.39,0.125,31.0,-0.00022721820856430177,0.00026952127766040107,-0.00045610792096032,0.0005321051404160556
-0.1614054238462,0.45,0.125,48.0,-0.00020039266723509942,0.00021086863454005016,-0.000379026015812696,0.0004348935932514495
-0.1614054238462,0.51,0.125,46.0,-0.00016026877924646562,0.00019701906355386518,-0.0003057905083360024,0.00037918374256253615
-0.1614054238462,0.57,0.125,53.0,-0.00014341355846325446,0.0001608171646973717,-0.0002769760613130103,0.0003338670916552049
-0.1614054238462,0.63,0.125,68.0,-0.00010691909212478989,0.00011759066791582938,-0.00020751407549855972,0.00023553166126751238
-0.1614054238462,0.69,0.125,103.0,-7.508130041226545e-05,7.8034878744875e-05,-0.00014302450307322645,0.00015790491969959008
-0.1614054238462,0.75,0.125,78.0,-0.00011780503363122659,0.00012679780340812583,-0.00023308102285345922,0.0002477588060437009
-0.1614054238462,0.81,0.125,29.0,-0.00017854214869953767,9.962525408199012e-05,-0.0004255914604866363,0.0001862578386095149
-0.2050582217609055,0.27,0.125,14.0,-0.0005162175938176562,0.0006625007789667493,-0.0009877364143777078,0.001380364697546764
-0.2050582217609055,0.33,0.125,26.0,-0.00047012464794558254,0.00040559784485193884,-0.0009308249570298313,0.0007610352876646
-0.2050582217609055,0.39,0.125,32.0,-0.0003439303514250107,0.00037075028385279824,-0.0006799527948878277,0.0007422671417528859
-0.2050582217609055,0.45,0.125,48.0,-0.0003099662003770892,0.00031304839679899233,-0.0006021959654921475,0.0006148485250198092
-0.2050582217609055,0.51,0.125,45.0,-0.00023148459289153825,0.0002566835277690749,-0.0004262824064188605,0.0005280925293940837
-0.2050582217609055,0.57,0.125,54.0,-0.00019383152166789104,0.0002302652891326832,-0.00039131737919475537,0.0004450130615598515
-0.2050582217609055,0.63,0.125,64.0,-0.0001386575095322352,0.00016029799557518745,-0.000270158179229566,0.00033558644476589677
-0.2050582217609055,0.69,0.125,105.0,-0.00011134333276052109,9.995246267557627e-05,-0.00022701797585344345,0.0002016867337931234
-0.2050582217609055,0.75,0.125,82.0,-0.00014752503977765,0.00013563752245679593,-0.0002762156679737114,0.0002906376498918814
-0.2050582217609055,0.81,0.125,26.0,-0.0002340199199563465,0.0001304826726033167,-0.000500733396798072,0.0002512987346424907
-0.2605171084697262,0.27,0.125,15.0,-0.0007208586913125876,0.0008240115709037231,-0.0013536531779091382,0.0017903588499115753
-0.2605171084697262,0.33,0.125,25.0,-0.000722502240900756,0.0006219080617359213,-0.001442208082638892,0.00122855324430038
-0.2605171084697262,0.39,0.125,35.0,-0.0005080017719170135,0.00048550860519084747,-0.0010172201731795999,0.0009515921942016639
-0.2605171084697262,0.45,0.125,46.0,-0.00041300356040446725,0.00042769910084836983,-0.0007958260865046299,0.0008480592041237483
-0.2605171084697262,0.51,0.125,45.0,-0.0003014202031481359,0.00032553178835799406,-0.0005742014085714043,0.0006637362658384537
-0.2605171084697262,0.57,0.125,53.0,-0.00025939139859598986,0.00027591577360712384,-0.0005099131000640562,0.0005541915386294856
-0.2605171084697262,0.63,0.125,60.0,-0.00018159407902594376,0.00020789703207811473,-0.0003601421232498655,0.0004023787129674645
-0.2605171084697262,0.69,0.125,106.0,-0.00015600220422459256,0.00012508794383763003,-0.00034018307122392333,0.0002318146481973801
-0.2605171084697262,0.75,0.125,85.0,-0.00015237620790939122,0.00016384425148285436,-0.0003080762623830224,0.0003302441347055878
-0.2605171084697262,0.81,0.125,26.0,-0.00025041994816599146,0.000151985529126204,-0.0005348551716404929,0.00027816983393130215
-0.3309750919646976,0.27,0.125,15.0,-0.0009325563112475071,0.0012322838270754648,-0.0018567522071123788,0.002355731599714926
-0.3309750919646976,0.33,0.125,26.0,-0.0009699407888852893,0.0009371842504079273,-0.0019859440749585193,0.001743898859024237
-0.3309750919646976,0.39,0.125,36.0,-0.0007664584531805632,0.0007292450214062091,-0.0014761221952314303,0.001351892025011918
-0.3309750919646976,0.45,0.125,45.0,-0.0005757332765778641,0.0005799980052256842,-0.0011025136006897391,0.0011381561722499031
-0.3309750919646976,0.51,0.125,45.0,-0.0004128656075673822,0.0004559408527783395,-0.0007847845280756883,0.0009105430618831389
-0.3309750919646976,0.57,0.125,50.0,-0.0003825023503780966,0.00037892818756665644,-0.0007209308755087903,0.000771177977504481
-0.3309750919646976,0.63,0.125,59.0,-0.0002427126370703299,0.0002680174659352656,-0.000482314401518787,0.0005163501996401647
-0.3309750919646976,0.69,0.125,107.0,-0.00019390476440765076,0.0001573406546663435,-0.0004035970392561944,0.0003097144051725422
-0.3309750919646976,0.75,0.125,87.0,-0.00018890749012517134,0.00018853523699722416,-0.000363916254505924,0.00037776233728648376
-0.3309750919646976,0.81,0.125,26.0,-0.000286548285548162,0.00017633388388142474,-0.000598356938448207,0.0003269356210684298
-0.4204887431174574,0.27,0.125,15.0,-0.0013351853932636003,0.0015487430560768007,-0.0024998166916624792,0.0031392798787574705
-0.4204887431174574,0.33,0.125,28.0,-0.0012326423507451314,0.0011858333346413722,-0.002413160301858626,0.0022303142330608802
-0.4204887431174574,0.39,0.125,35.0,-0.0010897565481447309,0.001092170319604024,-0.0022731862265112247,0.002049192376097023
-0.4204887431174574,0.45,0.125,47.0,-0.0007450140199140277,0.0007878956098335971,-0.001529308549790017,0.0015229547664373274
-0.4204887431174574,0.51,0.125,43.0,-0.0006412196458588428,0.0006269022022832643,-0.0012768405610802073,0.0013066661498701304
-0.4204887431174574,0.57,0.125,46.0,-0.0005347226704565655,0.000568553806753854,-0.0010352782149082424,0.0010717972127066067
-0.4204887431174574,0.63,0.125,63.0,-0.00033286737769640967,0.00036449660205096135,-0.000652731914764493,0.0006974161976824006
-0.4204887431174574,0.69,0.125,102.0,-0.0002456773188401586,0.00023239764401286855,-0.0005257860698568116,0.0004122912128965832
-0.4204887431174574,0.75,0.125,89.0,-0.00023204378261817827,0.00023690655064247373,-0.00046332760913150303,0.00046709058731746856
-0.4204887431174574,0.81,0.125,28.0,-0.0004211077359144328,0.0002925176280952442,-0.0008893491800826685,0.0005696580598043675
-0.534211750010971,0.27,0.125,15.0,-0.0018950065098124985,0.002052536467297712,-0.003600916107923546,0.00429117231080688
-0.534211750010971,0.33,0.125,27.0,-0.0016203624291885282,0.0015030859426965032,-0.0033019696451806533,0.0028087367953685506
-0.534211750010971,0.39,0.125,37.0,-0.0014684301662564081,0.0014174685234257852,-0.002999599045668882,0.002771506554585021
-0.534211750010971,0.45,0.125,46.0,-0.0010352599117334812,0.001094659826599956,-0.002033445572239395,0.0021489345462510877
-0.534211750010971,0.51,0.125,42.0,-0.0008511303741330369,0.000870555412903479,-0.0016825926057836315,0.0016699180636357725
-0.534211750010971,0.57,0.125,44.0,-0.0007650545207404731,0.0007758733795960854,-0.0014538780292302192,0.0015175697819193837
-0.534211750010971,0.63,0.125,65.0,-0.0004528995672176553,0.0004764360365896784,-0.000837884587938588,0.0009515836781209985
-0.534211750010971,0.69,0.125,96.0,-0.0003546774276044297,0.0003274462074159318,-0.0007129483359587054,0.0006449144171808979
-0.534211750010971,0.75,0.125,99.0,-0.0002931533464405265,0.0002978888043312801,-0.0005614395821232811,0.0006150149492514967
-0.534211750010971,0.81,0.125,24.0,-0.0006299223224896741,0.00047186790779331735,-0.0013447575206273184,0.0008587521365152767
-0.6786916380543273,0.27,0.125,16.0,-0.002249345202840069,0.00232737155833768,-0.004327222010138521,0.004688834362948721
-0.6786916380543273,0.33,0.125,27.0,-0.002091385473641814,0.0018809618332414645,-0.004244406125401239,0.003700428444451646
-0.6786916380543273,0.39,0.125,37.0,-0.0018737823707130259,0.0016703711486698142,-0.0037722254339360357,0.0032922637389815475
-0.6786916380543273,0.45,0.125,44.0,-0.0013285953127086419,0.0013350170750605506,-0.00260432677940302,0.0026744013070405265
-0.6786916380543273,0.51,0.125,42.0,-0.001062480822878924,0.001040345790801522,-0.002101667036502021,0.002148376269086756
-0.6786916380543273,0.57,0.125,45.0,-0.0008893430306684457,0.0009434954489586931,-0.0017832093846097147,0.0018216526558651502
-0.6786916380543273,0.63,0.125,60.0,-0.0006199743029811175,0.0006429610273929447,-0.001215819676890434,0.0012664816587203004
-0.6786916380543273,0.69,0.125,93.0,-0.00047913082113416514,0.00042395959846250753,-0.0009528879255085914,0.0008576224381939493
-0.6786916380543273,0.75,0.125,107.0,-0.00038550233711385953,0.0003847117760063063,-0.0007416986039686644,0.000797176167990954
-0.6786916380543273,0.81,0.125,24.0,-0.0008376903702873314,0.0006958645211191285,-0.0017706245752469665,0.0012103669497512258
-0.8622467393414398,0.21,0.125,6.0,-0.0030405703944345838,0.002620691185597268,-0.005714445880695899,0.0054190480464168704
-0.8622467393414398,0.27,0.125,13.0,-0.0032500034881316913,0.00329001275749016,-0.0062984358391790975,0.006564025561492087
-0.8622467393414398,0.33,0.125,30.0,-0.0024714042944428433,0.002057528947763173,-0.004756696223482447,0.003947936014388379
-0.8622467393414398,0.39,0.125,34.0,-0.002307899411748132,0.002024383714573183,-0.004754476356080626,0.003844977420560996
-0.8622467393414398,0.45,0.125,47.0,-0.0014881890235831838,0.0015140647626917143,-0.003077939252955642,0.0028754950964573543
-0.8622467393414398,0.51,0.125,40.0,-0.0013752763502476158,0.0012776839843822504,-0.0027592186915946187,0.0025477698524035653
-0.8622467393414398,0.57,0.125,44.0,-0.001078118102072591,0.0011209534636297872,-0.0021450564135188387,0.002082557208901135
-0.8622467393414398,0.63,0.125,57.0,-0.0007790545605839031,0.000833913865170706,-0.0015490972549475795,0.0016359108153977933
-0.8622467393414398,0.69,0.125,87.0,-0.0005915023669461252,0.0005943852664190484,-0.0011350387640174727,0.00119900104289563
-0.8622467393414398,0.75,0.125,113.0,-0.0005996514997948572,0.0005470597441828403,-0.001126198257019214,0.00109014567344745
-0.8622467393414398,0.81,0.125,27.0,-0.0010888314503095789,0.0009633518897084585,-0.0022391295378327535,0.0018037075870188846
-1.0954451150103284,0.21,0.125,7.0,-0.0035415497945731076,0.0027968365760969722,-0.006830184284289769,0.005086880981620831
-1.0954451150103284,0.27,0.125,18.0,-0.0030759326771842275,0.0029452379939016613,-0.0062193118939358185,0.005610654239533368
-1.0954451150103284,0.33,0.125,31.0,-0.00257622792524936,0.002339075916514345,-0.005127692527055789,0.004406239082422169
-1.0954451150103284,0.39,0.125,29.0,-0.002936534405410634,0.002569924852505153,-0.0060501011765452,0.004835029933406214
-1.0954451150103284,0.45,0.125,49.0,-0.001683554118607225,0.0016631016465849856,-0.003346295295251686,0.0031940374992954915
-1.0954451150103284,0.51,0.125,38.0,-0.001608290883297982,0.0015925159236411328,-0.0033238020320596404,0.0030711476868369838
-1.0954451150103284,0.57,0.125,45.0,-0.001301223371224271,0.001284963378870033,-0.0025747378303663743,0.002542556429890056
-1.0954451150103284,0.63,0.125,52.0,-0.001164114612649699,0.0011351360315891021,-0.002181231513876752,0.0023046824563973975
-1.0954451150103284,0.69,0.125,77.0,-0.0007927403788356567,0.0008178385421614394,-0.0015453128610748196,0.001730040518066732
-1.0954451150103284,0.75,0.125,117.0,-0.0007663063458913229,0.0007887874183619214,-0.001544466935975792,0.0015551686400080377
-1.0954451150103284,0.81,0.125,35.0,-0.0012429518254686114,0.0012357039568028575,-0.0024258061020136354,0.002358737427862408
-1.3917130042341714,0.21,0.125,7.0,-0.0036164872184365478,0.002697844895220514,-0.006865781947597143,0.005166259992411226
-1.3917130042341714,0.27,0.125,18.0,-0.003298593021691153,0.0030501126705637645,-0.006687857606169827,0.0057324975717007245
-1.3917130042341714,0.33,0.125,35.0,-0.002426349406710963,0.002234311823072704,-0.005214767553962498,0.004247692996573242
-1.3917130042341714,0.39,0.125,30.0,-0.0028269233445115697,0.002412861415764345,-0.005877191286940703,0.004491112221149173
-1.3917130042341714,0.45,0.125,47.0,-0.001870045848927503,0.0018548918237616758,-0.0037137312833841487,0.00361227041682591
-1.3917130042341714,0.51,0.125,37.0,-0.0018602568641684107,0.0017025508993378886,-0.0034875162676319444,0.0033427719388208765
-1.3917130042341714,0.57,0.125,42.0,-0.0015939886746118759,0.0015207862680299443,-0.002989817278407912,0.003010341697733684
-1.3917130042341714,0.63,0.125,53.0,-0.0013382446649324415,0.0014111796477694525,-0.002699526190075694,0.0027317496642361287
-1.3917130042341714,0.69,0.125,79.0,-0.0009381668603301842,0.000987329235060832,-0.0018728975724380187,0.0019788813211896452
-1.3917130042341714,0.75,0.125,118.0,-0.0009584744917784273,0.0009501802422715646,-0.0019019418981958628,0.0018529947906271338
-1.3917130042341714,0.81,0.125,32.0,-0.0014091663272941385,0.0014160369806574288,-0.0028262859840173164,0.0027994665129434013
-1.768107830884987,0.21,0.125,8.0,-0.0021347664239314943,0.0022049584119009195,-0.00405527917843658,0.004371423937232138
-1.768107830884987,0.27,0.125,19.0,-0.0029593071154308814,0.0028150565902321082,-0.0059890855606213825,0.005459150773693121
-1.768107830884987,0.33,0.125,34.0,-0.002270748894546109,0.002012912043329775,-0.004463107959838611,0.0039029771852165675
-1.768107830884987,0.39,0.125,37.0,-0.002175542689907392,0.002071201924415039,-0.004322106179432156,0.004119069497110459
-1.768107830884987,0.45,0.125,48.0,-0.0017819887744234604,0.0016464769911288509,-0.0034570446954457004,0.003223775958200439
-1.768107830884987,0.51,0.125,35.0,-0.0019337272892021413,0.0018433076929864566,-0.0038338316814319966,0.0036233641063720128
-1.768107830884987,0.57,0.125,45.0,-0.0015608488182278716,0.0015524521280567832,-0.003219543220624717,0.0029765249351731875
-1.768107830884987,0.63,0.125,56.0,-0.0013459859740319274,0.0013616623244302145,-0.0026174077335420166,0.0026366460758796848
-1.768107830884987,0.69,0.125,101.0,-0.0010350996853214208,0.0009777017347102747,-0.0020274788643926322,0.0019279767058906201
-1.768107830884987,0.75,0.125,99.0,-0.0011054844402697721,0.0010472925236385726,-0.002112305775409584,0.002112489605607331
-1.768107830884987,0.81,0.125,16.0,-0.0024857875935480993,0.0022559006618864596,-0.004938777979566433,0.004397713428108061
-2.2463002732069133,0.21,0.125,9.0,-0.00313312463209691,0.0025288722193678487,-0.006441287086677536,0.0046571114747220145
-2.2463002732069133,0.27,0.125,22.0,-0.002830502316966009,0.0027071076050800263,-0.005788779587724744,0.0055672465358461605
-2.2463002732069133,0.33,0.125,34.0,-0.0018630582161564431,0.0020777606478262745,-0.0038367895639262366,0.004068904218917838
-2.2463002732069133,0.39,0.125,39.0,-0.0017993012198439502,0.001764443242592385,-0.003361402970922597,0.0035966654860064237
-2.2463002732069133,0.45,0.125,52.0,-0.001704753854690112,0.0016986713995438142,-0.0033518920368685256,0.0033056035181171922
-2.2463002732069133,0.51,0.125,40.0,-0.0016609318121079439,0.0016890963720343672,-0.0033255050058519195,0.0032780246427901202
-2.2463002732069133,0.57,0.125,52.0,-0.0013817886061728963,0.0012676540756197856,-0.0027786902270985595,0.002468498621298603
-2.2463002732069133,0.63,0.125,63.0,-0.0014691973183386259,0.0013708559023939268,-0.0028823124585380874,0.0027341840648485685
-2.2463002732069133,0.69,0.125,123.0,-0.0009456203313681403,0.000957780975493766,-0.0018955920459607812,0.001886828492727358
-2.2463002732069133,0.75,0.125,59.0,-0.001261088188602884,0.0011872531405145426,-0.0025243828988471334,0.002393931132998433
-2.2463002732069133,0.81,0.125,5.0,-0.0035282568273792723,0.003528256827379272,-0.00631635449538599,0.007076791587955622
-2.853821938497887,0.21,0.125,11.0,-0.002967344331618206,0.0030959910061035835,-0.005956398762687567,0.005767650275033494
-2.853821938497887,0.27,0.125,21.0,-0.002963659372256895,0.002571759825696373,-0.0057556059011028985,0.005107055630373322
-2.853821938497887,0.33,0.125,43.0,-0.0016034543271269822,0.0016932106027591287,-0.003164937861804034,0.0034995822260505175
-2.853821938497887,0.39,0.125,42.0,-0.0019479408674224468,0.0018344144221090922,-0.0036664940075319895,0.0037516869772717294
-2.853821938497887,0.45,0.125,51.0,-0.0019605839153634882,0.0018134881479077091,-0.00371078684805194,0.00376294975365416
-2.853821938497887,0.51,0.125,46.0,-0.0020208987236843695,0.0018613774508952697,-0.003837850115069973,0.0036290870936899096
-2.853821938497887,0.57,0.125,53.0,-0.0017874127808804512,0.0017413359734623753,-0.0035298819089558944,0.003501259383526329
-2.853821938497887,0.63,0.125,86.0,-0.0013053363380135952,0.001229181697348311,-0.002630907761449195,0.0024607803359234645
-2.853821938497887,0.69,0.125,104.0,-0.0009157569646265297,0.0009170302817752346,-0.0017743405036831465,0.0018261393764041828
-2.853821938497887,0.75,0.125,40.0,-0.0012431219561483675,0.001308763524547681,-0.002515936326331621,0.0025789940192707957
-3.625650476828117,0.21,0.125,17.0,-0.002104393314219049,0.0021468920326416616,-0.0039298574735420035,0.004453377770637674
-3.625650476828117,0.27,0.125,29.0,-0.002225028975250296,0.0021378243192039306,-0.004693528218952512,0.0039170137562035525
-3.625650476828117,0.33,0.125,44.0,-0.0015140981843047953,0.0015483362425954925,-0.0028505877983367347,0.0030702475683143265
-3.625650476828117,0.39,0.125,51.0,-0.0017064020820752549,0.0018205940275750124,-0.0032592038677985774,0.003564755837676644
-3.625650476828117,0.45,0.125,54.0,-0.001790997332763887,0.0017452659059991509,-0.003623533180673438,0.0034101218106378506
-3.625650476828117,0.51,0.125,55.0,-0.0019366424653614388,0.0018754820316533153,-0.0038335211431349417,0.003578176898858079
-3.625650476828117,0.57,0.125,36.0,-0.0020812039574631728,0.0022594828156786186,-0.0041315066234181045,0.004256769932651201
-3.625650476828117,0.63,0.125,78.0,-0.001348636370543375,0.0012586326190826176,-0.002573442028124835,0.002651067311254084
-3.625650476828117,0.69,0.125,104.0,-0.0009664293227921647,0.0010308599604803028,-0.001955546861008833,0.001979869652711855
-3.625650476828117,0.75,0.125,28.0,-0.0015285341860870555,0.0015137057358222414,-0.0030197153130753743,0.00312819451321876
-4.606223395648529,0.15,0.125,5.0,-0.0030482484463399957,0.002566948205317532,-0.006263220208400933,0.004208406381043761
-4.606223395648529,0.21,0.125,24.0,-0.0017739522348530616,0.0015396776349532704,-0.0034400051860597057,0.0030901596685572784
-4.606223395648529,0.27,0.125,33.0,-0.002194889058446208,0.00214592796010037,-0.004305743128153702,0.004102324898448116
-4.606223395648529,0.33,0.125,53.0,-0.0016317595047880668,0.0016342901834841598,-0.003246271992560587,0.0031590846896880904
-4.606223395648529,0.39,0.125,51.0,-0.0020096566060357765,0.0020558764297701148,-0.0041605579361994,0.003926583188978505
-4.606223395648529,0.45,0.125,50.0,-0.0019359902578603538,0.0019382807781595356,-0.004085039953526133,0.003577231861566539
-4.606223395648529,0.51,0.125,53.0,-0.0023677821577155604,0.0022594006278851323,-0.004768742661269011,0.004426521792330549
-4.606223395648529,0.57,0.125,44.0,-0.002061733550342153,0.0021881040149233292,-0.004019407003178156,0.004220812451752894
-4.606223395648529,0.63,0.125,87.0,-0.0015881904150339382,0.001618894723277947,-0.003103400668451458,0.0030183089873026397
-4.606223395648529,0.69,0.125,83.0,-0.0012580473606010449,0.001246849143015634,-0.0024078641060933373,0.0025047457738575545
-4.606223395648529,0.75,0.125,17.0,-0.0024513920653226745,0.002237489510192897,-0.0049893607505602285,0.004334734546062012
-5.851996519306433,0.15,0.125,8.0,-0.002525260731453177,0.0022894455621576826,-0.0050559961243674505,0.0045628579883780895
-5.851996519306433,0.21,0.125,28.0,-0.001853877137496286,0.001918922445402699,-0.0037828982833392646,0.0037206046246690302
-5.851996519306433,0.27,0.125,41.0,-0.002167946700371512,0.0020028990930626754,-0.004067855378490244,0.004087281387972906
-5.851996519306433,0.33,0.125,58.0,-0.0016918352171216883,0.0016860022349161406,-0.003218769075962361,0.0033617349632793195
-5.851996519306433,0.39,0.125,51.0,-0.0020249110117310375,0.0021416567300183522,-0.004119068843264812,0.004082854681511026
-5.851996519306433,0.45,0.125,58.0,-0.002024512965373257,0.0020194689791475716,-0.00411581301388127,0.003918942666389203
-5.851996519306433,0.51,0.125,41.0,-0.003247053027598217,0.0030856751024142585,-0.006424228406950964,0.005925685025407412
-5.851996519306433,0.57,0.125,58.0,-0.0020734170760463226,0.0019446864818327787,-0.004149370146391817,0.0038418325411095
-5.851996519306433,0.63,0.125,87.0,-0.0017719190137098777,0.0018317056027408465,-0.003524946315263129,0.003584078484448697
-5.851996519306433,0.69,0.125,59.0,-0.001648348810117767,0.0017496378664904803,-0.003214570478090373,0.003525235855077035
-5.851996519306433,0.75,0.125,11.0,-0.0028487516206241363,0.002465819778127549,-0.00571941388891312,0.0048151856266097715
-7.434694395049632,0.15,0.125,12.0,-0.002316967111229576,0.002663454722153437,-0.004456195425962533,0.005337123527284933
-7.434694395049632,0.21,0.125,36.0,-0.0022321425739554265,0.0021300254563346816,-0.004460285743432145,0.004178601287300926
-7.434694395049632,0.27,0.125,57.0,-0.0019416421683150218,0.001669071628395623,-0.0038393532657446335,0.003330686348157914
-7.434694395049632,0.33,0.125,54.0,-0.0019285958354445312,0.0020169812340091273,-0.0038799194445493217,0.0038051535319937576
-7.434694395049632,0.39,0.125,59.0,-0.002101262018371296,0.0020227749533245024,-0.004241110214423467,0.0039739391237913575
-7.434694395049632,0.45,0.125,51.0,-0.0024655317793506747,0.0022937298157057304,-0.004801192632851776,0.004659838180323039
-7.434694395049632,0.51,0.125,44.0,-0.002565313938409461,0.002308247467359179,-0.004958999098885732,0.004387764088012652
-7.434694395049632,0.57,0.125,60.0,-0.00219695855631838,0.0020221688743087365,-0.004079885225095901,0.004243675278305712
-7.434694395049632,0.63,0.125,77.0,-0.002149776387532953,0.0020586130764848796,-0.004303094929490763,0.0040293678675872675
-7.434694395049632,0.69,0.125,44.0,-0.0025731861186041195,0.002641529133181291,-0.005061684568960203,0.005298515406038391
-7.434694395049632,0.75,0.125,6.0,-0.005964969677371256,0.0045391187677211,-0.01200844615775065,0.008303342456155273
-9.445439785451784,0.15,0.125,18.0,-0.002086007563739442,0.0017630058778724778,-0.004297051064462454,0.0034005129054135775
-9.445439785451784,0.21,0.125,37.0,-0.0022848155985122323,0.0022299708445950757,-0.004520355524068371,0.0041942102670364575
-9.445439785451784,0.27,0.125,59.0,-0.0020274663284244304,0.001959128942299386,-0.004158243673927659,0.0037635088357746245
-9.445439785451784,0.33,0.125,72.0,-0.0018030934599743932,0.0018572647668772607,-0.003629121861350949,0.0036515042366031133
-9.445439785451784,0.39,0.125,59.0,-0.0022432755497044355,0.002311351269081967,-0.004382863263904393,0.004450740775398969
-9.445439785451784,0.45,0.125,50.0,-0.0024395501093705018,0.0022287448170006654,-0.004970668387211447,0.0045107626282823825
-9.445439785451784,0.51,0.125,57.0,-0.0024169134381909663,0.0025952539325585274,-0.0046936485530837705,0.005159631728088683
-9.445439785451784,0.57,0.125,63.0,-0.0022690378896402046,0.0023489223324413278,-0.004949572489276654,0.0043727106735844175
-9.445439785451784,0.63,0.125,62.0,-0.002461512007053452,0.002405389570522694,-0.004869059490541024,0.0046284732860328425
-9.445439785451784,0.69,0.125,18.0,-0.004326594297210998,0.0039127047804995855,-0.009330914093954527,0.007068561919573731
-9.445439785451784,0.75,0.125,5.0,-0.0026668355868777267,0.002916493075061587,-0.004245415378540552,0.0064903397904440665
-11.99999999999999,0.15,0.125,22.0,-0.0019588125689458604,0.001613853743618034,-0.0038769865066304015,0.0031927896915342814
-11.99999999999999,0.21,0.125,43.0,-0.0024054470405516664,0.002435760739479564,-0.004646320687560408,0.004831690627762111
-11.99999999999999,0.27,0.125,64.0,-0.002557769653239398,0.0026924797063154152,-0.005227504430117062,0.005099769863980014
-11.99999999999999,0.33,0.125,81.0,-0.0017619818128866774,0.001932672749009068,-0.003566166502823257,0.0038155608512925533
-11.99999999999999,0.39,0.125,58.0,-0.002318832781279818,0.0021909125198448856,-0.004545819420498373,0.004369944512517422
-11.99999999999999,0.45,0.125,67.0,-0.0026667461788799684,0.002566168847187672,-0.005117885120752952,0.0051470826899443125
-11.99999999999999,0.51,0.125,47.0,-0.0038491278947167186,0.004071689745716921,-0.0077376620100563,0.007658444725475687
-11.99999999999999,0.57,0.125,54.0,-0.00339879450747624,0.0035676334097405407,-0.006748778432862965,0.0071013584621474266
-11.99999999999999,0.63,0.125,42.0,-0.0038711893775301683,0.004056902536170182,-0.007451545980220858,0.008055079241292788
-11.99999999999999,0.69,0.125,16.0,-0.006650220741073151,0.007331035740352364,-0.012995588017222065,0.014546667701990404
-11.99999999999999,0.81,0.125,5.0,-0.004911658259343321,0.0052277157067551535,-0.008240860554047113,0.010812034445113871
-0.1000000000000059,0.21,0.5,13.0,-0.00014273438308895058,0.0001302529136328698,-0.00028830768551246663,0.0002544998645326558
-0.1000000000000059,0.27,0.5,20.0,-0.00011774074482697761,0.00010151428820563849,-0.0002351542589370183,0.00019711124757280796
-0.1000000000000059,0.33,0.5,31.0,-0.00010605602074269925,0.00013504140900073367,-0.00020875547388432116,0.00028065477427182274
-0.1000000000000059,0.39,0.5,48.0,-7.345221812451572e-05,9.934412624849327e-05,-0.00013424804663996935,0.00020224654921120898
-0.1000000000000059,0.45,0.5,41.0,-0.00010036980253703168,0.00012479371819955757,-0.0001858069466967457,0.0002584186254104971
-0.1000000000000059,0.51,0.5,46.0,-7.448040020352802e-05,9.703967648052773e-05,-0.00013667172141306765,0.0002118831777282503
-0.1000000000000059,0.57,0.5,44.0,-0.0001018487598717579,0.00011628486792561705,-0.00019271081001232703,0.000241091602252401
-0.1000000000000059,0.63,0.5,47.0,-9.138966885250424e-05,0.00010964414464843484,-0.00017849920550754543,0.00022500780943488123
-0.1000000000000059,0.69,0.5,105.0,-5.504930670352739e-05,6.031716191171108e-05,-0.00010204621997746495,0.00012314025241949564
-0.1000000000000059,0.75,0.5,93.0,-7.517119209203168e-05,8.495281379953901e-05,-0.00015679972772205132,0.00015820719427353758
-0.1000000000000059,0.81,0.5,11.0,-0.00032763484945752633,0.00016193891325503706,-0.0006722894543305085,0.00017390490260588644
-0.1270454343320682,0.21,0.5,13.0,-0.0002333655003687856,0.00021767372290573892,-0.0004647428999981833,0.0004162627709477979
-0.1270454343320682,0.27,0.5,20.0,-0.00018371982640130142,0.00016835971861366183,-0.0003710833341054043,0.0003165214643149215
-0.1270454343320682,0.33,0.5,31.0,-0.00014575808429728582,0.00015929889489173896,-0.00027589896930770523,0.0003325843767190239
-0.1270454343320682,0.39,0.5,48.0,-9.354559394759621e-05,0.0001152147651707886,-0.00018068695060193283,0.00023586772956955896
-0.1270454343320682,0.45,0.5,41.0,-0.00012017930770686123,0.00014486561147579788,-0.0002262765101096833,0.00030402322409835977
-0.1270454343320682,0.51,0.5,47.0,-8.159645192385001e-05,0.00011495490506293094,-0.00015615146734032582,0.00023568024719091253
-0.1270454343320682,0.57,0.5,44.0,-0.00010931118844142811,0.00012980806660553074,-0.0002113378869245785,0.00025886562722145283
-0.1270454343320682,0.63,0.5,47.0,-9.823240576404543e-05,0.00011255104930796636,-0.00019126877649639978,0.00023426402560480398
-0.1270454343320682,0.69,0.5,104.0,-5.478664180085971e-05,6.606024574583568e-05,-0.00010370937607783067,0.00013258118696572155
-0.1270454343320682,0.75,0.5,93.0,-7.436935086188899e-05,8.342832624782414e-05,-0.00015378768889420447,0.0001632042878522723
-0.1270454343320682,0.81,0.5,11.0,-0.00032708095723104366,0.00016016025540460888,-0.0006751703098478393,0.00017835554502416588
-0.1614054238462196,0.21,0.5,13.0,-0.0003743950055082827,0.00037722796116663196,-0.0007368753455066148,0.0007049446809624866
-0.1614054238462196,0.27,0.5,20.0,-0.0003129999421773189,0.0002643111691894804,-0.0005952431961083599,0.0005469522915321492
-0.1614054238462196,0.33,0.5,31.0,-0.00020692661876177155,0.00022735118330911435,-0.00041163493104042723,0.0004418976897603544
-0.1614054238462196,0.39,0.5,48.0,-0.0001334294369827447,0.00016063564986350978,-0.00025292100103748523,0.0003293015664647702
-0.1614054238462196,0.45,0.5,41.0,-0.00016027367465279208,0.00019601629525498217,-0.00031663969654963634,0.00038245347710267615
-0.1614054238462196,0.51,0.5,47.0,-0.00011200791143326054,0.00013791946191090928,-0.0002071922357743812,0.0002828009795136146
-0.1614054238462196,0.57,0.5,44.0,-0.00013995028827892454,0.00014566988780997627,-0.0002575195183579822,0.0003121586881860581
-0.1614054238462196,0.63,0.5,48.0,-0.00010948340527213244,0.0001428473930985703,-0.000222262548138139,0.00026987335575644894
-0.1614054238462196,0.69,0.5,103.0,-6.230601321055069e-05,7.222666378631448e-05,-0.00012150021796869146,0.00015105383670961387
-0.1614054238462196,0.75,0.5,93.0,-8.629267902188927e-05,8.810872442487757e-05,-0.00016333878199224026,0.00017912808844872832
-0.1614054238462196,0.81,0.5,11.0,-0.00033341147062202495,0.0001664045744997998,-0.0007232700471174879,0.00019267552612643109
-0.2050582217609179,0.21,0.5,13.0,-0.0006011067270412603,0.0006072824582183042,-0.0011958483408374102,0.001186746459000254
-0.2050582217609179,0.27,0.5,21.0,-0.0005016216455353085,0.0004384178368340079,-0.0009415591001316109,0.0008607721573909083
-0.2050582217609179,0.33,0.5,31.0,-0.0003471733551253584,0.0003445596409664231,-0.0006873389400705271,0.00068794871522558
-0.2050582217609179,0.39,0.5,47.0,-0.00020755000544596259,0.00024926403287244935,-0.0004055108931699297,0.0004986441857058393
-0.2050582217609179,0.45,0.5,41.0,-0.00022711936947951439,0.0002948447891087141,-0.00047183843386024784,0.0005390546351776612
-0.2050582217609179,0.51,0.5,47.0,-0.0001537317602818252,0.00020080732904482782,-0.0002963926756527677,0.00040836472977243203
-0.2050582217609179,0.57,0.5,45.0,-0.00019005653713987029,0.0001978603499005472,-0.00035837135142126455,0.00041301006435389694
-0.2050582217609179,0.63,0.5,50.0,-0.0001432954714871362,0.00016677034921620907,-0.0002761562331340543,0.00033859697058782033
-0.2050582217609179,0.69,0.5,101.0,-8.169925555009792e-05,8.879998473692605e-05,-0.00015062101877093504,0.00018603938362007991
-0.2050582217609179,0.75,0.5,93.0,-0.00010336428758855145,0.00011027742700067702,-0.00020158877593047669,0.00021501523438087838
-0.2050582217609179,0.81,0.5,10.0,-0.0002522376767927066,0.00021695825251771703,-0.0009067974888987217,0.00024168474400602206
-0.2605171084697261,0.21,0.5,13.0,-0.0009725711358760524,0.0009430345362114429,-0.001874686243664846,0.0018928746393323888
-0.2605171084697261,0.27,0.5,21.0,-0.0008247834134521072,0.0007198706511268579,-0.0015865569541846389,0.0013871356427995881
-0.2605171084697261,0.33,0.5,31.0,-0.0005346243252607463,0.0004966858490440175,-0.0010726142311993454,0.0009705794291844864
-0.2605171084697261,0.39,0.5,49.0,-0.00030343423073317215,0.0003383885678134968,-0.0005981277164305796,0.0006474626925064074
-0.2605171084697261,0.45,0.5,39.0,-0.00035761357839222626,0.0003744580738467007,-0.0006891822595661114,0.000747232908019974
-0.2605171084697261,0.51,0.5,47.0,-0.00021169474109156342,0.000245956595494451,-0.0004037692558607926,0.0005078353031221731
-0.2605171084697261,0.57,0.5,49.0,-0.0002128178569692044,0.00023942566255887238,-0.0004096279661269546,0.000474158563742505
-0.2605171084697261,0.63,0.5,53.0,-0.00015879488680598213,0.00018104170517242087,-0.0003041827086491653,0.0003770542771605729
-0.2605171084697261,0.69,0.5,94.0,-9.983966184847196e-05,0.00010903980302828343,-0.00019179143921101895,0.0002208834853624889
-0.2605171084697261,0.75,0.5,93.0,-0.00011269784919683053,0.00011634250718250867,-0.00021877126988571294,0.0002363002820628569
-0.2605171084697261,0.81,0.5,10.0,-0.0002906790362088966,0.00023567157524257912,-0.0009813810836753944,0.0002707306392458919
-0.3309750919646838,0.21,0.5,13.0,-0.0014503022983812029,0.0014539109040231034,-0.0029973305486695467,0.002710220768962567
-0.3309750919646838,0.27,0.5,22.0,-0.0011619814552403076,0.0010739993861873835,-0.0024014921428352778,0.002092449657621717
-0.3309750919646838,0.33,0.5,31.0,-0.0008566282723191211,0.0007383584287452341,-0.001762633919882602,0.0014247293571741288
-0.3309750919646838,0.39,0.5,48.0,-0.0004930024335128735,0.000496274250650043,-0.0009416608534898701,0.0010048052646724874
-0.3309750919646838,0.45,0.5,40.0,-0.0005044087631216901,0.0005137823739895755,-0.000982824113149032,0.0009988848509585105
-0.3309750919646838,0.51,0.5,47.0,-0.00029896671882382805,0.0003428442206836818,-0.0005826559213904255,0.0006783789040469794
-0.3309750919646838,0.57,0.5,51.0,-0.000280601416535489,0.0003117148277335281,-0.0005558679006944168,0.0006053496058312076
-0.3309750919646838,0.63,0.5,53.0,-0.00019709582417346433,0.00023718524747014992,-0.0003950348585586703,0.00047982785701967983
-0.3309750919646838,0.69,0.5,94.0,-0.00012553392968839297,0.00013633483044003632,-0.00024307194258300983,0.00027470143660164457
-0.3309750919646838,0.75,0.5,90.0,-0.00013652369828997404,0.00013886118331529746,-0.00026243034291109743,0.0002776783618620164
-0.3309750919646838,0.81,0.5,10.0,-0.00033033353466724183,0.0002561519141051192,-0.0010779346384933563,0.0003048474194650083
-0.4204887431174444,0.21,0.5,13.0,-0.0021846943588377287,0.0020214439190424675,-0.004371940827083146,0.0038305520162810096
-0.4204887431174444,0.27,0.5,21.0,-0.0018268997127383292,0.0014335485226440348,-0.0035500963666664008,0.002835419662888346
-0.4204887431174444,0.33,0.5,32.0,-0.001296930622205543,0.0010810547314393276,-0.002622796934110658,0.002110478048214015
-0.4204887431174444,0.39,0.5,48.0,-0.0007183629843176268,0.0007640373167999993,-0.0014259244688965792,0.001425929672302039
-0.4204887431174444,0.45,0.5,40.0,-0.0007259241123925851,0.0007353701645069385,-0.0014629241660133329,0.0014214816151098468
-0.4204887431174444,0.51,0.5,49.0,-0.00045102716804723894,0.00044270353889794896,-0.0008329155176773392,0.0008959802758976583
-0.4204887431174444,0.57,0.5,51.0,-0.00039581293976051674,0.0004131800466804705,-0.0007903160388009246,0.0008285591115938472
-0.4204887431174444,0.63,0.5,56.0,-0.0002794779372273453,0.0003102531480348496,-0.0005292903142948764,0.0006440812982090559
-0.4204887431174444,0.69,0.5,90.0,-0.000162935601103639,0.00017954445846163968,-0.0003200254268728609,0.0003599129133099921
-0.4204887431174444,0.75,0.5,89.0,-0.00017302352346798734,0.0001715138256654073,-0.0003257805660998272,0.0003484854638733239
-0.4204887431174444,0.81,0.5,10.0,-0.0003815193811698154,0.0002884733505256931,-0.0010308080713778505,0.0003521898002542389
-0.5342117500109873,0.21,0.5,13.0,-0.0030049570657390712,0.0026800404964980114,-0.006202494403408698,0.005138406981122657
-0.5342117500109873,0.27,0.5,23.0,-0.002237637073776345,0.0020378775740974944,-0.0046489843421917585,0.003975803117377897
-0.5342117500109873,0.33,0.5,32.0,-0.0018172491179409926,0.0015529574221532301,-0.0037634695339409077,0.0028943339100672718
-0.5342117500109873,0.39,0.5,46.0,-0.001058831182236385,0.0010702337423094152,-0.0021692677762362267,0.002062079899825079
-0.5342117500109873,0.45,0.5,41.0,-0.0010406800769433002,0.0010234667208379189,-0.002051763313921818,0.0019343409568594154
-0.5342117500109873,0.51,0.5,49.0,-0.0006192565652545168,0.0006185414346319121,-0.0012299259382999599,0.0012890290671611544
-0.5342117500109873,0.57,0.5,51.0,-0.0005432507452735063,0.0005744657153677173,-0.0010528087052296153,0.0011213406196667335
-0.5342117500109873,0.63,0.5,58.0,-0.00037856104052126654,0.0004300487401793154,-0.00074096061830213,0.0008648281033352318
-0.5342117500109873,0.69,0.5,88.0,-0.00023493592883335889,0.00023348525108513377,-0.0004580024468035833,0.00046942602477696656
-0.5342117500109873,0.75,0.5,87.0,-0.00022876938822912594,0.00023105221521524906,-0.00045133497737932836,0.00047349872086204767
-0.5342117500109873,0.81,0.5,11.0,-0.000651165741394258,0.0003621751753758085,-0.0013315915234395012,0.0006835405940412245
-0.6786916380543186,0.21,0.5,13.0,-0.003608582742480704,0.0031058365636833342,-0.007059910332707162,0.006028406776178488
-0.6786916380543186,0.27,0.5,23.0,-0.0029792650701511865,0.0026314752804842507,-0.005905948487282223,0.005011275411902972
-0.6786916380543186,0.33,0.5,34.0,-0.002267492015505755,0.0019271548650390583,-0.004906363815884016,0.0035433437670778136
-0.6786916380543186,0.39,0.5,47.0,-0.0014014564178132646,0.0013935297408449775,-0.002836149955453131,0.0025911636022853276
-0.6786916380543186,0.45,0.5,42.0,-0.001367021435805584,0.001246451793251554,-0.002696968652411515,0.0024369901533955875
-0.6786916380543186,0.51,0.5,46.0,-0.0009129528056857825,0.0008528351939187627,-0.0018166526391517788,0.0016676768209349605
-0.6786916380543186,0.57,0.5,52.0,-0.0007309295744978647,0.0007404536010465325,-0.001452590977547052,0.0014569077184530246
-0.6786916380543186,0.63,0.5,57.0,-0.0005037701627167559,0.000545236947068431,-0.0009478311058105212,0.001093675092720839
-0.6786916380543186,0.69,0.5,89.0,-0.0002947961389443588,0.0003239838703783315,-0.0005720263995263157,0.0006354777120903683
-0.6786916380543186,0.75,0.5,85.0,-0.00033068590213117,0.0003281826783867227,-0.0006538317277268218,0.0006399884207942321
-0.6786916380543186,0.81,0.5,11.0,-0.0009521419499269641,0.0005200687894574893,-0.0019755347919955583,0.0009989537940948208
-0.8622467393414629,0.21,0.5,14.0,-0.0037907557219618213,0.0033022474372735385,-0.007662598470736291,0.006182367495680096
-0.8622467393414629,0.27,0.5,22.0,-0.0033736421106991877,0.003225129282385415,-0.007076770626800428,0.006128249028367606
-0.8622467393414629,0.33,0.5,36.0,-0.002745809885717543,0.0022888129692207413,-0.005633728672520377,0.004334068749467275
-0.8622467393414629,0.39,0.5,46.0,-0.001590605386088863,0.0015625976197716288,-0.00327009603932575,0.002879711732467736
-0.8622467393414629,0.45,0.5,42.0,-0.0016263278500994144,0.001556230012622043,-0.003246373635671121,0.003067407300809865
-0.8622467393414629,0.51,0.5,46.0,-0.0012070513974184493,0.0010811999204827483,-0.002399818113426165,0.002162340059407504
-0.8622467393414629,0.57,0.5,55.0,-0.0008834196513700394,0.0008996613136313584,-0.001691810502157425,0.0017709745775498391
-0.8622467393414629,0.63,0.5,56.0,-0.0006669961176581437,0.0006800176104751758,-0.0012934158387323154,0.0013659404833193838
-0.8622467393414629,0.69,0.5,86.0,-0.0004153320886589606,0.0004585652531509016,-0.0008199714307190199,0.0008714528495290225
-0.8622467393414629,0.75,0.5,85.0,-0.0004608920321795848,0.0004545259744215724,-0.0009006706437607486,0.0008998886582345207
-0.8622467393414629,0.81,0.5,11.0,-0.0014534294927071672,0.000757051607366717,-0.0028959496188997636,0.0014909785410001702
-1.095445115010322,0.21,0.5,14.0,-0.003713769103745442,0.003426829440694676,-0.007224897658663633,0.006813495663461056
-1.095445115010322,0.27,0.5,25.0,-0.0031766519153149987,0.003060375732982055,-0.006568781674505515,0.005792580641249841
-1.095445115010322,0.33,0.5,35.0,-0.003114673930920303,0.002619482482734638,-0.006187935625487511,0.004887579268097844
-1.095445115010322,0.39,0.5,48.0,-0.001813018793389536,0.0016818172168871718,-0.0035915669867921485,0.0033592371924402024
-1.095445115010322,0.45,0.5,41.0,-0.0020589381533656303,0.0019420722039976343,-0.0041727243392928265,0.0036911118960346032
-1.095445115010322,0.51,0.5,47.0,-0.0014765395758803818,0.0014064824859820054,-0.0030686249841993403,0.002638326117574532
-1.095445115010322,0.57,0.5,56.0,-0.0010759462307398545,0.0011170176981499607,-0.0021079426767362775,0.0022483207997993212
-1.095445115010322,0.63,0.5,58.0,-0.0008530344863541745,0.0008725365162723512,-0.0016730476961210384,0.0016936295294308502
-1.095445115010322,0.69,0.5,83.0,-0.0005734706396952396,0.0005880863749776564,-0.00113034477919725,0.0011758791538555994
-1.095445115010322,0.75,0.5,84.0,-0.0006630486038701704,0.0006563170935264974,-0.0013371376566339269,0.0012613789592073135
-1.095445115010322,0.81,0.5,8.0,-0.0015254726488190269,0.0012556559923294075,-0.004199835095035705,0.0014730609230853388
-1.3917130042341714,0.21,0.5,13.0,-0.003497629579469432,0.003462367586153945,-0.006763953079246958,0.006688718584659641
-1.3917130042341714,0.27,0.5,27.0,-0.0029597371652509133,0.0027374623508487138,-0.005835611746933603,0.005260327493681427
-1.3917130042341714,0.33,0.5,33.0,-0.003103753459813891,0.002575495826361907,-0.005905739208103298,0.005215961000313725
-1.3917130042341714,0.39,0.5,53.0,-0.0018183316489164345,0.0015643666989038345,-0.0036191604998988447,0.0031570876561814436
-1.3917130042341714,0.45,0.5,45.0,-0.0022244384420843275,0.0019211153830974946,-0.004428694026326965,0.003918612223459926
-1.3917130042341714,0.51,0.5,50.0,-0.0016813292753027136,0.0016564273388848024,-0.003541084843364606,0.003106878421865583
-1.3917130042341714,0.57,0.5,54.0,-0.0012403101567512557,0.0011991050480530951,-0.002475799481950467,0.0023382458376997885
-1.3917130042341714,0.63,0.5,55.0,-0.0009892946049855043,0.001002993592669964,-0.001990712963767725,0.0019317488915931598
-1.3917130042341714,0.69,0.5,93.0,-0.0006847260219185513,0.0007137059627605514,-0.0013691267714473583,0.0013910669794202236
-1.3917130042341714,0.75,0.5,69.0,-0.0008970790626261258,0.0008896112456278029,-0.0018333529147583501,0.0016011235113571286
-1.3917130042341714,0.81,0.5,6.0,-0.00020381653295881152,0.00018013805203152358,-0.00041621094285954063,0.000365022195934465
-1.7681078308849811,0.21,0.5,15.0,-0.0027063974201646445,0.0029115611750143646,-0.005803688036341948,0.005389237244346988
-1.7681078308849811,0.27,0.5,31.0,-0.003004677081525545,0.0026434222502494564,-0.005807858287726393,0.005329548398386943
-1.7681078308849811,0.33,0.5,34.0,-0.0023472882850410406,0.0024018395639840893,-0.004569511213440928,0.004704513468805876
-1.7681078308849811,0.39,0.5,53.0,-0.00184015528306438,0.0016949762431230457,-0.0036578254583847884,0.0034436099612887012
-1.7681078308849811,0.45,0.5,52.0,-0.002093607554332555,0.0018584456167115972,-0.004078195732602852,0.0037321821598677346
-1.7681078308849811,0.51,0.5,50.0,-0.001714880103914197,0.0016207270968787628,-0.003524885202247562,0.0030671214704405783
-1.7681078308849811,0.57,0.5,49.0,-0.0016092249891937341,0.001532932772872372,-0.003333060887231426,0.0028768185301208146
-1.7681078308849811,0.63,0.5,62.0,-0.0009827112461699959,0.0008729316643290736,-0.0018666848683008945,0.0017394707898848532
-1.7681078308849811,0.69,0.5,101.0,-0.0007881025341953129,0.0007750802123209996,-0.0015590771581554905,0.0015382859840865739
-1.7681078308849811,0.75,0.5,47.0,-0.001234528780485752,0.0010475909413440233,-0.002481770223481391,0.0019627801439203937
-2.2463002732069244,0.21,0.5,15.0,-0.0035384739360796854,0.0034522674433159067,-0.006970092748712547,0.006513067132772179
-2.2463002732069244,0.27,0.5,34.0,-0.00243222805144322,0.002353474905649299,-0.005066314438548068,0.004479657901764691
-2.2463002732069244,0.33,0.5,39.0,-0.002147490176943587,0.0020861794397246587,-0.004200274762947214,0.004114968194911307
-2.2463002732069244,0.39,0.5,49.0,-0.0021877829277298843,0.0020817459779011783,-0.004130406857808727,0.004201465569591405
-2.2463002732069244,0.45,0.5,56.0,-0.0018591765135110348,0.0017190621330730402,-0.0036310635273293754,0.003396688548497635
-2.2463002732069244,0.51,0.5,52.0,-0.0021777373522371404,0.0019170597841970361,-0.004476085396164821,0.003672589684831511
-2.2463002732069244,0.57,0.5,47.0,-0.0017401506129240782,0.001684567727871602,-0.0035098487614830727,0.0032429889677974
-2.2463002732069244,0.63,0.5,67.0,-0.0009966449283174167,0.00098810019031843,-0.0020856046706312936,0.0018828342038325974
-2.2463002732069244,0.69,0.5,99.0,-0.0009363176072917449,0.0008675535735238192,-0.0018536299320959467,0.0017226393132689813
-2.2463002732069244,0.75,0.5,37.0,-0.0014531757371499367,0.0011814830919410087,-0.0029871638508719425,0.0022609477493718217
-2.8538219384978865,0.15,0.5,6.0,-0.0050237851107686575,0.0037135804375423485,-0.009827702341939212,0.007164613687778672
-2.8538219384978865,0.21,0.5,16.0,-0.002853418160550156,0.0029570986972543307,-0.00569101105891383,0.005513075934458912
-2.8538219384978865,0.27,0.5,33.0,-0.0021805334061820066,0.00232708961932013,-0.004571176045841824,0.004392675498400804
-2.8538219384978865,0.33,0.5,47.0,-0.0017619240704671456,0.0017330247348994667,-0.0035345288773504777,0.0033843936562837343
-2.8538219384978865,0.39,0.5,50.0,-0.002162237600803659,0.0021162723325340994,-0.004390721847010702,0.004051801888549703
-2.8538219384978865,0.45,0.5,53.0,-0.001927909844856407,0.0018543184958625808,-0.003954095034544547,0.0034723768306622565
-2.8538219384978865,0.51,0.5,55.0,-0.001998813837551515,0.0017859039384381886,-0.00394640156974858,0.00343357982240534
-2.8538219384978865,0.57,0.5,44.0,-0.0015823905263760128,0.001500968387161953,-0.00309216517669721,0.00302462456956794
-2.8538219384978865,0.63,0.5,67.0,-0.0012132497569496675,0.0011282594061474463,-0.0024143862062487925,0.00217406656058609
-2.8538219384978865,0.69,0.5,98.0,-0.0011181700494453327,0.001083655935135772,-0.0022564835580158676,0.0020752841838183747
-2.8538219384978865,0.75,0.5,30.0,-0.0019291165321035065,0.0015489799579923766,-0.004043830978569563,0.002848203287645919
-3.625650476828113,0.15,0.5,9.0,-0.0019430197007592096,0.0018345990724293088,-0.003636450796218542,0.0037753144826912065
-3.625650476828113,0.21,0.5,17.0,-0.0021726296747053104,0.0021426421139319547,-0.0040504353418184666,0.004183301744519337
-3.625650476828113,0.27,0.5,36.0,-0.0020760159478808945,0.001768388447638759,-0.004120769268699206,0.0034559299307562906
-3.625650476828113,0.33,0.5,58.0,-0.0014118266262340285,0.0013412897607668146,-0.002835082139341902,0.0025733713302183727
-3.625650476828113,0.39,0.5,49.0,-0.001949649486038693,0.001821252026066761,-0.0038811822522180784,0.0034598272096696856
-3.625650476828113,0.45,0.5,52.0,-0.0013688604946892084,0.0013034068753343367,-0.0028425061658465707,0.002459038193614964
-3.625650476828113,0.51,0.5,47.0,-0.0012998772753843651,0.0013570090705828505,-0.0025124633927570833,0.0026668303748691438
-3.625650476828113,0.57,0.5,44.0,-0.0018408514111250167,0.0018855123803898728,-0.003625297567016616,0.0036303374431223916
-3.625650476828113,0.63,0.5,67.0,-0.0014263391053574775,0.001320325256216309,-0.002735043701224357,0.002614466436337649
-3.625650476828113,0.69,0.5,95.0,-0.0012053630469018224,0.0011577340288752454,-0.002431955503125835,0.0022177405462518187
-3.625650476828113,0.75,0.5,26.0,-0.0031128305666626188,0.0027362696585593255,-0.006032878301460396,0.005245292617093227
-4.606223395648544,0.15,0.5,9.0,-0.0020290920179027467,0.0022479090426050807,-0.003935499239247082,0.0042269954258480095
-4.606223395648544,0.21,0.5,22.0,-0.0016092609863309275,0.0018217573469247147,-0.0030368665477417687,0.0034810774028864455
-4.606223395648544,0.27,0.5,41.0,-0.001936794313917049,0.001838380513578298,-0.004080819658674616,0.003394378132787906
-4.606223395648544,0.33,0.5,54.0,-0.0014570144934368762,0.0014382707134788317,-0.0029663764203370444,0.002749387722668662
-4.606223395648544,0.39,0.5,53.0,-0.001662962602184345,0.0014615200938622815,-0.0031263072223046756,0.00302564261066826
-4.606223395648544,0.45,0.5,55.0,-0.001274258179415006,0.0011911599157586766,-0.0024401282363970714,0.0022904859123887887
-4.606223395648544,0.51,0.5,41.0,-0.0016895593492838525,0.001439348375715198,-0.0034236481973304073,0.002721456806736072
-4.606223395648544,0.57,0.5,43.0,-0.0017962990410136887,0.001979544552002756,-0.0032485163617408407,0.0040024877173201676
-4.606223395648544,0.63,0.5,77.0,-0.0013484704134868529,0.0013057790989338856,-0.0028319045501885077,0.0024773663055350156
-4.606223395648544,0.69,0.5,80.0,-0.001431252529558357,0.0013085755604487661,-0.0027601369628327765,0.0025230351117377214
-4.606223395648544,0.75,0.5,23.0,-0.0033694588583261047,0.003327745016123885,-0.0065983432253673225,0.006533722664033248
-5.851996519306419,0.15,0.5,11.0,-0.0025854218445253096,0.0025466321216562997,-0.00511627746073276,0.004727368343199667
-5.851996519306419,0.21,0.5,24.0,-0.00241244732522025,0.0025976201678893428,-0.005052048257871302,0.004809988756556737
-5.851996519306419,0.27,0.5,42.0,-0.0018990156589050145,0.001930113917691042,-0.0036791091911305483,0.0038798761175057993
-5.851996519306419,0.33,0.5,52.0,-0.0014607700654165978,0.0014615049961464734,-0.002820484712998408,0.0028942558984398565
-5.851996519306419,0.39,0.5,56.0,-0.0017157376400680992,0.0014802110019677584,-0.0034972401885968764,0.0028549638885132316
-5.851996519306419,0.45,0.5,62.0,-0.0017714496012909827,0.001746863407457911,-0.003487242588627691,0.003477100127176039
-5.851996519306419,0.51,0.5,49.0,-0.0018626182576915544,0.0018321686461570768,-0.0037093201935943774,0.003570559296848282
-5.851996519306419,0.57,0.5,49.0,-0.0019119292018091982,0.0018141546126971917,-0.0038340816421633525,0.0035993052108669434
-5.851996519306419,0.63,0.5,65.0,-0.0017204321911614118,0.001667476307588819,-0.003471029037285971,0.0032163886689609783
-5.851996519306419,0.69,0.5,70.0,-0.0016333827146257664,0.0015959826461126366,-0.0031730118991739648,0.0030597643213210574
-5.851996519306419,0.75,0.5,16.0,-0.0029034575610571538,0.0028730187544554623,-0.00606097329697885,0.005333704821086075
-7.434694395049625,0.15,0.5,12.0,-0.0017426969765748181,0.0024046640805573654,-0.003077687198909975,0.0053275754549008516
-7.434694395049625,0.21,0.5,29.0,-0.0018140669948004972,0.0021270774849586603,-0.0035495019249494166,0.004332756962486341
-7.434694395049625,0.27,0.5,59.0,-0.0015118872882657515,0.0015426272941465172,-0.0030291099872410804,0.003002117631306853
-7.434694395049625,0.33,0.5,59.0,-0.0016230665169876533,0.0015083620582270127,-0.0032809084070679465,0.0028711561048927314
-7.434694395049625,0.39,0.5,52.0,-0.0018159537536259704,0.0016908532306489105,-0.003297061634223984,0.0034903399619161226
-7.434694395049625,0.45,0.5,55.0,-0.0019874175152726154,0.001905257305992066,-0.004028130306000586,0.0036783517447806077
-7.434694395049625,0.51,0.5,51.0,-0.002138260290806696,0.002152508953866227,-0.0042769239992656305,0.00415607661707985
-7.434694395049625,0.57,0.5,62.0,-0.002295495115308939,0.0023677025404466225,-0.004724068878391814,0.004446996278473745
-7.434694395049625,0.63,0.5,64.0,-0.002166425636444829,0.0019617334638863115,-0.004387013774244181,0.003774711596178671
-7.434694395049625,0.69,0.5,46.0,-0.0030941292836149854,0.0030440698222714414,-0.00620538852939444,0.005826148940598033
-7.434694395049625,0.75,0.5,7.0,-0.007127456209720074,0.005058549476491522,-0.014171408267518582,0.009763237981146408
-9.445439785451809,0.15,0.5,13.0,-0.0026405778232048717,0.0025621764358649953,-0.004806392552177996,0.005324508451263751
-9.445439785451809,0.21,0.5,36.0,-0.0022059154237096526,0.0021539624724412976,-0.004585391217273837,0.0041386550292447834
-9.445439785451809,0.27,0.5,52.0,-0.0017538915280560761,0.0017190261237836181,-0.0034400596654724737,0.0032869195327691024
-9.445439785451809,0.33,0.5,69.0,-0.0018930558311781975,0.0018870773271172938,-0.003691855537554301,0.003637423559870883
-9.445439785451809,0.39,0.5,70.0,-0.0020139646782848545,0.0020337240913234304,-0.004109908975581006,0.003897919883655943
-9.445439785451809,0.45,0.5,55.0,-0.002335216886178803,0.002155715529524289,-0.004694704518563736,0.004261437551386181
-9.445439785451809,0.51,0.5,55.0,-0.0024983347124159405,0.0026871382809096384,-0.005080703906757004,0.005045618344089717
-9.445439785451809,0.57,0.5,49.0,-0.003290452259764622,0.003192879124646918,-0.006946020340768644,0.006065712617524746
-9.445439785451809,0.63,0.5,56.0,-0.0034879514856452527,0.0033183441517858447,-0.007280995653232024,0.006199902711379483
-9.445439785451809,0.69,0.5,34.0,-0.004291329806380894,0.004387686552782385,-0.008359348755206265,0.00890876265269498
-9.445439785451809,0.75,0.5,7.0,-0.010506779040788863,0.010082277229380836,-0.021265389690583066,0.018809893198519
-12.0,0.15,0.5,14.0,-0.0026793935207218905,0.003213492641541805,-0.005456274563789138,0.005963890363673162
-12.0,0.21,0.5,38.0,-0.0016841380456188593,0.0017692007498158583,-0.003344245023057092,0.003360954432934479
-12.0,0.27,0.5,55.0,-0.0022438327112870443,0.0020991701355637985,-0.0044186718898986625,0.004072249396361926
-12.0,0.33,0.5,69.0,-0.0021471855232683204,0.0019663815733771423,-0.004121488275761761,0.0038545987361498723
-12.0,0.39,0.5,80.0,-0.0023988145232881823,0.002472883905238747,-0.004750098606724239,0.004802541782052268
-12.0,0.45,0.5,56.0,-0.0024437655434156164,0.0024735082245652407,-0.004962285108828332,0.004778131561872255
-12.0,0.51,0.5,48.0,-0.004252566484574172,0.003612427075579186,-0.008384166950334115,0.007016617105578033
-12.0,0.57,0.5,47.0,-0.005286408783520353,0.004868419503997803,-0.01074049921538768,0.009254295035842349
-12.0,0.63,0.5,44.0,-0.00614622576768963,0.005503135866665897,-0.012257528628766976,0.010585543806638386
-12.0,0.69,0.5,27.0,-0.008146269892265356,0.007557067557873869,-0.016219222250642172,0.01488935634805005
-12.0,0.75,0.5,13.0,-0.010477557562006282,0.01066832307327853,-0.021689606396166322,0.02046062472807709
-0.0999999999999897,0.21,1.0,12.0,-9.187512392304812e-05,0.0001029074018831095,-0.000173457006035472,0.00020768967271124434
-0.0999999999999897,0.27,1.0,28.0,-6.844968318314929e-05,6.395310645356863e-05,-0.0001338749069474434,0.00012377101867062088
-0.0999999999999897,0.33,1.0,35.0,-8.121799616500749e-05,6.723867856226631e-05,-0.00017146141381305539,0.00012413915168405542
-0.0999999999999897,0.39,1.0,51.0,-5.972100256133265e-05,6.846440533880991e-05,-0.00011390973317694103,0.00014229012966700675
-0.0999999999999897,0.45,1.0,50.0,-6.674473026944119e-05,8.097968545909062e-05,-0.00012594675085974633,0.00016919739989517999
-0.0999999999999897,0.51,1.0,50.0,-7.298218000785107e-05,8.29424682761849e-05,-0.00013699215066892,0.0001760639486325898
-0.0999999999999897,0.57,1.0,61.0,-6.392450769890715e-05,7.262634195924265e-05,-0.00011420705731167372,0.00014897650890932223
-0.0999999999999897,0.63,1.0,56.0,-5.238571830601745e-05,6.568655728714898e-05,-9.497095837474748e-05,0.00013075814084329622
-0.0999999999999897,0.69,1.0,91.0,-4.561599252162513e-05,5.515793076821824e-05,-8.560393684390978e-05,0.00010936825030162546
-0.0999999999999897,0.75,1.0,52.0,-8.74527571406148e-05,8.166214994756513e-05,-0.00017054789124016842,0.00016356299765493261
-0.0999999999999897,0.81,1.0,11.0,-2.7007264282818646e-06,2.6753417449543226e-06,-5.499986317116729e-06,5.241199630334542e-06
-0.1270454343320429,0.21,1.0,12.0,-0.00011834943491372754,0.00012861199095912508,-0.00021119972758423217,0.0002752941887276806
-0.1270454343320429,0.27,1.0,28.0,-0.00010337063646064728,9.284357480372996e-05,-0.00020001029317772966,0.00019049578604764621
-0.1270454343320429,0.33,1.0,35.0,-0.00012009193183228175,9.218282863636557e-05,-0.00025183265261509517,0.00017343738290844706
-0.1270454343320429,0.39,1.0,51.0,-7.22771123498105e-05,8.14645881116427e-05,-0.0001491231660431986,0.00016665299470896354
-0.1270454343320429,0.45,1.0,51.0,-7.594934287618511e-05,9.62913264997414e-05,-0.00015020636260848293,0.00018297561988115475
-0.1270454343320429,0.51,1.0,49.0,-8.242895127857867e-05,9.696662264472546e-05,-0.0001540534580225845,0.00020208507355074984
-0.1270454343320429,0.57,1.0,61.0,-6.939912855986809e-05,7.55584626049905e-05,-0.00013027450685356858,0.00016385693846375664
-0.1270454343320429,0.63,1.0,56.0,-5.4091794652324873e-05,7.017686216034358e-05,-9.980978463480275e-05,0.0001472146959134432
-0.1270454343320429,0.69,1.0,92.0,-4.737309411853203e-05,5.3473021697872057e-05,-9.051103713416994e-05,0.00010586578799213891
-0.1270454343320429,0.75,1.0,51.0,-8.876092928346201e-05,8.423289362415582e-05,-0.00016924146112859434,0.00016545203551740308
-0.1270454343320429,0.81,1.0,11.0,-3.128895721507781e-06,3.1621298806121958e-06,-6.141861554024133e-06,6.2396220754781705e-06
-0.161405423846211,0.21,1.0,12.0,-0.00016668410898636706,0.00019947403410088926,-0.00031886786396315814,0.0003910882422300894
-0.161405423846211,0.27,1.0,28.0,-0.00016155216666112414,0.0001608172099277878,-0.0003265547253361056,0.0003089621895217048
-0.161405423846211,0.33,1.0,35.0,-0.00018094196086404962,0.00013851348862527573,-0.00037916471171753455,0.00026468691505962923
-0.161405423846211,0.39,1.0,51.0,-0.00010936014087025133,0.00011277855140261683,-0.00021702644606859015,0.0002216678987852989
-0.161405423846211,0.45,1.0,51.0,-0.00010883116809028726,0.0001158712774405398,-0.0002094315170496724,0.0002404612887540724
-0.161405423846211,0.51,1.0,52.0,-0.00010094878037896416,0.00012073473974752021,-0.0001972021467267084,0.00023586455172472539
-0.161405423846211,0.57,1.0,58.0,-7.955205640114335e-05,9.867308324366414e-05,-0.00015592251357815574,0.00019375154140955812
-0.161405423846211,0.63,1.0,58.0,-6.342224865629658e-05,7.866698270508206e-05,-0.00012074750795899288,0.00015998848887942285
-0.161405423846211,0.69,1.0,90.0,-5.326030494188355e-05,5.650163583514271e-05,-9.929957996023724e-05,0.00011186755142931195
-0.161405423846211,0.75,1.0,52.0,-9.181741400237061e-05,8.48312454929629e-05,-0.00017904022046789683,0.0001683181053284517
-0.161405423846211,0.81,1.0,10.0,-4.0476169779474284e-06,3.7408912557232516e-06,-8.291713416876478e-06,7.007575603811411e-06
-0.2050582217609286,0.21,1.0,12.0,-0.00029038193989499016,0.00032589739819504634,-0.0005267032309234523,0.0006638654667240406
-0.2050582217609286,0.27,1.0,28.0,-0.00029245018822958023,0.00027607548839022575,-0.0005753093841685967,0.000547623675949728
-0.2050582217609286,0.33,1.0,35.0,-0.0003050169658514399,0.00024780575153204285,-0.0006419655933163288,0.0004563243195242302
-0.2050582217609286,0.39,1.0,51.0,-0.0001833700446093685,0.0001771669882448702,-0.0003631040038222434,0.0003414958769878446
-0.2050582217609286,0.45,1.0,51.0,-0.0001648130242378278,0.00017134287481506848,-0.000326145781770273,0.0003393409192541184
-0.2050582217609286,0.51,1.0,54.0,-0.0001428130133982005,0.0001554142905461745,-0.00027133500783625236,0.0003218277692281412
-0.2050582217609286,0.57,1.0,56.0,-0.00010967587668526375,0.0001325811519280687,-0.00021629134815255046,0.00026311478732917473
-0.2050582217609286,0.63,1.0,58.0,-8.60113069490755e-05,9.611588654732136e-05,-0.00014981860884839086,0.0002040722521059407
-0.2050582217609286,0.69,1.0,90.0,-6.198410539539813e-05,6.889477968996082e-05,-0.00011743839667876087,0.00014008751516301032
-0.2050582217609286,0.75,1.0,52.0,-0.00010460718788038697,0.0001009664825442106,-0.00020391013897295553,0.0001953106605172691
-0.2050582217609286,0.81,1.0,10.0,-9.934858603193994e-06,7.600371678752851e-06,-2.0043871112918688e-05,1.4169122658905891e-05
-0.2605171084697369,0.21,1.0,12.0,-0.0004697402374687924,0.0005581006436973219,-0.0009131524954722202,0.0010644802157323517
-0.2605171084697369,0.27,1.0,28.0,-0.0004979684934923903,0.00046134753554032246,-0.0009774241092558994,0.0009207478008857723
-0.2605171084697369,0.33,1.0,36.0,-0.0004941201224374135,0.00038706439921946267,-0.001027431604055875,0.0007309813801808706
-0.2605171084697369,0.39,1.0,51.0,-0.00028844991809354826,0.0002680611659438394,-0.0005824583788987975,0.0005254699017750676
-0.2605171084697369,0.45,1.0,52.0,-0.0002467468273146929,0.0002437970673707347,-0.0004932001845320364,0.0004888404068338595
-0.2605171084697369,0.51,1.0,52.0,-0.00021616700007568256,0.00023028096189460606,-0.00039969193617266785,0.00047258908731244106
-0.2605171084697369,0.57,1.0,56.0,-0.00015550504079679735,0.00018484756328000524,-0.000290095074357882,0.00035551277741334566
-0.2605171084697369,0.63,1.0,57.0,-0.00010441982354745334,0.00013393247998582685,-0.00020366265855992677,0.00026169313524408364
-0.2605171084697369,0.69,1.0,93.0,-7.639263392454075e-05,8.636252067421563e-05,-0.00014280151826401367,0.00016978726666996854
-0.2605171084697369,0.75,1.0,50.0,-0.000128427685688209,0.0001237893239409166,-0.00026158284788112566,0.00023997175255295123
-0.2605171084697369,0.81,1.0,10.0,-1.5731955622040886e-05,1.126001655081389e-05,-3.262712929776354e-05,2.0086188594565973e-05
-0.3309750919646775,0.21,1.0,12.0,-0.0007757227641300588,0.0008910496419503929,-0.0015640706083288813,0.0016801224640375532
-0.3309750919646775,0.27,1.0,28.0,-0.000803708047792425,0.0007663860000988474,-0.0016494821846499792,0.0014591328507815296
-0.3309750919646775,0.33,1.0,37.0,-0.0007836616504668338,0.0006150945022308604,-0.0015320032805486486,0.001157257867488399
-0.3309750919646775,0.39,1.0,50.0,-0.0004613079482519534,0.00042352916522238576,-0.0009235009468776622,0.0008062909275222446
-0.3309750919646775,0.45,1.0,52.0,-0.00037109001223136276,0.00037515061874240864,-0.0007471332682921873,0.0007222682670262151
-0.3309750919646775,0.51,1.0,54.0,-0.00029761895449636393,0.00030658096250208014,-0.0005953767496406469,0.0006381144054749975
-0.3309750919646775,0.57,1.0,58.0,-0.00021593134477263944,0.0002331306644711112,-0.0004286567624386641,0.0004740978436173493
-0.3309750919646775,0.63,1.0,55.0,-0.00013220426700160683,0.00016802037373047797,-0.0002578202651294833,0.00034150432436764284
-0.3309750919646775,0.69,1.0,90.0,-9.851749242273352e-05,0.00010498573234715613,-0.00019006873549995044,0.00021477635023618824
-0.3309750919646775,0.75,1.0,51.0,-0.00014826898352488682,0.00014340539836709475,-0.0003055204604044499,0.0002638845077025893
-0.3309750919646775,0.81,1.0,10.0,-2.3996349880748172e-05,2.0163236632253336e-05,-4.734849803563875e-05,3.6642874408046145e-05
-0.4204887431174665,0.21,1.0,13.0,-0.0011755962135180324,0.0013252728497901557,-0.0023441266202488867,0.0026448692509984727
-0.4204887431174665,0.27,1.0,29.0,-0.0014430617418081033,0.0012120653505857401,-0.0029844930996456836,0.0023568546084218726
-0.4204887431174665,0.33,1.0,35.0,-0.0011265265223396874,0.0009162258161588627,-0.0022650582706071364,0.0016673969901061065
-0.4204887431174665,0.39,1.0,52.0,-0.0006978043657110093,0.0006083666827119269,-0.0013737428222119668,0.001186733258982755
-0.4204887431174665,0.45,1.0,53.0,-0.0005508217244186211,0.0005353429466039762,-0.0011531636366698935,0.0010062509837573642
-0.4204887431174665,0.51,1.0,53.0,-0.00046315146090856584,0.000466064009015888,-0.0009359671474372407,0.0009148952989591426
-0.4204887431174665,0.57,1.0,56.0,-0.00029393877228351203,0.00032211398152566083,-0.0005638499225182257,0.0006408764143544819
-0.4204887431174665,0.63,1.0,56.0,-0.00017765684649246208,0.00020131481020950568,-0.0003410386292901446,0.0004347952790452795
-0.4204887431174665,0.69,1.0,90.0,-0.00012395759623864814,0.0001348558822800569,-0.0002453111726969862,0.00027514160484629513
-0.4204887431174665,0.75,1.0,50.0,-0.00017162507380450364,0.00016958772046579763,-0.0003507356371653437,0.0003193699282138642
-0.4204887431174665,0.81,1.0,10.0,-4.342354321985015e-05,3.9060812471880635e-05,-8.517837706101353e-05,7.093894056066904e-05
-0.5342117500109822,0.21,1.0,13.0,-0.001983386953275988,0.0018764989314356843,-0.0038167676164726745,0.003909791408844313
-0.5342117500109822,0.27,1.0,29.0,-0.00200957275982696,0.0017629904389053783,-0.004217922675715988,0.003339703641861225
-0.5342117500109822,0.33,1.0,36.0,-0.001638942274505632,0.0012184920914313571,-0.003251642654610763,0.0024476303403708132
-0.5342117500109822,0.39,1.0,52.0,-0.000992617060791984,0.0008869299090934511,-0.0020277507632876237,0.0016760373262680154
-0.5342117500109822,0.45,1.0,52.0,-0.0008539922813769761,0.0007717220435426991,-0.00163268166260923,0.0015377736806948192
-0.5342117500109822,0.51,1.0,54.0,-0.0006568407416279576,0.0006692384374021454,-0.0013054331375825267,0.0013209818624480042
-0.5342117500109822,0.57,1.0,57.0,-0.00041571870720491787,0.000466784119057472,-0.0007975228317139213,0.0009309421544756285
-0.5342117500109822,0.63,1.0,57.0,-0.0002270280441651084,0.0002930399976983925,-0.0004413715250733356,0.0005740327661318068
-0.5342117500109822,0.69,1.0,88.0,-0.00017568571756290669,0.00018243944369799998,-0.00034332477659237417,0.0003695345172380808
-0.5342117500109822,0.75,1.0,49.0,-0.0002200769507166061,0.00021790164735954542,-0.00043044244771172404,0.0004142930907047755
-0.5342117500109822,0.81,1.0,10.0,-9.231281274797395e-05,7.977552136807744e-05,-0.0001816288450210945,0.00014945643148191792
-0.6786916380543073,0.21,1.0,14.0,-0.0028266192361641016,0.00271013429055372,-0.0054674119524242915,0.00545273139797066
-0.6786916380543073,0.27,1.0,29.0,-0.0027438795921887905,0.002248514182164561,-0.0054821263226899715,0.004285973337880356
-0.6786916380543073,0.33,1.0,36.0,-0.0022408879374476074,0.0018348791153091635,-0.004667871475788345,0.003338274132026771
-0.6786916380543073,0.39,1.0,52.0,-0.0013125747990904504,0.0011882300010096576,-0.0027395458711629273,0.002287056796917644
-0.6786916380543073,0.45,1.0,54.0,-0.001151652241187597,0.0010467039362581213,-0.0022670862458484212,0.001986520628984969
-0.6786916380543073,0.51,1.0,54.0,-0.0009187700468674397,0.0008908162976781615,-0.0017737131198623875,0.001754844130281347
-0.6786916380543073,0.57,1.0,57.0,-0.0005798326579671702,0.0006157322955688291,-0.0010961716088909096,0.001241556847601207
-0.6786916380543073,0.63,1.0,57.0,-0.0003041114525708411,0.00033459095552142284,-0.0005637632864458332,0.0007088280679487028
-0.6786916380543073,0.69,1.0,86.0,-0.00022256623616475455,0.00022876448172943708,-0.0004428277660072895,0.00044396406133281077
-0.6786916380543073,0.75,1.0,49.0,-0.00026279824046287055,0.00023538792189432413,-0.0005073874950462611,0.0004791989334540633
-0.6786916380543073,0.81,1.0,9.0,-0.00015748340273363573,0.000148261346939464,-0.0003170148791476541,0.00027817833545392155
-0.8622467393414316,0.21,1.0,15.0,-0.003799884613480508,0.0036877106501616613,-0.00745987643433261,0.0072459800072132
-0.8622467393414316,0.27,1.0,28.0,-0.003314610730795862,0.002742793745067855,-0.006967676508301433,0.005059003151677459
-0.8622467393414316,0.33,1.0,41.0,-0.00251522773843792,0.0022228777345157146,-0.005368758764039065,0.003988497921314107
-0.8622467393414316,0.39,1.0,52.0,-0.0017292718997240334,0.0015415533760419428,-0.0034950736188906826,0.0029299373146913924
-0.8622467393414316,0.45,1.0,52.0,-0.0015733123307975997,0.0014448348050886814,-0.00319121608642655,0.0027767760559334787
-0.8622467393414316,0.51,1.0,55.0,-0.0012917147524951122,0.0011522620276421868,-0.002497082859461174,0.002308935846351685
-0.8622467393414316,0.57,1.0,53.0,-0.0007587288835817996,0.0007847509586266178,-0.001415791034388041,0.0015958733312356527
-0.8622467393414316,0.63,1.0,60.0,-0.00036977200347508446,0.00043450365209366773,-0.0007331751504528519,0.0008190422295108604
-0.8622467393414316,0.69,1.0,86.0,-0.00030472793775759057,0.0002930559729215037,-0.0005949344536581546,0.0005800530473917266
-0.8622467393414316,0.75,1.0,47.0,-0.00032577409372081835,0.0003058857945488517,-0.0006447892873894275,0.000589056181568989
-0.8622467393414316,0.81,1.0,8.0,-0.00026805894721787515,0.0002619829872320123,-0.0005044360558466993,0.0004947927443951986
-1.0954451150103155,0.21,1.0,15.0,-0.004242850020867771,0.004306400983333206,-0.0079925125658898,0.008470022581741501
-1.0954451150103155,0.27,1.0,29.0,-0.003840260568042298,0.0033162101544774174,-0.007895087883491607,0.0063189089750584175
-1.0954451150103155,0.33,1.0,44.0,-0.0027294364051271545,0.00232264623295382,-0.005558485722670376,0.004428510311915893
-1.0954451150103155,0.39,1.0,51.0,-0.0022939502168196134,0.0021008470742095837,-0.004679137493423354,0.004052408852718576
-1.0954451150103155,0.45,1.0,52.0,-0.001956540209114305,0.00165717152880144,-0.003897599683969651,0.0032573761597841076
-1.0954451150103155,0.51,1.0,54.0,-0.0017560217745490794,0.0016569020007030403,-0.0035253239178019346,0.00333725024658514
-1.0954451150103155,0.57,1.0,54.0,-0.000951495462472175,0.0010282899881848022,-0.0018932418657296422,0.0020602840861568793
-1.0954451150103155,0.63,1.0,61.0,-0.000541274687426607,0.0005830763278017473,-0.0011032374572629382,0.001177441314294551
-1.0954451150103155,0.69,1.0,81.0,-0.0004322624287567853,0.00040874677114312286,-0.0008351088830901643,0.0008096181561105599
-1.0954451150103155,0.75,1.0,47.0,-0.0004506335109561205,0.00045268191288476493,-0.0009244662420359765,0.0008158665005198164
-1.0954451150103155,0.81,1.0,8.0,-0.0003875957266292057,0.00040108256369796036,-0.0007715833399315475,0.0007436961344430838
-1.391713004234152,0.15,1.0,5.0,-0.00786643530006581,0.005785505504186482,-0.014007591480995462,0.011768171281874596
-1.391713004234152,0.21,1.0,14.0,-0.003950026361321933,0.0042285368395540346,-0.007389226256147267,0.008672989080805141
-1.391713004234152,0.27,1.0,31.0,-0.0034807600030004045,0.003073849953431867,-0.007132507790262361,0.005857455246103364
-1.391713004234152,0.33,1.0,49.0,-0.0028453807138978534,0.002432635813322166,-0.005607184713265991,0.004829129714124051
-1.391713004234152,0.39,1.0,47.0,-0.002551279034457131,0.002600432725858498,-0.0052050871371462,0.0046510282135180814
-1.391713004234152,0.45,1.0,55.0,-0.002345393038464908,0.002229510215583701,-0.004842040105373109,0.004195794724058422
-1.391713004234152,0.51,1.0,53.0,-0.0022980536616833847,0.002180557623078434,-0.004500440574710131,0.004334976219354343
-1.391713004234152,0.57,1.0,52.0,-0.0013073446578619158,0.0014602058048499413,-0.002641028676618495,0.002890078675866449
-1.391713004234152,0.63,1.0,59.0,-0.0008510609682361907,0.0008264612137106045,-0.0016228068083838968,0.001801432677383391
-1.391713004234152,0.69,1.0,82.0,-0.0006265466274607311,0.0005905919412381196,-0.0012179223346503747,0.0012010850667770407
-1.391713004234152,0.75,1.0,45.0,-0.0007379776646156786,0.0006388039713805134,-0.0014518066980273485,0.0012458464255024402
-1.391713004234152,0.81,1.0,8.0,-0.000524603652411193,0.0005341419772565692,-0.0010129923181417394,0.0009690121836845082
-1.7681078308849716,0.15,1.0,5.0,-0.007241681523609443,0.0048969233782188105,-0.012055092411141843,0.011006796956519783
-1.7681078308849716,0.21,1.0,15.0,-0.0031359506922772496,0.0034929672560890176,-0.005884982349575116,0.007012646418565528
-1.7681078308849716,0.27,1.0,33.0,-0.0029846212815974717,0.0026764377911962733,-0.00648650527642441,0.004908891300728908
-1.7681078308849716,0.33,1.0,51.0,-0.0026195527687201147,0.002506717407263028,-0.005278569538115345,0.00471083059246152
-1.7681078308849716,0.39,1.0,43.0,-0.0026335233806599905,0.002591212367247498,-0.0052249149193807085,0.004949350074104073
-1.7681078308849716,0.45,1.0,57.0,-0.0024055162589874408,0.0022753748424579525,-0.004808065870207148,0.004386462487844334
-1.7681078308849716,0.51,1.0,53.0,-0.0026513961593622915,0.00256862589311667,-0.005104004952283887,0.004901048847514887
-1.7681078308849716,0.57,1.0,52.0,-0.001740759196395196,0.0017297429258832184,-0.0033534885905920067,0.00348251233484044
-1.7681078308849716,0.63,1.0,57.0,-0.0010324614702693841,0.001142050799090067,-0.0021145585570369616,0.002161130437710193
-1.7681078308849716,0.69,1.0,84.0,-0.0008092501413627563,0.0008112797668704283,-0.001602139642339756,0.00153527265402931
-1.7681078308849716,0.75,1.0,42.0,-0.0010386899748579665,0.0008925126849913313,-0.0020487839395792965,0.0018000477455468729
-1.7681078308849716,0.81,1.0,8.0,-0.0006324067769572803,0.0006233951063104718,-0.001183803058197569,0.0011874438645194686
-2.246300273206905,0.15,1.0,6.0,-0.004956933354449267,0.005783929347492296,-0.009274650702672157,0.011359165910161043
-2.246300273206905,0.21,1.0,14.0,-0.0027014843794922563,0.0030863479285513015,-0.00525589674037922,0.006164634251798479
-2.246300273206905,0.27,1.0,36.0,-0.002479559874878233,0.0024199593395545604,-0.005295531318107886,0.004362908674070292
-2.246300273206905,0.33,1.0,54.0,-0.002315557213115915,0.002023242416264975,-0.0044008911374044885,0.003983486776759588
-2.246300273206905,0.39,1.0,49.0,-0.0022122823612716015,0.0020762161684770033,-0.004588338123145724,0.003825551074578301
-2.246300273206905,0.45,1.0,57.0,-0.002208813656590221,0.002181513741584285,-0.004410950321695294,0.00432968610761519
-2.246300273206905,0.51,1.0,42.0,-0.002733398310686505,0.002779069401323009,-0.005588357466247687,0.0053070033850903045
-2.246300273206905,0.57,1.0,58.0,-0.0017450988460200364,0.0016632381089547038,-0.0033767939334960703,0.0034500113424173516
-2.246300273206905,0.63,1.0,54.0,-0.0012636624231361822,0.001212517494990798,-0.002436875272457326,0.002337237207870316
-2.246300273206905,0.69,1.0,79.0,-0.0009408195362861128,0.0009509303239208116,-0.0019003092035359732,0.001892399607622964
-2.246300273206905,0.75,1.0,43.0,-0.0012807684513375071,0.0010863708333777868,-0.0025033059449328975,0.0020770977441781284
-2.246300273206905,0.81,1.0,8.0,-0.0007328752415303869,0.0007347395170735435,-0.0014127306519490235,0.00138816684497646
-2.8538219384978705,0.15,1.0,5.0,-0.004396279078790101,0.005300196689839097,-0.005775280071211287,0.010845606663901686
-2.8538219384978705,0.21,1.0,18.0,-0.0026166042929065504,0.002337805198168514,-0.005193318683301785,0.004413589597835573
-2.8538219384978705,0.27,1.0,35.0,-0.002376700533655258,0.002116161582856352,-0.004601483119175816,0.004193753004634623
-2.8538219384978705,0.33,1.0,60.0,-0.0019190246427871853,0.0017289958057697455,-0.003717166239919858,0.003312317135034386
-2.8538219384978705,0.39,1.0,48.0,-0.002356108115860139,0.001965239151107237,-0.004750133438148986,0.003723514840517867
-2.8538219384978705,0.45,1.0,57.0,-0.00208250088452646,0.0021043866890013622,-0.004222843061401384,0.00409530600139917
-2.8538219384978705,0.51,1.0,51.0,-0.001807463611226786,0.0020319757171641316,-0.0036557448011785816,0.0040158217664358065
-2.8538219384978705,0.57,1.0,50.0,-0.0019047181463315156,0.0019866308547493734,-0.003793504404521347,0.003852255595702399
-2.8538219384978705,0.63,1.0,49.0,-0.0015433647965428516,0.0013852449627739108,-0.0029723669325269655,0.002759721508861052
-2.8538219384978705,0.69,1.0,77.0,-0.001132957151926819,0.001031967999340733,-0.002167431471651284,0.0020129410686871587
-2.8538219384978705,0.75,1.0,41.0,-0.0013570909406926824,0.001178164152750544,-0.0028238187266645264,0.0022302203449122786
-2.8538219384978705,0.81,1.0,7.0,-0.004460650055019323,0.00313576716455144,-0.011482754251638643,0.004130672826471235
-3.625650476828138,0.15,1.0,5.0,-0.0038414360144152435,0.004552164831927065,-0.0049681648382660076,0.012212036600459799
-3.625650476828138,0.21,1.0,23.0,-0.0022469695232952046,0.0019424901007210978,-0.00456019355229099,0.003669134302299492
-3.625650476828138,0.27,1.0,35.0,-0.001848784870678105,0.001807293129072573,-0.003553176431474588,0.0035860146504234605
-3.625650476828138,0.33,1.0,65.0,-0.001741523605310839,0.001503943964374003,-0.0034961174682558156,0.0029008557841638943
-3.625650476828138,0.39,1.0,50.0,-0.0022534041471472675,0.0017294096684262051,-0.0044880966975723675,0.0034461797843234453
-3.625650476828138,0.45,1.0,49.0,-0.002270458624692003,0.0021823872541516113,-0.004470758427036813,0.004238595098661136
-3.625650476828138,0.51,1.0,53.0,-0.001613502410662963,0.001482881297603644,-0.003168250013272063,0.0029460830568851146
-3.625650476828138,0.57,1.0,52.0,-0.001760274462483171,0.0016855505530759725,-0.0034400709272633203,0.0034484970823002443
-3.625650476828138,0.63,1.0,45.0,-0.001964772813685779,0.0016295810452577047,-0.003886877560557897,0.003132477532789741
-3.625650476828138,0.69,1.0,75.0,-0.0010379834794887856,0.0010965602286390208,-0.002199941650561913,0.0020166054704062178
-3.625650476828138,0.75,1.0,37.0,-0.0016591353159809026,0.0015033796621516608,-0.003452318246354319,0.002761045275684377
-3.625650476828138,0.81,1.0,8.0,-0.004356191246614419,0.003019239439709817,-0.009555073181169237,0.005354535393149581
-4.606223395648545,0.15,1.0,7.0,-0.0044801975709085435,0.0028032123745481384,-0.008088493966901934,0.005335407726975813
-4.606223395648545,0.21,1.0,21.0,-0.0021186930058574227,0.0016366096087539477,-0.004173384219162888,0.0033562179094998716
-4.606223395648545,0.27,1.0,48.0,-0.0015263176081231685,0.0014008463043844017,-0.003003134220618775,0.002747784190137312
-4.606223395648545,0.33,1.0,52.0,-0.0014689722035504422,0.0013473619367741687,-0.003097209431797286,0.0025330268191008968
-4.606223395648545,0.39,1.0,58.0,-0.0016839613894004599,0.001540442191972336,-0.003497335336463985,0.002903967882656367
-4.606223395648545,0.45,1.0,47.0,-0.0018255378403510606,0.0016550924995605756,-0.003685453592958033,0.003205327068977454
-4.606223395648545,0.51,1.0,53.0,-0.0013169101660718604,0.0012609171538478954,-0.0025134921670770536,0.0025382240538666767
-4.606223395648545,0.57,1.0,54.0,-0.0016323260683793982,0.0016023243825429847,-0.0032233962586604966,0.0031164011354567304
-4.606223395648545,0.63,1.0,51.0,-0.00129787386527542,0.0012095985473628789,-0.002572342187876929,0.0023821497383026613
-4.606223395648545,0.69,1.0,63.0,-0.0012484325422089696,0.0012061068845555516,-0.0025146915196369597,0.0023395958502102636
-4.606223395648545,0.75,1.0,35.0,-0.0015249374282704977,0.0016026837959700602,-0.003364662143205537,0.0029655102500671547
-4.606223395648545,0.81,1.0,7.0,-0.004363115068911374,0.0029730609759264543,-0.009930309788600792,0.005103473785022959
-5.851996519306446,0.15,1.0,9.0,-0.002116233093357018,0.00259826154849039,-0.00406468673375377,0.005326403396526646
-5.851996519306446,0.21,1.0,22.0,-0.002202862972783133,0.0020386373061501858,-0.004394895644524195,0.003884353565440179
-5.851996519306446,0.27,1.0,50.0,-0.0015835870148410245,0.0015129551230747447,-0.003227145831070178,0.0028608083872143355
-5.851996519306446,0.33,1.0,50.0,-0.0015072007875109265,0.0014067591325464337,-0.0032392968724148145,0.0026384958267896092
-5.851996519306446,0.39,1.0,56.0,-0.0014273444597715664,0.0012110428896391534,-0.002761323853992593,0.0024764307103977115
-5.851996519306446,0.45,1.0,56.0,-0.001681551017828908,0.0015633701210063231,-0.0033131145122847695,0.0030184181638880027
-5.851996519306446,0.51,1.0,56.0,-0.0013371405089442185,0.0013099825039037825,-0.0026855213565753194,0.002465454027844839
-5.851996519306446,0.57,1.0,48.0,-0.0017117353658796398,0.0017692290704902035,-0.0031474967516055344,0.003770254631843283
-5.851996519306446,0.63,1.0,54.0,-0.001625425359732855,0.001605889975775993,-0.0032055497242725705,0.003182552465701316
-5.851996519306446,0.69,1.0,50.0,-0.0017208553770081884,0.0015714820888474343,-0.003452851682746776,0.003015843793987356
-5.851996519306446,0.75,1.0,35.0,-0.002329820028898438,0.002307311103244945,-0.0047932418955195,0.004285406615273533
-5.851996519306446,0.81,1.0,9.0,-0.0039725298742045575,0.003022732387361615,-0.008414367905970034,0.005357405991120065
-7.434694395049615,0.15,1.0,7.0,-0.0023734851024781313,0.0021512539745266444,-0.004526454353912969,0.004199862189758698
-7.434694395049615,0.21,1.0,26.0,-0.0017249822243250409,0.0016535475240364353,-0.0032250026604030485,0.0034061104838229335
-7.434694395049615,0.27,1.0,50.0,-0.0014984213588853943,0.0013447120599950314,-0.0030524879476054945,0.0026733795919855353
-7.434694395049615,0.33,1.0,55.0,-0.001051285189565473,0.001081447128199202,-0.0020498012163075556,0.002112497447116001
-7.434694395049615,0.39,1.0,58.0,-0.0011339887061159303,0.0011086957333552485,-0.002249217488672003,0.002236234775258704
-7.434694395049615,0.45,1.0,51.0,-0.0018265511567025269,0.001733223609598917,-0.003541141497072558,0.0033422408936366627
-7.434694395049615,0.51,1.0,66.0,-0.0014634065781147145,0.001518032180084232,-0.002933555264024801,0.002881829745752702
-7.434694395049615,0.57,1.0,52.0,-0.0018271679253189642,0.0019521550262802084,-0.0036828461633325532,0.0037004752850784877
-7.434694395049615,0.63,1.0,44.0,-0.002556440993431281,0.0023312181896925255,-0.005235921402213091,0.004582546850160433
-7.434694395049615,0.69,1.0,48.0,-0.003124909220749793,0.0028362605520096773,-0.006297228239015835,0.005356548353385216
-7.434694395049615,0.75,1.0,26.0,-0.00456574050552668,0.004448497428918855,-0.00920545764481114,0.00815498411965234
-7.434694395049615,0.81,1.0,9.0,-0.005840482615652302,0.00540840191166053,-0.011492012242279115,0.01000761491890128
-7.434694395049615,0.87,1.0,5.0,-0.00795908930115994,0.0055876950298551446,-0.01798590460201306,0.009083792916947697
-9.445439785451782,0.15,1.0,9.0,-0.0012756346732573473,0.001393196450560771,-0.002337178331549714,0.002856288425246539
-9.445439785451782,0.21,1.0,24.0,-0.0020154457517875595,0.0020908477191682435,-0.003873127651597022,0.004011478922673496
-9.445439785451782,0.27,1.0,55.0,-0.0014637764759965965,0.0013533248558000022,-0.0029359457329944964,0.002545875345239891
-9.445439785451782,0.33,1.0,67.0,-0.0013010661558432977,0.0013061114692194077,-0.0025532394273815678,0.0026323350335427918
-9.445439785451782,0.39,1.0,46.0,-0.0022718701294584505,0.002126632912256605,-0.00454598370994201,0.0042448615841078965
-9.445439785451782,0.45,1.0,64.0,-0.0023252989203155785,0.0021424682714094585,-0.004710368608343503,0.0042812121545508335
-9.445439785451782,0.51,1.0,66.0,-0.001996893899736578,0.0020728086698540583,-0.0038466551194275746,0.004007429977113975
-9.445439785451782,0.57,1.0,40.0,-0.0032994801122031275,0.003257917591506099,-0.006840119761671104,0.006222204038977007
-9.445439785451782,0.63,1.0,42.0,-0.004792951451838821,0.0035980652564994815,-0.0098569727746487,0.006706642855594221
-9.445439785451782,0.69,1.0,42.0,-0.006907361930675302,0.006343688106932665,-0.013663854183002986,0.012449786047710827
-9.445439785451782,0.75,1.0,14.0,-0.011482225851937871,0.012545061049451299,-0.021454671188445375,0.024680848576749067
-9.445439785451782,0.81,1.0,14.0,-0.005467736564011986,0.005006893284530279,-0.010476040596056595,0.009659365428507575
-9.445439785451782,0.87,1.0,12.0,-0.005178400213688267,0.004979676633560611,-0.010362784440202081,0.009467748253650805
-9.445439785451782,0.93,1.0,5.0,-0.0022495668097321604,0.003119369996556111,-0.004089710895599462,0.006450974198533112
-11.999999999999991,0.21,1.0,27.0,-0.0021086613647530237,0.00199885666291344,-0.004172874608412793,0.003923279498004739
-11.999999999999991,0.27,1.0,53.0,-0.0017367847552927508,0.0017811217534244943,-0.0033577890470074022,0.003609985985804409
-11.999999999999991,0.33,1.0,63.0,-0.001842851877607326,0.0019023906601714395,-0.003587864176761842,0.003788979775038957
-11.999999999999991,0.39,1.0,62.0,-0.0029712819274286023,0.002778898065393253,-0.005853904927702431,0.005406697596903091
-11.999999999999991,0.45,1.0,58.0,-0.0047422011780757205,0.004060894154621804,-0.01008714893176272,0.007418508626142803
-11.999999999999991,0.51,1.0,63.0,-0.005269294433352383,0.004914921649378891,-0.010347323964928799,0.009126445721809496
-11.999999999999991,0.57,1.0,46.0,-0.006409128352358127,0.005625159641984202,-0.012768027984353532,0.010961250436555254
-11.999999999999991,0.63,1.0,30.0,-0.009558118910191168,0.007305151783157277,-0.019987415381240936,0.013197847242229957
-11.999999999999991,0.69,1.0,35.0,-0.01122130904431216,0.009848856711399435,-0.022745870354632308,0.01750131972772533
-11.999999999999991,0.75,1.0,23.0,-0.015416304605948183,0.015109233842831587,-0.02862570217016023,0.0314995315232314
-11.999999999999991,0.81,1.0,11.0,-0.01084229784788123,0.008136030943423876,-0.022058470211983726,0.015394503969412858
-11.999999999999991,0.87,1.0,13.0,-0.006542064428555295,0.006852680772588899,-0.013031807440416278,0.01321007028909957
-11.999999999999991,0.93,1.0,8.0,-0.008261174457351805,0.007633199742341531,-0.017364846729161137,0.01382932154808942
-11.999999999999991,0.99,1.0,5.0,-0.004836065288123504,0.004836065288123503,-0.007958800432295732,0.008008946809680584
-0.0999999999999926,0.27,2.0,20.0,-5.2662966641997076e-05,5.022461299551652e-05,-0.00010752574590877165,9.438668882784424e-05
-0.0999999999999926,0.33,2.0,33.0,-3.562174649639642e-05,3.270199725514228e-05,-6.89498822511372e-05,6.473332192535655e-05
-0.0999999999999926,0.39,2.0,52.0,-2.6043325574214924e-05,2.2552729222368996e-05,-5.2015308217345556e-05,4.294323276094539e-05
-0.0999999999999926,0.45,2.0,60.0,-1.75450435928801e-05,1.647064047926688e-05,-3.585960973465306e-05,3.1695067309537725e-05
-0.0999999999999926,0.51,2.0,50.0,-2.1265216857260187e-05,2.3727262266218954e-05,-3.961314187721752e-05,5.06602621025587e-05
-0.0999999999999926,0.57,2.0,51.0,-2.2019956439415267e-05,2.9144449822347286e-05,-4.11030421101594e-05,5.917722915790263e-05
-0.0999999999999926,0.63,2.0,58.0,-2.5698424550605128e-05,3.239214582782252e-05,-4.840574334658799e-05,6.673685868015041e-05
-0.0999999999999926,0.69,2.0,55.0,-2.9600593601360067e-05,3.217878489545581e-05,-5.3268453325669326e-05,6.895233505571417e-05
-0.0999999999999926,0.75,2.0,38.0,-3.7768996372480055e-05,4.3603666083130725e-05,-7.216557955712364e-05,8.850627159322333e-05
-0.0999999999999926,0.81,2.0,33.0,-4.660705776774228e-05,4.8545179663135094e-05,-8.923520176990033e-05,9.318008617962387e-05
-0.0999999999999926,0.87,2.0,19.0,-3.4353942636007866e-05,2.9302866481729288e-05,-0.00012178857571619258,3.1070087278503176e-05
-0.0999999999999926,0.93,2.0,23.0,-7.348883665461827e-07,7.087835396413054e-07,-1.3560962826805544e-06,1.404083543087979e-06
-0.1270454343320486,0.27,2.0,20.0,-7.665947996913885e-05,6.772554005351697e-05,-0.00015366951071906472,0.00013347011152950973
-0.1270454343320486,0.33,2.0,33.0,-4.70493147580997e-05,4.848024535797037e-05,-9.869328366589143e-05,8.99865785671984e-05
-0.1270454343320486,0.39,2.0,53.0,-3.5156101286073557e-05,3.20700103353469e-05,-7.282455240981554e-05,6.142418982901843e-05
-0.1270454343320486,0.45,2.0,59.0,-2.6746298628588395e-05,2.1768348553635257e-05,-5.0178641118726074e-05,4.360120488740695e-05
-0.1270454343320486,0.51,2.0,50.0,-2.6259099930732343e-05,2.7803678101617614e-05,-5.279679810571668e-05,5.427589143165996e-05
-0.1270454343320486,0.57,2.0,51.0,-2.4948998721345705e-05,2.9436428024239757e-05,-4.707223125276067e-05,6.182491717723657e-05
-0.1270454343320486,0.63,2.0,58.0,-2.7708059410674757e-05,3.168726332964422e-05,-5.179930068618456e-05,6.768310480337423e-05
-0.1270454343320486,0.69,2.0,55.0,-2.7444186902940058e-05,3.7869861341524235e-05,-5.4489758424829015e-05,6.821683353294622e-05
-0.1270454343320486,0.75,2.0,38.0,-3.7406372366200686e-05,4.5269662700110286e-05,-7.277597594795557e-05,8.914450949717343e-05
-0.1270454343320486,0.81,2.0,33.0,-4.613462133269557e-05,5.052638717533786e-05,-9.356404209680946e-05,8.812495178780029e-05
-0.1270454343320486,0.87,2.0,19.0,-5.885228195049833e-05,2.947588860353948e-05,-0.00012647865153143567,3.19580361768776e-05
-0.1270454343320486,0.93,2.0,23.0,-1.1002539283837055e-06,1.037767394779089e-06,-2.1496305666428356e-06,2.014003357229485e-06
-0.1614054238461599,0.27,2.0,20.0,-0.00011984077695903421,0.00010717053218861276,-0.00023454586868566811,0.00021147915008970362
-0.1614054238461599,0.33,2.0,33.0,-7.424861942680404e-05,7.253757275818565e-05,-0.00015021759876014944,0.00013939795265487974
-0.1614054238461599,0.39,2.0,54.0,-5.818045176060172e-05,4.917693636012541e-05,-0.00011678576623837509,9.375627350285596e-05
-0.1614054238461599,0.45,2.0,58.0,-3.7231875341267416e-05,3.273977237589098e-05,-7.335124749780607e-05,6.247883741253331e-05
-0.1614054238461599,0.51,2.0,50.0,-4.111389021701525e-05,3.5723498183948104e-05,-8.155220458396679e-05,7.126320344357579e-05
-0.1614054238461599,0.57,2.0,51.0,-3.0371230624104745e-05,3.399844539634606e-05,-6.250218223725376e-05,6.471396570036542e-05
-0.1614054238461599,0.63,2.0,58.0,-3.080372923618002e-05,3.4825567681528995e-05,-5.827534724103527e-05,7.340397434598766e-05
-0.1614054238461599,0.69,2.0,55.0,-3.2101511563393605e-05,3.4837334923922836e-05,-5.624382987992325e-05,7.212885495175154e-05
-0.1614054238461599,0.75,2.0,38.0,-3.9323703483530275e-05,4.523801854976961e-05,-7.401879746892634e-05,9.143313500635552e-05
-0.1614054238461599,0.81,2.0,33.0,-4.847185111200937e-05,4.9937345370805156e-05,-9.486009476769698e-05,9.784054924091338e-05
-0.1614054238461599,0.87,2.0,19.0,-6.17742541388813e-05,2.9934389878932197e-05,-0.00012985503851953146,3.3606504077691504e-05
-0.1614054238461599,0.93,2.0,23.0,-1.6334303444676495e-06,1.4760308824100524e-06,-3.113165063480111e-06,2.815550715430469e-06
-0.2050582217608856,0.27,2.0,20.0,-0.00021186535408980917,0.0001943652506195707,-0.00041300727578385356,0.00035704668311929493
-0.2050582217608856,0.33,2.0,33.0,-0.00012920279897344478,0.00012349778484731407,-0.00026300424872112974,0.00023964618019896931
-0.2050582217608856,0.39,2.0,54.0,-0.00010462814908385602,8.771803138284755e-05,-0.00021424443644635005,0.00016618175824148528
-0.2050582217608856,0.45,2.0,58.0,-6.149414990020815e-05,5.710119429892486e-05,-0.0001244076138809998,0.00011103357812131652
-0.2050582217608856,0.51,2.0,50.0,-6.87780548582383e-05,5.779496118411281e-05,-0.00014165902695793006,0.00010800970621992189
-0.2050582217608856,0.57,2.0,51.0,-4.821824297749302e-05,4.43537791502765e-05,-9.461741565317127e-05,8.786237229538257e-05
-0.2050582217608856,0.63,2.0,58.0,-3.9226234621454304e-05,4.590749114036434e-05,-7.6579727667591e-05,9.177937728184925e-05
-0.2050582217608856,0.69,2.0,56.0,-3.751769383987633e-05,4.455477439441808e-05,-7.0880418214901e-05,8.82961514323487e-05
-0.2050582217608856,0.75,2.0,37.0,-4.364470089300187e-05,5.158659111345665e-05,-8.05150450031346e-05,0.00010900841475599987
-0.2050582217608856,0.81,2.0,33.0,-5.734652679442709e-05,5.610018571206549e-05,-0.00011004717719193819,0.0001115532277960337
-0.2050582217608856,0.87,2.0,19.0,-6.906318742579275e-05,3.3725991914966335e-05,-0.0001471932296947884,3.883399641938628e-05
-0.2050582217608856,0.93,2.0,23.0,-2.435109933224281e-06,2.405372359583646e-06,-4.93087998071484e-06,4.461598369912992e-06
-0.260517108469752,0.27,2.0,20.0,-0.0003360345086765766,0.00033579749166331736,-0.0006813878270793749,0.0006243685721859475
-0.260517108469752,0.33,2.0,33.0,-0.00022763737247521863,0.00021004445618362885,-0.00044332951285533194,0.0004073839728550311
-0.260517108469752,0.39,2.0,54.0,-0.00017364483259463484,0.00015148772533031432,-0.00036782393825074937,0.0002860753287128221
-0.260517108469752,0.45,2.0,59.0,-0.00010482507071862544,0.00010175731959435019,-0.00021582513462562817,0.00018724896181527065
-0.260517108469752,0.51,2.0,50.0,-0.00011942153996885341,9.021041069121514e-05,-0.0002271154240103341,0.00018429702428368334
-0.260517108469752,0.57,2.0,50.0,-7.699920749033424e-05,6.855426991861767e-05,-0.0001551025665038887,0.00012913883849376525
-0.260517108469752,0.63,2.0,58.0,-5.931196776728189e-05,6.271916917316596e-05,-0.0001156480234565932,0.0001290578009284617
-0.260517108469752,0.69,2.0,55.0,-5.446055443700466e-05,6.0258849099075845e-05,-0.0001036875725504058,0.00012034432591223337
-0.260517108469752,0.75,2.0,38.0,-5.899118674250599e-05,6.866992355737636e-05,-0.00011130999568172954,0.0001430830028055691
-0.260517108469752,0.81,2.0,33.0,-7.749017101805042e-05,8.031590731452029e-05,-0.0001473604096384066,0.00015820247578956023
-0.260517108469752,0.87,2.0,19.0,-8.967617780714151e-05,4.384772858309236e-05,-0.00019931725553317127,5.40821031636099e-05
-0.260517108469752,0.93,2.0,23.0,-4.969393260556991e-06,4.556727024370275e-06,-9.898797239207055e-06,8.685730240358607e-06
-0.3309750919646431,0.27,2.0,20.0,-0.0005807683552226766,0.0005493395569576425,-0.0011791475639305977,0.0010140802063989167
-0.3309750919646431,0.33,2.0,34.0,-0.0003669558572712557,0.00036949770445667956,-0.0007479484134371008,0.0006959271246296082
-0.3309750919646431,0.39,2.0,55.0,-0.000310796299566686,0.00026044703166058336,-0.0005969156508607772,0.000495367981286007
-0.3309750919646431,0.45,2.0,58.0,-0.00018283239180883498,0.00016207544034492187,-0.0003686866168676723,0.0003189321999191635
-0.3309750919646431,0.51,2.0,49.0,-0.00018406592991854166,0.00015861210805113066,-0.00039060864700996587,0.00029262257511175957
-0.3309750919646431,0.57,2.0,51.0,-0.00011624096774676567,0.00010471135358736493,-0.00025206347749073257,0.0001969775226893653
-0.3309750919646431,0.63,2.0,58.0,-8.22359317237303e-05,8.819672402861384e-05,-0.00016773539999100936,0.00017477433779820723
-0.3309750919646431,0.69,2.0,55.0,-7.342088593106707e-05,7.767603228937427e-05,-0.0001406405790616933,0.00015945193326983166
-0.3309750919646431,0.75,2.0,37.0,-7.4354880142323e-05,8.360885246481565e-05,-0.0001320736774327401,0.00017633814910476963
-0.3309750919646431,0.81,2.0,33.0,-9.704199565910824e-05,9.572095301472922e-05,-0.00018270675112106447,0.00018407799656518383
-0.3309750919646431,0.87,2.0,19.0,-8.947249905648526e-05,4.972106172236469e-05,-0.000231723384323807,6.916330442817646e-05
-0.3309750919646431,0.93,2.0,23.0,-8.983889893126283e-06,7.819658739759702e-06,-1.850752080609662e-05,1.4383941174417455e-05
-0.4204887431174273,0.27,2.0,20.0,-0.0009161279061134278,0.000868195664590663,-0.0018723004944284861,0.0016159883666729488
-0.4204887431174273,0.33,2.0,35.0,-0.000602880895625825,0.0005953302238798123,-0.0012115922924665044,0.001147768533840226
-0.4204887431174273,0.39,2.0,54.0,-0.0005210607806348247,0.0004222337822137368,-0.0010507204086404726,0.0008052209804137742
-0.4204887431174273,0.45,2.0,58.0,-0.000303006839791137,0.0002623542673337216,-0.00060287006631604,0.0005059080276570578
-0.4204887431174273,0.51,2.0,49.0,-0.00029780782561542556,0.00023842353484176666,-0.000620002411829992,0.00045224515246166974
-0.4204887431174273,0.57,2.0,51.0,-0.00018689901273893298,0.0001557160822984267,-0.0003812713598039119,0.0002983641430052957
-0.4204887431174273,0.63,2.0,60.0,-0.00012226951760549364,0.00011629553640793102,-0.00023272637402156548,0.0002246810483306972
-0.4204887431174273,0.69,2.0,52.0,-9.357284330648656e-05,0.00010226851714065341,-0.0001782227538059815,0.0002059274956035059
-0.4204887431174273,0.75,2.0,38.0,-8.25521081024241e-05,0.00010626871908817727,-0.0001619986021560062,0.0002157053888556044
-0.4204887431174273,0.81,2.0,33.0,-0.00011869630426941465,0.0001110477826277812,-0.00022620487420359437,0.00021958878000858712
-0.4204887431174273,0.87,2.0,18.0,-0.00011886452330454216,5.61331125579139e-05,-0.0002855835167993256,8.417510096501947e-05
-0.4204887431174273,0.93,2.0,24.0,-1.3763987115635827e-05,1.1574107535677316e-05,-2.783147897868796e-05,2.2659029978440853e-05
-0.5342117500109889,0.27,2.0,20.0,-0.0014145773166399907,0.0012968341627212564,-0.002839432340734864,0.002436253340314991
-0.5342117500109889,0.33,2.0,37.0,-0.0009546720882254349,0.0008977595109475511,-0.001898513191382157,0.0017560705630641292
-0.5342117500109889,0.39,2.0,52.0,-0.0008116409930912306,0.0006622330606058973,-0.0016905756371552567,0.001270666401515797
-0.5342117500109889,0.45,2.0,60.0,-0.0005006663250777942,0.00044875013613847456,-0.001011787646231717,0.0008621969967803834
-0.5342117500109889,0.51,2.0,49.0,-0.0003878007423884793,0.0003149023824418546,-0.0007592480813894695,0.0006396737905204349
-0.5342117500109889,0.57,2.0,51.0,-0.0002687605040520468,0.00022099887243290364,-0.0005487267234937504,0.00040828411157155085
-0.5342117500109889,0.63,2.0,58.0,-0.00015869701643601378,0.00016952422464367475,-0.00033770260812231585,0.00031512715205287805
-0.5342117500109889,0.69,2.0,52.0,-0.00012294027749632565,0.00014107466543359764,-0.0002453277609071762,0.00027136229638867666
-0.5342117500109889,0.75,2.0,39.0,-0.00010608864190551838,0.0001294972964580601,-0.0002002996214903486,0.0002482260191693761
-0.5342117500109889,0.81,2.0,31.0,-0.0001447428754835291,0.0001469233443435757,-0.0002878790433974069,0.00029692618071187703
-0.5342117500109889,0.87,2.0,19.0,-0.00012568181204235672,6.373842006630108e-05,-0.00029615147529932586,0.00010346052038589848
-0.5342117500109889,0.93,2.0,24.0,-1.9805632636879434e-05,1.4759698228331803e-05,-3.972395614192425e-05,2.8369420564581427e-05
-0.6786916380543315,0.27,2.0,21.0,-0.0019627725175717947,0.0017679635663841215,-0.0039077616192492,0.003390223749812515
-0.6786916380543315,0.33,2.0,36.0,-0.001447002720813113,0.0013574987304954898,-0.002936067247041517,0.002640259498844725
-0.6786916380543315,0.39,2.0,55.0,-0.0010981718055413747,0.0010215019277693136,-0.0022636213077625515,0.0019021043024510316
-0.6786916380543315,0.45,2.0,59.0,-0.0007414338093545081,0.0007453860893116917,-0.0016390588102803585,0.0013525553939457424
-0.6786916380543315,0.51,2.0,50.0,-0.0005597867305201268,0.0004918618599942448,-0.0011295201926184825,0.0009443347048408837
-0.6786916380543315,0.57,2.0,47.0,-0.00042671350033351714,0.00034542327211954275,-0.0008601677616947004,0.0006843133636405182
-0.6786916380543315,0.63,2.0,59.0,-0.000238583601354994,0.00022126559317755778,-0.00048384404548543674,0.00042093483896696093
-0.6786916380543315,0.69,2.0,52.0,-0.0001755023182679648,0.00018389064397777093,-0.00033799984142495463,0.0003748125938190859
-0.6786916380543315,0.75,2.0,39.0,-0.00014073679080626433,0.00016398773359640708,-0.00025846938414263274,0.00032866437185357636
-0.6786916380543315,0.81,2.0,31.0,-0.00018293742686474842,0.00019118604537240994,-0.000376661796977958,0.0003672628097417369
-0.6786916380543315,0.87,2.0,19.0,-0.00015435041889638154,8.239978952450423e-05,-0.0003406964794904434,0.00015067352810645647
-0.6786916380543315,0.93,2.0,24.0,-3.1046296976957756e-05,2.4382659785413398e-05,-6.574527166378661e-05,4.5027878105656094e-05
-0.8622467393414301,0.21,2.0,5.0,-0.005286764000717527,0.007066403052011559,-0.009692019538704445,0.015199806722808563
-0.8622467393414301,0.27,2.0,20.0,-0.002856414697985618,0.002426700763201576,-0.005672463965772139,0.004645835267340877
-0.8622467393414301,0.33,2.0,38.0,-0.00209507484463397,0.0018925907621746144,-0.0038703245205169317,0.003751990538026902
-0.8622467393414301,0.39,2.0,55.0,-0.0016452531567973027,0.0013896161978320131,-0.0033500273563507733,0.0026722155053889615
-0.8622467393414301,0.45,2.0,57.0,-0.0012426360845794295,0.0011174619828550653,-0.0025657452774519936,0.0020839668723212895
-0.8622467393414301,0.51,2.0,52.0,-0.0008230271310575318,0.0007469038441638758,-0.0016619260232157561,0.0013954125052210399
-0.8622467393414301,0.57,2.0,48.0,-0.000614572331207012,0.0005487389646997924,-0.0012749900575341482,0.0010210419532788897
-0.8622467393414301,0.63,2.0,56.0,-0.00035467617679316307,0.00034036339592152315,-0.0007158338489099759,0.000658743495881852
-0.8622467393414301,0.69,2.0,56.0,-0.000241276103802299,0.0002454690477397314,-0.00046009576618799683,0.0004850378679420293
-0.8622467393414301,0.75,2.0,37.0,-0.0002053149659739233,0.00022708336279541745,-0.0003798363445046607,0.00046578537247972
-0.8622467393414301,0.81,2.0,30.0,-0.00022980747560716723,0.0002432581418278239,-0.0004664716757582289,0.00045880845178294217
-0.8622467393414301,0.87,2.0,18.0,-0.00020528809142608955,0.00013245874027095254,-0.0004433361008551534,0.00023674381046553237
-0.8622467393414301,0.93,2.0,24.0,-5.694924383391939e-05,4.189461325591408e-05,-0.00012169416301584747,7.686564448128896e-05
-1.0954451150103115,0.21,2.0,5.0,-0.007297097058091983,0.006724388197605569,-0.012307459346900562,0.014021485255697552
-1.0954451150103115,0.27,2.0,21.0,-0.0034191531148025952,0.0031278323426542566,-0.0068890725167532725,0.006027165630936571
-1.0954451150103115,0.33,2.0,40.0,-0.0025640468035491954,0.0024942599818086244,-0.005108031720139426,0.004848973974478025
-1.0954451150103115,0.39,2.0,55.0,-0.0024188602138651267,0.001990485992335868,-0.004745777880936213,0.003906316573477214
-1.0954451150103115,0.45,2.0,55.0,-0.0017776175685713632,0.001518440891865657,-0.0034856789601593347,0.002927120659463195
-1.0954451150103115,0.51,2.0,55.0,-0.0013341644145655161,0.0012204685287642997,-0.002658889463063612,0.0023395427645737485
-1.0954451150103115,0.57,2.0,44.0,-0.0009684645842068249,0.00077185233424486,-0.0019030117576109922,0.0015708322928950358
-1.0954451150103115,0.63,2.0,57.0,-0.000553337863837186,0.0004836154054510149,-0.0011420195301416571,0.0009473595366242684
-1.0954451150103115,0.69,2.0,54.0,-0.00035848706461893173,0.00036853199884678123,-0.0007129533289804424,0.0007128294783352569
-1.0954451150103115,0.75,2.0,39.0,-0.00027913991300773655,0.0003083000134703309,-0.0005440072077642929,0.0006192530711348768
-1.0954451150103115,0.81,2.0,29.0,-0.000324646919318851,0.0002816448573621269,-0.0006083894801064694,0.0005821079193173634
-1.0954451150103115,0.87,2.0,17.0,-0.00025976037124264827,0.00020626992839781175,-0.0005512994674984129,0.0003889655072216826
-1.0954451150103115,0.93,2.0,24.0,-0.0001019253692525037,7.270657731403889e-05,-0.00021831543973732895,0.00013504994228218174
-1.0954451150103115,0.99,2.0,5.0,-7.191428847765914e-05,4.4781121129133786e-05,-0.0001418598383740921,8.787417666740181e-05
-1.39171300423419,0.21,2.0,5.0,-0.00748485417486857,0.005534605376516467,-0.013561359372689829,0.010462761278653622
-1.39171300423419,0.27,2.0,23.0,-0.00332615151585744,0.0030371461965222396,-0.007017512509162281,0.0058207072793773715
-1.39171300423419,0.33,2.0,41.0,-0.0028653497913744734,0.0030892948742901167,-0.0058098744239127595,0.005834668857645068
-1.39171300423419,0.39,2.0,54.0,-0.0028127868965342195,0.002643033706675843,-0.006015357201195679,0.004923331683903243
-1.39171300423419,0.45,2.0,55.0,-0.002256365992452041,0.0020563460612184757,-0.004584618892536978,0.0038866479669457856
-1.39171300423419,0.51,2.0,57.0,-0.0018614972502853438,0.0016097854515653733,-0.00373341277119152,0.0031965301419593726
-1.39171300423419,0.57,2.0,41.0,-0.0013163176505609443,0.0012009686315844342,-0.0027893867757868575,0.002252326112142802
-1.39171300423419,0.63,2.0,57.0,-0.0007864209885797798,0.0007259045593298484,-0.0016446667073120296,0.0013537403433502002
-1.39171300423419,0.69,2.0,54.0,-0.0004993535308102704,0.0005001856918726875,-0.0010072795104794953,0.0010092944582436923
-1.39171300423419,0.75,2.0,40.0,-0.0003890761108760922,0.00040722658159499927,-0.0007559899344733326,0.0008497712673561443
-1.39171300423419,0.81,2.0,26.0,-0.0004132997572038246,0.0003680247271715317,-0.0008053719174249081,0.0007459582554348046
-1.39171300423419,0.87,2.0,18.0,-0.0003494971693514732,0.0003008776327074733,-0.0007311370953116082,0.0005576210102988573
-1.39171300423419,0.93,2.0,24.0,-0.0001785181160820046,0.00012765935022166205,-0.00040815776959833393,0.000221680962424644
-1.39171300423419,0.99,2.0,5.0,-0.0001410760961459979,8.948655488900661e-05,-0.0002817022130144676,0.000144217697618254
-1.7681078308849574,0.21,2.0,5.0,-0.006860924001548517,0.004740970533738788,-0.012289221560258022,0.009995782168714374
-1.7681078308849574,0.27,2.0,23.0,-0.0028951130786267925,0.002760242590019077,-0.005813301729312045,0.00541573704899506
-1.7681078308849574,0.33,2.0,46.0,-0.0027439907146583277,0.0027765693866792125,-0.005475451917747934,0.005308454593680809
-1.7681078308849574,0.39,2.0,54.0,-0.0031636432461618616,0.002881619147894355,-0.006271237934847696,0.005544273400254391
-1.7681078308849574,0.45,2.0,52.0,-0.002638300839815853,0.0024195385912035633,-0.005276668566895403,0.004613422702548708
-1.7681078308849574,0.51,2.0,55.0,-0.0026231520740067154,0.002217133974134917,-0.005119109358555269,0.00440429128868449
-1.7681078308849574,0.57,2.0,44.0,-0.0015765462735143584,0.001464009031551877,-0.003106631726124053,0.002873229605973129
-1.7681078308849574,0.63,2.0,54.0,-0.0011321392030769811,0.0010189203042025804,-0.0023862325796192626,0.0019246136443229812
-1.7681078308849574,0.69,2.0,54.0,-0.0007017711179337777,0.000643119708879305,-0.0013176942675405315,0.0012879672527084
-1.7681078308849574,0.75,2.0,38.0,-0.0006135307299118711,0.0005478145071090446,-0.0011694021676364181,0.0011283256021356381
-1.7681078308849574,0.81,2.0,28.0,-0.0005314303976423559,0.0004416694424141877,-0.0010611369478524528,0.0008644965662433176
-1.7681078308849574,0.87,2.0,17.0,-0.0005421595963900201,0.00044303715686142236,-0.0011458504661837293,0.0008290387947802589
-1.7681078308849574,0.93,2.0,22.0,-0.0003657891203708168,0.0002088506683905615,-0.0007767592516231429,0.000368508706983568
-1.7681078308849574,0.99,2.0,8.0,-0.00014492102352539615,0.00010328370779737195,-0.0002939234478074315,0.00019755658407411648
-2.2463002732069515,0.21,2.0,7.0,-0.0043304504824015645,0.004049370895551051,-0.008787725324598181,0.007831865074203177
-2.2463002732069515,0.27,2.0,22.0,-0.0027724715983622025,0.0027915806743788805,-0.005491090866509327,0.005518720105513277
-2.2463002732069515,0.33,2.0,48.0,-0.0024020345367266184,0.0023362125397974544,-0.0046623338513809495,0.004652035423836234
-2.2463002732069515,0.39,2.0,56.0,-0.0028695443786634803,0.0028632570944972196,-0.00586262229893404,0.0053081352261889585
-2.2463002732069515,0.45,2.0,50.0,-0.002655099751069015,0.0024174671348867163,-0.005382002029335264,0.004720799380544009
-2.2463002732069515,0.51,2.0,53.0,-0.0027790282906804925,0.002518875743534575,-0.0055704843942280015,0.004861120449246835
-2.2463002732069515,0.57,2.0,44.0,-0.0024023061737795492,0.002187596130447164,-0.004898814426908719,0.004129850650236446
-2.2463002732069515,0.63,2.0,55.0,-0.0014429003069643196,0.0012786139181627779,-0.0028612573197917463,0.0024855933000852677
-2.2463002732069515,0.69,2.0,52.0,-0.000901475116618128,0.0008697869164215032,-0.0016951617602319932,0.0018058532327297095
-2.2463002732069515,0.75,2.0,37.0,-0.000854928439659105,0.0008381586546085218,-0.001722438722949694,0.0016008386906438635
-2.2463002732069515,0.81,2.0,27.0,-0.0008313026947030153,0.0006715269868027965,-0.0016886704250658172,0.0012321508331594956
-2.2463002732069515,0.87,2.0,18.0,-0.000818614154652423,0.0006223716321042019,-0.0016939947135391651,0.0011221665715444302
-2.2463002732069515,0.93,2.0,22.0,-0.0005197508560550496,0.00034981994990094286,-0.0011787157561913494,0.0005817430408100988
-2.2463002732069515,0.99,2.0,9.0,-0.00018236887062001155,0.0001899461017303685,-0.0003519395578461604,0.00037813348196070383
-2.853821938497878,0.21,2.0,7.0,-0.0035873854137049737,0.003680139377395798,-0.006637597743926916,0.0075382794514597135
-2.853821938497878,0.27,2.0,23.0,-0.002525354898961195,0.0028179433902168613,-0.005044502278098447,0.005437093721936511
-2.853821938497878,0.33,2.0,50.0,-0.002063971613253569,0.002011926643146931,-0.00406649654072992,0.003962896259108028
-2.853821938497878,0.39,2.0,55.0,-0.002542578576621406,0.002383351052203716,-0.00499457447772665,0.004829735160227787
-2.853821938497878,0.45,2.0,51.0,-0.0024068165846504856,0.0021433560136440728,-0.004767900816385965,0.004225812169652637
-2.853821938497878,0.51,2.0,54.0,-0.002513418283771359,0.0024319788258716983,-0.005178079629547344,0.004751447803042465
-2.853821938497878,0.57,2.0,41.0,-0.0025193487156990836,0.002379707115136842,-0.00506659467669637,0.004519482204366394
-2.853821938497878,0.63,2.0,55.0,-0.0015730103888926998,0.0015393641797736913,-0.0033734427080302125,0.003072606764132973
-2.853821938497878,0.69,2.0,52.0,-0.001199632732545449,0.0011952608847174025,-0.0023717424640897163,0.002366295811917613
-2.853821938497878,0.75,2.0,38.0,-0.001154591804941795,0.001103909030241101,-0.0022837792740443823,0.0020888294341925586
-2.853821938497878,0.81,2.0,24.0,-0.0012907948556184915,0.0010262457849464165,-0.0026796489754731027,0.0019294837894119972
-2.853821938497878,0.87,2.0,19.0,-0.0010512012767368642,0.0008143515239291826,-0.0022083522435371095,0.0015241024607488046
-2.853821938497878,0.93,2.0,22.0,-0.0007487353494932547,0.00047855055121807005,-0.001644227856891164,0.0008804139532829749
-2.853821938497878,0.99,2.0,9.0,-0.0003421737232945218,0.0004008299281845022,-0.0006211429165642982,0.0008208206015980997
-3.62565047682812,0.21,2.0,7.0,-0.0032787520390453262,0.003520388059879896,-0.0062331427213501165,0.006177956060183786
-3.62565047682812,0.27,2.0,23.0,-0.0022111722582996442,0.002268542130855755,-0.004316218299149423,0.004506328044799265
-3.62565047682812,0.33,2.0,52.0,-0.0019744721265643234,0.0018408043848600827,-0.0037595273088792754,0.0035561505620046252
-3.62565047682812,0.39,2.0,55.0,-0.0019116112014335059,0.0018612406902846152,-0.003848147912510897,0.003547951814000949
-3.62565047682812,0.45,2.0,50.0,-0.001831454158509576,0.0017954569815835566,-0.003744249762796606,0.003296466510032073
-3.62565047682812,0.51,2.0,52.0,-0.0022979770425933465,0.0019422377358567693,-0.004472742406595929,0.003955594721117966
-3.62565047682812,0.57,2.0,41.0,-0.002325302807344446,0.0021427052335205986,-0.004536954432565634,0.004164791389943512
-3.62565047682812,0.63,2.0,54.0,-0.001638866173340416,0.0015746149963072515,-0.0031980309217488306,0.0030255160183061073
-3.62565047682812,0.69,2.0,53.0,-0.0011936778303921305,0.0011688207944293512,-0.002344105104217599,0.002308676896925526
-3.62565047682812,0.75,2.0,37.0,-0.001488598982689293,0.0013669610757671925,-0.0030380288406929535,0.0025835540842762935
-3.62565047682812,0.81,2.0,26.0,-0.001295761487712195,0.0010342949867830555,-0.0026943854252667867,0.001968431024439362
-3.62565047682812,0.87,2.0,17.0,-0.001138104996811393,0.0008941613205028988,-0.0025000610810728473,0.0015831992978782021
-3.62565047682812,0.93,2.0,24.0,-0.0010186510635803044,0.0007597670278278641,-0.002159926364816111,0.0014245080480713769
-3.62565047682812,0.99,2.0,9.0,-0.000595289758880321,0.0006962593496570153,-0.001115988025795344,0.0013750221726168928
-4.606223395648518,0.21,2.0,8.0,-0.0025904007539464848,0.00274953735600926,-0.005052024470767982,0.005467986680949585
-4.606223395648518,0.27,2.0,24.0,-0.0015430819113078909,0.0016217075921507046,-0.0030738684613198426,0.003185405216322905
-4.606223395648518,0.33,2.0,53.0,-0.0016806465778539028,0.0016238202560434315,-0.003329427249217047,0.0031632559835131357
-4.606223395648518,0.39,2.0,54.0,-0.0014976191139194554,0.0013655493873691283,-0.002948108930754747,0.0026770308433921707
-4.606223395648518,0.45,2.0,51.0,-0.001636547666074042,0.001569604256558425,-0.0034250722076271927,0.0028677976799959723
-4.606223395648518,0.51,2.0,49.0,-0.0018777446966178398,0.0017366075422554058,-0.0038960604040487955,0.0032950662236724683
-4.606223395648518,0.57,2.0,43.0,-0.0016027416334171854,0.0016683262880942246,-0.0032130872324197673,0.003208303697109556
-4.606223395648518,0.63,2.0,52.0,-0.001461507583087227,0.0014181237126428712,-0.0029010629438892665,0.00274394847190906
-4.606223395648518,0.69,2.0,44.0,-0.0012450112357287144,0.001309981275050007,-0.0025397802859030215,0.002553767472708818
-4.606223395648518,0.75,2.0,39.0,-0.0014056863850894633,0.0014699546990049395,-0.0027726947903830255,0.002865440524713028
-4.606223395648518,0.81,2.0,27.0,-0.001441617554384836,0.0014033801261432192,-0.002876428857142682,0.002736425080511388
-4.606223395648518,0.87,2.0,17.0,-0.0015180672118988597,0.0012367042989050903,-0.002969696534955057,0.0024011588998299597
-4.606223395648518,0.93,2.0,24.0,-0.0011675889827963127,0.0008832065469758822,-0.0026633163684232223,0.0015667997909085442
-4.606223395648518,0.99,2.0,15.0,-0.0018738938187145909,0.0014135827549609271,-0.0043373213566432044,0.002458576541575376
-5.851996519306429,0.21,2.0,10.0,-0.0021212746308763935,0.0023168435706657164,-0.004171574541676549,0.004405505097347372
-5.851996519306429,0.27,2.0,22.0,-0.0017226227938620042,0.0015909132481701348,-0.0033291160670878934,0.0032898356155323352
-5.851996519306429,0.33,2.0,48.0,-0.0016622217523624325,0.001683817671374584,-0.003286208545410261,0.0032358807293846655
-5.851996519306429,0.39,2.0,54.0,-0.0015802103798237095,0.001624027744179853,-0.003334086416078951,0.00296984171527385
-5.851996519306429,0.45,2.0,58.0,-0.0013201032559345318,0.0013371176520379383,-0.0026161955839933905,0.0026314435354657384
-5.851996519306429,0.51,2.0,44.0,-0.0017780346255435546,0.001698583580545648,-0.0034131030656963557,0.0033520141265195405
-5.851996519306429,0.57,2.0,50.0,-0.001371361845533066,0.0014743718937054845,-0.002737948448070632,0.002784066452794024
-5.851996519306429,0.63,2.0,47.0,-0.0015137519560865982,0.001340493036940933,-0.002900288622082226,0.0026265021787722537
-5.851996519306429,0.69,2.0,41.0,-0.001779475915629259,0.0016541039727869784,-0.0034933433916901667,0.003180894578548403
-5.851996519306429,0.75,2.0,31.0,-0.0017988489892283778,0.0019230436297310246,-0.0035343332195789394,0.0037860848187224612
-5.851996519306429,0.81,2.0,37.0,-0.002236002269826355,0.002216166113695211,-0.004342193706834681,0.0042359142253494035
-5.851996519306429,0.87,2.0,16.0,-0.0023625684152818785,0.0020457752726088813,-0.0046351260925205804,0.00385783704469324
-5.851996519306429,0.93,2.0,24.0,-0.0018531064205844058,0.0013840217746805882,-0.0037528624540954505,0.002633095865876604
-5.851996519306429,0.99,2.0,18.0,-0.0018832297130911555,0.0019143063893291735,-0.0040448120700314494,0.0034818733644308387
-7.434694395049619,0.21,2.0,9.0,-0.0011067074834317666,0.0011150146772871778,-0.0020144517719226517,0.002318128441594267
-7.434694395049619,0.27,2.0,24.0,-0.0012341854045233671,0.0011789777362282354,-0.0024909994304248154,0.002243080161865763
-7.434694395049619,0.33,2.0,50.0,-0.0013211167755046338,0.0012543795058485064,-0.0024242839766509877,0.002550039059115068
-7.434694395049619,0.39,2.0,56.0,-0.0011375498598111006,0.0011701070773271476,-0.002243338064665821,0.0022872033675794055
-7.434694395049619,0.45,2.0,56.0,-0.0014063511495381626,0.0012978481126389462,-0.0027204917404706997,0.0025757407381347868
-7.434694395049619,0.51,2.0,46.0,-0.001597746815058802,0.001572057933345988,-0.0031998375366801015,0.0031871766783423
-7.434694395049619,0.57,2.0,56.0,-0.0012309594571960807,0.0013264798779866857,-0.0024511498172740337,0.002648605609024289
-7.434694395049619,0.63,2.0,40.0,-0.0015382608047901064,0.0015277231641582045,-0.003098964168778873,0.0029423432144235736
-7.434694395049619,0.69,2.0,37.0,-0.002092691105501453,0.0019022325213369365,-0.004020904867495753,0.0039553131480535445
-7.434694395049619,0.75,2.0,34.0,-0.0027262489621615914,0.0025309430802328494,-0.005766799682684954,0.004856691824019399
-7.434694395049619,0.81,2.0,27.0,-0.004095640184165616,0.00379189280072385,-0.008332347697195831,0.007221479523963084
-7.434694395049619,0.87,2.0,20.0,-0.003421746216910501,0.004215573125269535,-0.0063896795886327455,0.009201124715872611
-7.434694395049619,0.93,2.0,21.0,-0.0020007457671881185,0.001646679902846208,-0.0041957216920698315,0.0031390185274595478
-7.434694395049619,0.99,2.0,23.0,-0.0027931010381707848,0.002483640771175527,-0.005645300596051579,0.004900458548803677
-9.445439785451788,0.21,2.0,8.0,-0.003765141296542207,0.0022037240566791932,-0.007964101042753732,0.0039001841083293604
-9.445439785451788,0.27,2.0,26.0,-0.0018600354728551625,0.0018971114112470687,-0.0036977365021187572,0.003806577829042058
-9.445439785451788,0.33,2.0,53.0,-0.001601167446915019,0.0015147267901878016,-0.003167169714027662,0.0030856366358239917
-9.445439785451788,0.39,2.0,58.0,-0.0015838505825741078,0.0016605642219429824,-0.003076980230890289,0.003200261971970161
-9.445439785451788,0.45,2.0,58.0,-0.0018684141213182802,0.0019309722025076406,-0.0036757877717614536,0.003886114367371626
-9.445439785451788,0.51,2.0,52.0,-0.0017144503172877115,0.0017105033703980021,-0.0032847186520527493,0.003425254476673546
-9.445439785451788,0.57,2.0,54.0,-0.0019441273502728922,0.0022567539876854146,-0.0040104236852304045,0.004309920949419963
-9.445439785451788,0.63,2.0,37.0,-0.00276857642679878,0.002506305876117528,-0.005616698905297174,0.004732157860139203
-9.445439785451788,0.69,2.0,38.0,-0.004393625792810932,0.0034472787108042685,-0.008695835294159487,0.006639619801082579
-9.445439785451788,0.75,2.0,28.0,-0.006731960105646557,0.0059546883610053555,-0.013749276486890215,0.011215142893677948
-9.445439785451788,0.81,2.0,19.0,-0.0084105512578936,0.00872703110838199,-0.01663286635481319,0.017283192648802632
-9.445439785451788,0.87,2.0,19.0,-0.004411626902286014,0.0069305367522079185,-0.007898942681316759,0.015173390362367093
-9.445439785451788,0.93,2.0,17.0,-0.003224309340775785,0.0029187166240494476,-0.006539569532212323,0.005521320780239908
-9.445439785451788,0.99,2.0,26.0,-0.0028492905799276922,0.0029788095191925572,-0.005564440066330299,0.005952511369739936
-9.445439785451788,1.05,2.0,7.0,-0.0056953543439994805,0.0035198133817047716,-0.01213567475267027,0.00631121576730678
-11.999999999999996,0.21,2.0,7.0,-0.0019346268163512464,0.0017839648119979054,-0.0038227137447623565,0.0032730312574685673
-11.999999999999996,0.27,2.0,31.0,-0.0018232827200145483,0.002020480317096868,-0.0036413258652726443,0.003972190502073299
-11.999999999999996,0.33,2.0,48.0,-0.0018753043065114319,0.0019400241905020723,-0.0035930789260346964,0.0037752945903627715
-11.999999999999996,0.39,2.0,52.0,-0.0018751444353251327,0.0021670908843753546,-0.00367963161290293,0.004151087444828473
-11.999999999999996,0.45,2.0,65.0,-0.001700912743900526,0.0017280441854793302,-0.003314778706127659,0.0034626105811321815
-11.999999999999996,0.51,2.0,55.0,-0.001988092399312199,0.0021296382604329062,-0.003936882768566271,0.004177340824179565
-11.999999999999996,0.57,2.0,52.0,-0.0026140373918900365,0.0024600189587851333,-0.0052926613639718316,0.004842589336006687
-11.999999999999996,0.63,2.0,34.0,-0.004990342791447498,0.004341260688271071,-0.01087007883927432,0.007766603948535864
-11.999999999999996,0.69,2.0,33.0,-0.00786027408685691,0.006870932981893088,-0.016357327727191402,0.013377661210872685
-11.999999999999996,0.75,2.0,29.0,-0.009524734967989874,0.008608987529638937,-0.020459951196154375,0.015382579275846466
-11.999999999999996,0.81,2.0,16.0,-0.015680031710574846,0.011405307217491407,-0.03191759796249166,0.021854256862028763
-11.999999999999996,0.87,2.0,18.0,-0.010535697619782059,0.01673518366104664,-0.019317901161946066,0.03447412223423136
-11.999999999999996,0.93,2.0,17.0,-0.002937715683659949,0.0030884100965227496,-0.005602525974953657,0.0064101564714172145
-11.999999999999996,0.99,2.0,26.0,-0.0023872488885708504,0.0016686209524853573,-0.004861681661586142,0.0031906215050184
-11.999999999999996,1.05,2.0,17.0,-0.0032547376351653675,0.0034566477891824067,-0.00611421742403778,0.007095987892200179
-0.1000000000000116,0.27,3.0,20.0,-2.079474624275968e-05,2.0390455891385857e-05,-4.224231980069906e-05,3.753505793343231e-05
-0.1000000000000116,0.33,3.0,19.0,-1.3031141240899259e-05,1.3918226769443712e-05,-2.5817998900295108e-05,2.709383413607423e-05
-0.1000000000000116,0.39,3.0,42.0,-9.34680651018517e-06,8.60058714856194e-06,-1.7846922073830038e-05,1.7155453405247992e-05
-0.1000000000000116,0.45,3.0,40.0,-1.0308062174612171e-05,8.736653610196118e-06,-2.184786833586016e-05,1.5818078341434783e-05
-0.1000000000000116,0.51,3.0,50.0,-7.90189352463902e-06,6.408325709425612e-06,-1.550782545309791e-05,1.2812658464665917e-05
-0.1000000000000116,0.57,3.0,48.0,-5.502340674614292e-06,5.018836454500709e-06,-1.0971690299313418e-05,9.712860711460371e-06
-0.1000000000000116,0.63,3.0,49.0,-4.186754521822027e-06,3.929342202657204e-06,-8.348012628418338e-06,7.716690630211835e-06
-0.1000000000000116,0.69,3.0,46.0,-7.706378850123648e-06,1.3240285906951538e-05,-1.385571955428747e-05,2.884759767667703e-05
-0.1000000000000116,0.75,3.0,49.0,-9.231056772296987e-06,1.3745022732698915e-05,-1.6336752486089218e-05,2.956412425919597e-05
-0.1000000000000116,0.81,3.0,43.0,-1.6251343050557573e-05,1.905017312331873e-05,-2.9938582049231566e-05,3.8765378948431146e-05
-0.1000000000000116,0.87,3.0,26.0,-2.6650385870507632e-05,2.2900414792858634e-05,-5.271092792874539e-05,4.536092912529134e-05
-0.1000000000000116,0.93,3.0,34.0,-4.019990977120329e-07,3.8341987743980974e-07,-7.620926120137783e-07,7.829737929355849e-07
-0.1000000000000116,0.99,3.0,33.0,-5.095654944081169e-07,4.5318227121898186e-07,-1.0786920160057554e-06,8.117080171831047e-07
-0.127045434332047,0.27,3.0,20.0,-2.96808956243739e-05,2.6226714044533807e-05,-5.75744266187809e-05,5.181733857675699e-05
-0.127045434332047,0.33,3.0,19.0,-1.6852088528641778e-05,1.8582131407267388e-05,-3.471026515382339e-05,3.5731607270944834e-05
-0.127045434332047,0.39,3.0,42.0,-1.2132407629312374e-05,1.1773305287820723e-05,-2.578714757626738e-05,2.2241957196702454e-05
-0.127045434332047,0.45,3.0,40.0,-1.3592707089592735e-05,1.142456534837991e-05,-2.8984654009738736e-05,2.1575938952776637e-05
-0.127045434332047,0.51,3.0,49.0,-1.0448355079388304e-05,8.95475393772665e-06,-2.1927107152500382e-05,1.718803524651289e-05
-0.127045434332047,0.57,3.0,49.0,-7.53698135256325e-06,6.302384852816006e-06,-1.4409891438361398e-05,1.2694842990274617e-05
-0.127045434332047,0.63,3.0,49.0,-4.957519933897089e-06,4.835940011968071e-06,-1.022022994316347e-05,9.16511075698737e-06
-0.127045434332047,0.69,3.0,46.0,-8.12136091408309e-06,1.3444315483725785e-05,-1.4792490517122324e-05,3.0009337608214487e-05
-0.127045434332047,0.75,3.0,49.0,-9.736258985439642e-06,1.349465628315497e-05,-1.7430642686239196e-05,2.9952772274938576e-05
-0.127045434332047,0.81,3.0,43.0,-1.6540597342820682e-05,2.004757139359353e-05,-3.1932581066044875e-05,3.988918984784976e-05
-0.127045434332047,0.87,3.0,26.0,-3.1027611474609566e-05,2.364227937410444e-05,-5.5990509350106625e-05,4.637278395999959e-05
-0.127045434332047,0.93,3.0,34.0,-5.491645056420492e-07,5.27854940671159e-07,-1.1437644371797989e-06,1.074125563318434e-06
-0.127045434332047,0.99,3.0,33.0,-7.371385432090138e-07,5.555506461939915e-07,-1.4769865332888947e-06,1.0818647415644554e-06
-0.1614054238461627,0.27,3.0,20.0,-4.0429154559748154e-05,4.1253863547789394e-05,-8.594993777573399e-05,7.557429558558322e-05
-0.1614054238461627,0.33,3.0,19.0,-2.5970833203241628e-05,2.6269730837574085e-05,-5.148035993299585e-05,5.331542720405763e-05
-0.1614054238461627,0.39,3.0,42.0,-1.867328848127827e-05,1.7068143128394983e-05,-3.655425089255925e-05,3.323793182799961e-05
-0.1614054238461627,0.45,3.0,40.0,-1.9830963440025816e-05,1.6282549086631443e-05,-4.297221147024004e-05,3.0843503648225206e-05
-0.1614054238461627,0.51,3.0,49.0,-1.6404907029423186e-05,1.3083159410886972e-05,-3.34881263352621e-05,2.4501777637209456e-05
-0.1614054238461627,0.57,3.0,49.0,-1.0481117999018075e-05,9.294524022605168e-06,-2.0831147032141654e-05,1.8451347291100368e-05
-0.1614054238461627,0.63,3.0,49.0,-7.162418334246973e-06,6.295991562986478e-06,-1.4481019534905771e-05,1.244726906891905e-05
-0.1614054238461627,0.69,3.0,46.0,-8.667183432895355e-06,1.338602275356151e-05,-1.567026731863405e-05,2.82021928476093e-05
-0.1614054238461627,0.75,3.0,49.0,-1.0023520509714275e-05,1.563623630831575e-05,-1.852206750376701e-05,3.152615807868119e-05
-0.1614054238461627,0.81,3.0,42.0,-1.7433560408302135e-05,2.122753730980195e-05,-3.168341335065797e-05,4.336881214632489e-05
-0.1614054238461627,0.87,3.0,27.0,-2.8934550014632554e-05,2.5137599093066097e-05,-5.800178460382069e-05,5.389400541027822e-05
-0.1614054238461627,0.93,3.0,34.0,-7.923367879922947e-07,6.968353914907986e-07,-1.7000147910134257e-06,1.3361960542746302e-06
-0.1614054238461627,0.99,3.0,33.0,-6.25890731451474e-07,4.991228001680842e-07,-1.2706669533081839e-06,9.782680936388407e-07
-0.2050582217609531,0.27,3.0,20.0,-6.990057884904664e-05,6.695384481929926e-05,-0.00013858100300413506,0.00012396594678578475
-0.2050582217609531,0.33,3.0,19.0,-4.5936204036035336e-05,4.450743964280129e-05,-8.655486043489294e-05,8.818583545170376e-05
-0.2050582217609531,0.39,3.0,43.0,-3.270302503930936e-05,2.9289770564597824e-05,-6.521629216326439e-05,5.6734600555380093e-05
-0.2050582217609531,0.45,3.0,39.0,-3.497600594938154e-05,2.70464310597499e-05,-7.124795306193409e-05,5.0253569589842646e-05
-0.2050582217609531,0.51,3.0,49.0,-2.7008780606885734e-05,2.1993300346567937e-05,-5.5671279988377877e-05,4.262680130764287e-05
-0.2050582217609531,0.57,3.0,49.0,-1.8015784922288668e-05,1.5687649191459756e-05,-3.661058275592179e-05,2.9748956694128927e-05
-0.2050582217609531,0.63,3.0,49.0,-1.1676865203970193e-05,1.0359032114072766e-05,-2.2804361400742503e-05,1.9992678163267304e-05
-0.2050582217609531,0.69,3.0,46.0,-1.0866050987191783e-05,1.5847666496807105e-05,-2.0484322719851343e-05,3.385759360483218e-05
-0.2050582217609531,0.75,3.0,49.0,-1.3068028460080109e-05,1.713723479181599e-05,-2.268494471439e-05,3.694472466865074e-05
-0.2050582217609531,0.81,3.0,41.0,-1.9418069285020927e-05,2.369653412038165e-05,-3.586808354385479e-05,4.961551500714108e-05
-0.2050582217609531,0.87,3.0,27.0,-3.49930763794438e-05,2.9362589068840362e-05,-6.558087993515582e-05,6.1927428955666e-05
-0.2050582217609531,0.93,3.0,35.0,-1.376235600185294e-06,1.3370651354017394e-06,-2.8811286529942778e-06,2.504490569585164e-06
-0.2050582217609531,0.99,3.0,33.0,-4.246258402499483e-07,4.34047190245762e-07,-8.344585307737129e-07,8.87930184419591e-07
-0.2605171084697753,0.27,3.0,20.0,-0.00012395946780321957,0.00011499573188478241,-0.00024234165731711502,0.00021801892008917255
-0.2605171084697753,0.33,3.0,19.0,-8.163110185054721e-05,8.526842902522736e-05,-0.00015910536067516792,0.00016565437776045573
-0.2605171084697753,0.39,3.0,43.0,-6.096800000194289e-05,5.3353383300114124e-05,-0.00011905165968429049,0.00011057557902218685
-0.2605171084697753,0.45,3.0,39.0,-6.30448828425417e-05,5.132326143770528e-05,-0.00012885754674796354,9.684446345897715e-05
-0.2605171084697753,0.51,3.0,49.0,-5.0370515910088556e-05,4.1612692656730957e-05,-0.00010411826172009524,7.65226603990734e-05
-0.2605171084697753,0.57,3.0,49.0,-3.2138131630108136e-05,2.9732288690603387e-05,-6.733879566277389e-05,5.636412623025443e-05
-0.2605171084697753,0.63,3.0,49.0,-2.010095081194545e-05,1.888576263481081e-05,-4.2444211436733684e-05,3.456154339591653e-05
-0.2605171084697753,0.69,3.0,46.0,-1.6780988558249015e-05,2.3502944207596837e-05,-3.131265615566567e-05,4.8544148183496094e-05
-0.2605171084697753,0.75,3.0,49.0,-1.9296477354971282e-05,2.575626208303288e-05,-3.553779507568825e-05,5.650305262327395e-05
-0.2605171084697753,0.81,3.0,41.0,-2.8254487963743015e-05,3.399124587042045e-05,-5.2309069255918935e-05,7.081487437112313e-05
-0.2605171084697753,0.87,3.0,25.0,-5.330533811511299e-05,4.4697771413230036e-05,-0.00010323110595404431,8.972635937384667e-05
-0.2605171084697753,0.93,3.0,37.0,-2.879936580431787e-06,2.512061198767615e-06,-5.857405949914729e-06,4.765511627759914e-06
-0.2605171084697753,0.99,3.0,33.0,-9.615591656872995e-07,8.586242095913524e-07,-1.8176098311348838e-06,1.6829626057621664e-06
-0.3309750919646893,0.27,3.0,20.0,-0.0001939777968257122,0.00018486773361721002,-0.0004142547598007015,0.00035311559967467475
-0.3309750919646893,0.33,3.0,19.0,-0.0001512033855377278,0.0001469603149621293,-0.0002942368368117448,0.0002872108444210482
-0.3309750919646893,0.39,3.0,43.0,-0.00010327967422945434,9.449951417406376e-05,-0.00020896787751017122,0.0001823643618034898
-0.3309750919646893,0.45,3.0,39.0,-0.00011289166008385325,8.817180667836344e-05,-0.0002433004659632732,0.00016401701268059548
-0.3309750919646893,0.51,3.0,49.0,-8.928921085254092e-05,7.246493386711056e-05,-0.0001870669938535489,0.00013470407110259018
-0.3309750919646893,0.57,3.0,49.0,-5.657921675151506e-05,5.1535941617460416e-05,-0.00011783477858843776,9.68390533561813e-05
-0.3309750919646893,0.63,3.0,49.0,-3.5538797891601095e-05,3.235516214924173e-05,-7.647465608630737e-05,6.0130113161393594e-05
-0.3309750919646893,0.69,3.0,46.0,-2.4528616994673827e-05,3.219400801701006e-05,-4.771555588778245e-05,6.695156445358339e-05
-0.3309750919646893,0.75,3.0,50.0,-2.870663024671173e-05,3.391613061909907e-05,-5.354107354652027e-05,7.26008968790944e-05
-0.3309750919646893,0.81,3.0,40.0,-3.820179811461763e-05,4.9266157972679147e-05,-7.150515111838712e-05,9.938539491058545e-05
-0.3309750919646893,0.87,3.0,24.0,-6.769846600592147e-05,6.632557427279182e-05,-0.0001429376771998628,0.00012180227975538308
-0.3309750919646893,0.93,3.0,38.0,-5.39171439133735e-06,4.318285342428645e-06,-1.1012842828106595e-05,8.45470765513946e-06
-0.3309750919646893,0.99,3.0,33.0,-1.645323094267296e-06,1.4468100558444211e-06,-3.2724941361648643e-06,2.887396106056287e-06
-0.4204887431174244,0.27,3.0,20.0,-0.000318531819956702,0.0003084853113226586,-0.000660150808799769,0.0005744293673675301
-0.4204887431174244,0.33,3.0,19.0,-0.0002698391508586204,0.0002802726065147445,-0.000530419685487429,0.0005507099487950176
-0.4204887431174244,0.39,3.0,42.0,-0.00018416852610062928,0.0001558410174535409,-0.0003584597533665522,0.0003181205615133161
-0.4204887431174244,0.45,3.0,40.0,-0.00018645520874899135,0.0001495142639394184,-0.0003875568786643739,0.00028018549845269916
-0.4204887431174244,0.51,3.0,50.0,-0.00014978867703284183,0.00011915068123459702,-0.00031256513759105335,0.00022273755881700987
-0.4204887431174244,0.57,3.0,49.0,-0.0001026674395944308,8.566710013376543e-05,-0.000204665730447776,0.00017220762970047185
-0.4204887431174244,0.63,3.0,48.0,-6.324405146039726e-05,5.503359509943747e-05,-0.00012887550605440596,0.00010479862880591716
-0.4204887431174244,0.69,3.0,46.0,-3.7370692880799424e-05,4.409168854810834e-05,-7.57488326043353e-05,8.46900087651592e-05
-0.4204887431174244,0.75,3.0,50.0,-4.1189599175746347e-05,4.909129527153933e-05,-8.235945282457031e-05,9.859319538817386e-05
-0.4204887431174244,0.81,3.0,39.0,-5.3308052549604633e-05,6.296217019429075e-05,-0.00010102261352608487,0.00013492556939658678
-0.4204887431174244,0.87,3.0,23.0,-8.928936117509816e-05,8.774378810312432e-05,-0.00018757865548266162,0.00017685080234316634
-0.4204887431174244,0.93,3.0,40.0,-9.270927910881735e-06,8.043713864102516e-06,-1.9031630186572195e-05,1.4985583195177055e-05
-0.4204887431174244,0.99,3.0,33.0,-2.6928080457062448e-06,2.349841026281839e-06,-5.324764366273327e-06,4.499534125187191e-06
-0.5342117500109385,0.27,3.0,20.0,-0.0005426931719705021,0.0004909500676987998,-0.0010348894772270886,0.0009605268905249041
-0.5342117500109385,0.33,3.0,19.0,-0.0004982573353228587,0.0005057012358731302,-0.0009654452962113752,0.0010105168320224307
-0.5342117500109385,0.39,3.0,42.0,-0.00031085273379779355,0.0002682351015987781,-0.0005851255824589962,0.000545102775493855
-0.5342117500109385,0.45,3.0,39.0,-0.0003065542163679964,0.00025565625015397516,-0.00065163406873285,0.00047398322646181136
-0.5342117500109385,0.51,3.0,51.0,-0.00024927127844510933,0.00019488513604314894,-0.0004954735270946633,0.0003806538007007523
-0.5342117500109385,0.57,3.0,50.0,-0.00016322786961365368,0.0001481913922667053,-0.0003306315119768757,0.0002729912767263296
-0.5342117500109385,0.63,3.0,46.0,-0.00010780125417148543,9.404844248679129e-05,-0.00021615870898259847,0.00017660205588369132
-0.5342117500109385,0.69,3.0,47.0,-5.6870471731590716e-05,5.186382799116159e-05,-0.00011053714658719777,0.0001001148266870462
-0.5342117500109385,0.75,3.0,49.0,-6.596836729555271e-05,7.301797724971118e-05,-0.0001337430087904393,0.0001432114359380605
-0.5342117500109385,0.81,3.0,39.0,-6.459188783821501e-05,8.018484651087858e-05,-0.00012259418141118795,0.0001694396121726406
-0.5342117500109385,0.87,3.0,24.0,-0.00012414147786559662,0.00010933080439241486,-0.00023991305686230094,0.00023456918335847444
-0.5342117500109385,0.93,3.0,39.0,-1.5372369067021188e-05,1.518661003338511e-05,-3.249495770307129e-05,2.7588046006566013e-05
-0.5342117500109385,0.99,3.0,34.0,-4.156702651172744e-06,3.8106388901386155e-06,-8.294483422754805e-06,7.2596027166739265e-06
-0.6786916380542937,0.27,3.0,21.0,-0.0007681315107058308,0.0007497051779584452,-0.0015109422988010583,0.0014647960511625254
-0.6786916380542937,0.33,3.0,18.0,-0.0008520096420179966,0.0009386595642346922,-0.0016651919305823001,0.0017356175597022221
-0.6786916380542937,0.39,3.0,42.0,-0.00048405100128633914,0.0004428616400938032,-0.0009965157234723644,0.0008367804749591234
-0.6786916380542937,0.45,3.0,40.0,-0.0004869171821424539,0.0004295584915476405,-0.0010100568017758476,0.0007725623744206826
-0.6786916380542937,0.51,3.0,49.0,-0.0004293613428121775,0.0003244976098250151,-0.000828235339412888,0.0006387238595774604
-0.6786916380542937,0.57,3.0,51.0,-0.00026589786510286507,0.00023801696402650136,-0.0005408907417725362,0.00045585046040945714
-0.6786916380542937,0.63,3.0,45.0,-0.00017299908218411535,0.00015033668550090966,-0.0003584306695671582,0.0002929639890429487
-0.6786916380542937,0.69,3.0,47.0,-0.00010952975510970979,8.239610778809148e-05,-0.00022700950214866482,0.00016093351115797807
-0.6786916380542937,0.75,3.0,49.0,-9.382418485976239e-05,9.296653894481615e-05,-0.00019506511253367974,0.00017660232365063858
-0.6786916380542937,0.81,3.0,38.0,-9.370732349951545e-05,0.00010769744082090728,-0.00017231222875342274,0.00023884684095637279
-0.6786916380542937,0.87,3.0,24.0,-0.00016137329841863982,0.00015742971943543814,-0.00030425929416818046,0.00031969176683076576
-0.6786916380542937,0.93,3.0,41.0,-2.6410025740654355e-05,2.3254249686796454e-05,-5.609581608910277e-05,4.197775361805913e-05
-0.6786916380542937,0.99,3.0,34.0,-7.333088525077112e-06,6.553764788380468e-06,-1.5384702604185973e-05,1.1828577366233956e-05
-0.862246739341482,0.27,3.0,21.0,-0.0011477035931981405,0.0011284043431016735,-0.0022534085793001596,0.0021897367379631566
-0.862246739341482,0.33,3.0,18.0,-0.001191492137661125,0.0013951571783971516,-0.0024014754397919187,0.002760440965855034
-0.862246739341482,0.39,3.0,42.0,-0.0007359376952630978,0.0007051626852944405,-0.0014790122718328484,0.0013446910986128376
-0.862246739341482,0.45,3.0,40.0,-0.0007799955979710117,0.0007399433684001305,-0.0016789844171575885,0.0013437558469764754
-0.862246739341482,0.51,3.0,49.0,-0.0006663261792156496,0.0005408052579772563,-0.0014220058552606944,0.0009954247483183985
-0.862246739341482,0.57,3.0,52.0,-0.0004267088571746587,0.00036873305034579215,-0.0008548224219605495,0.0007308026875359214
-0.862246739341482,0.63,3.0,43.0,-0.0003534638656959764,0.00029851699660759503,-0.0007580894220695671,0.0005551119952147954
-0.862246739341482,0.69,3.0,46.0,-0.00017316009470204604,0.00013847391653591578,-0.0003651642234161625,0.00025507104439393335
-0.862246739341482,0.75,3.0,51.0,-0.0001486843508792838,0.0001315432686585545,-0.0002918209652066024,0.0002692496425737138
-0.862246739341482,0.81,3.0,38.0,-0.0001289333693072204,0.00015242847632221295,-0.00024529512377383176,0.00033368164204800553
-0.862246739341482,0.87,3.0,24.0,-0.0002273022029655003,0.00021950875885485822,-0.00042555367498879225,0.00043336487345354023
-0.862246739341482,0.93,3.0,39.0,-4.7672704387668894e-05,3.6269901846250695e-05,-9.776459919808553e-05,6.962133024089485e-05
-0.862246739341482,0.99,3.0,36.0,-3.6575567549352256e-05,1.909988578575617e-05,-8.550894153932469e-05,3.1156977325379355e-05
-1.095445115010326,0.27,3.0,20.0,-0.001766914585845053,0.0016981251870049092,-0.0034317198393505003,0.003343566055911692
-1.095445115010326,0.33,3.0,18.0,-0.0017455717641243994,0.0019345808714184072,-0.0034648213754537266,0.00357524262602907
-1.095445115010326,0.39,3.0,41.0,-0.0011449503382945146,0.0011146288177398952,-0.0022859234508937863,0.002135582900445738
-1.095445115010326,0.45,3.0,42.0,-0.0012611902356155003,0.0011097012945928996,-0.0025747528372830424,0.0021537588807226298
-1.095445115010326,0.51,3.0,47.0,-0.0008493280074533219,0.0007365490862196019,-0.0016370613584403334,0.0014383747819024506
-1.095445115010326,0.57,3.0,53.0,-0.0009473140452012205,0.0007498688228210951,-0.0019360118095960637,0.001397528256361913
-1.095445115010326,0.63,3.0,44.0,-0.0005965181502928362,0.000515489345616665,-0.0012042026474090417,0.0009794780487800726
-1.095445115010326,0.69,3.0,45.0,-0.0003005609067128595,0.0002340404887255289,-0.0006040364447691285,0.0004403675231105138
-1.095445115010326,0.75,3.0,52.0,-0.0002397223888561897,0.00021529461569832342,-0.0004870732261488173,0.00040032122548813633
-1.095445115010326,0.81,3.0,37.0,-0.00019653213461928072,0.00023069248050020343,-0.00037465592832644696,0.00045889174059953976
-1.095445115010326,0.87,3.0,24.0,-0.0002790098557137226,0.0003149729398921755,-0.0005598979907522285,0.0005801983221821194
-1.095445115010326,0.93,3.0,39.0,-8.031010977717475e-05,5.65508280441918e-05,-0.0001661960809825795,0.00010974357088641371
-1.095445115010326,0.99,3.0,37.0,-5.7430422575235475e-05,3.3753556690365104e-05,-0.00013431399346962156,5.744822873414448e-05
-1.3917130042341828,0.27,3.0,20.0,-0.0021985868676596336,0.002200902767617115,-0.004345999744589027,0.004236187586737633
-1.3917130042341828,0.33,3.0,18.0,-0.0024368044925972233,0.0023549666581532337,-0.004500346114652402,0.004799720314712257
-1.3917130042341828,0.39,3.0,41.0,-0.0017177318357310132,0.0014953557106268838,-0.0033521976386562775,0.002930101311789623
-1.3917130042341828,0.45,3.0,42.0,-0.0017558301471420335,0.0015747184074220877,-0.0036036795592757328,0.0029961836150491548
-1.3917130042341828,0.51,3.0,45.0,-0.001339303089084177,0.0011807450035892174,-0.002816293183789123,0.0022736676803076367
-1.3917130042341828,0.57,3.0,55.0,-0.001343582196473582,0.0011744685024571739,-0.0028218833980928433,0.0020528881871530523
-1.3917130042341828,0.63,3.0,45.0,-0.0009563802471401555,0.0007737515975683381,-0.0019113615547421935,0.0014808672387813
-1.3917130042341828,0.69,3.0,44.0,-0.00048080235358279223,0.0003755280463292453,-0.0010118589074028879,0.000689267604542846
-1.3917130042341828,0.75,3.0,53.0,-0.0003887771170495739,0.00030891525026144123,-0.0007674501665185025,0.0005850683247556949
-1.3917130042341828,0.81,3.0,36.0,-0.00031643665903632304,0.0003102500546203754,-0.0005757381243208173,0.0006564807112299568
-1.3917130042341828,0.87,3.0,24.0,-0.0003638390488911596,0.00037302722488666247,-0.000685375036746828,0.0007516843995752582
-1.3917130042341828,0.93,3.0,38.0,-0.00014612174998059228,0.00011421065839250503,-0.0003023139059871476,0.00021530133236063553
-1.3917130042341828,0.99,3.0,37.0,-0.00010664244048051877,6.186243163582731e-05,-0.00023907711573498955,0.00010836402500024183
-1.768107830884983,0.27,3.0,18.0,-0.00224653586948987,0.002370003153860273,-0.004295301695977209,0.00479788502558305
-1.768107830884983,0.33,3.0,21.0,-0.0023658886030505366,0.0024369642466149097,-0.0046603644335146245,0.005225451681699306
-1.768107830884983,0.39,3.0,38.0,-0.0021434960333464696,0.002062715371695348,-0.004351298875797487,0.003933291059271256
-1.768107830884983,0.45,3.0,42.0,-0.002159811161444979,0.0019214606534329692,-0.00434436714186659,0.0036370290894817197
-1.768107830884983,0.51,3.0,47.0,-0.0022089727805403797,0.0017860085831121388,-0.004404070841851819,0.003518878116624184
-1.768107830884983,0.57,3.0,55.0,-0.0014282554190849562,0.0012499751941552645,-0.0027766569584771615,0.00247316804612556
-1.768107830884983,0.63,3.0,45.0,-0.00110904727931877,0.00099297110524442,-0.00229683134286644,0.0019661645129154474
-1.768107830884983,0.69,3.0,42.0,-0.0006550006679308603,0.0005515090437536421,-0.0013511435406342266,0.0010284802538155897
-1.768107830884983,0.75,3.0,51.0,-0.000545945072774852,0.00046754913026835176,-0.001170970149150168,0.0008770394747908427
-1.768107830884983,0.81,3.0,40.0,-0.0004437910965469969,0.00041931908926506737,-0.000852956784732827,0.0008705617287718799
-1.768107830884983,0.87,3.0,23.0,-0.000470150871458472,0.0005121496712878559,-0.0009215117607101813,0.0009907222213578338
-1.768107830884983,0.93,3.0,36.0,-0.00023747022629324956,0.00017249254310761696,-0.0004661472586526479,0.00033264490549077724
-1.768107830884983,0.99,3.0,38.0,-0.00016178410247128774,0.000107582478746658,-0.0003640217060302743,0.00020182745284458414
-2.246300273206898,0.27,3.0,17.0,-0.0015115381117696744,0.001910159821640928,-0.0029669247468663063,0.0037413883112364446
-2.246300273206898,0.33,3.0,19.0,-0.0025054950590847748,0.002489080946426401,-0.0045702719670123425,0.005106732179574092
-2.246300273206898,0.39,3.0,40.0,-0.002223201127406708,0.002023469970689139,-0.0044362178130280296,0.003943928897602013
-2.246300273206898,0.45,3.0,46.0,-0.0019808548290045557,0.0019338711155128352,-0.00401225417915913,0.0038042241322345715
-2.246300273206898,0.51,3.0,43.0,-0.002577768486696997,0.002269475995776504,-0.0051058450102507225,0.004531721484411952
-2.246300273206898,0.57,3.0,53.0,-0.001540917453222516,0.0015090108946376217,-0.0029827965914814977,0.002998531090638846
-2.246300273206898,0.63,3.0,42.0,-0.001476816935188863,0.0013266637019588039,-0.0030456069470034494,0.002462902985772807
-2.246300273206898,0.69,3.0,46.0,-0.0008816494705390502,0.0007558376682725523,-0.0017493278859734927,0.0014288252440985516
-2.246300273206898,0.75,3.0,49.0,-0.0007901525772666777,0.0006269177647792177,-0.001529850189244955,0.001235910012827678
-2.246300273206898,0.81,3.0,43.0,-0.0005950728428412159,0.0005871935132790029,-0.0012089453396677383,0.0011790135223446927
-2.246300273206898,0.87,3.0,34.0,-0.0005388999102899781,0.0004964057063516274,-0.0010749023819826048,0.0009691096902490771
-2.246300273206898,0.93,3.0,25.0,-0.00031560280447904496,0.0002338009154574067,-0.0006654504246341537,0.00042931898092718294
-2.246300273206898,0.99,3.0,33.0,-0.00028181094818481833,0.00016853345405734414,-0.0006147223693577909,0.0003155945788348858
-2.246300273206898,1.05,3.0,7.0,-6.646707239056854e-05,4.450432423646365e-05,-0.00014138064364761825,8.156048934157141e-05
-2.8538219384978643,0.21,3.0,5.0,-0.003226288829685697,0.0033560250006933632,-0.005414501273984152,0.006841786172394393
-2.8538219384978643,0.27,3.0,14.0,-0.0016557256215991275,0.0018267405648538513,-0.0030873851010729475,0.003868890715570499
-2.8538219384978643,0.33,3.0,24.0,-0.0017703445407653653,0.0017722573541158618,-0.0033984966198259362,0.0036176635792320158
-2.8538219384978643,0.39,3.0,38.0,-0.0017641972288064852,0.0016219849938444073,-0.003345725577308668,0.003195968675795653
-2.8538219384978643,0.45,3.0,40.0,-0.0020774749188809906,0.0020316738830225326,-0.004155903601696664,0.003907876260235189
-2.8538219384978643,0.51,3.0,49.0,-0.0019240890458189514,0.001854573095507368,-0.0038319658817614777,0.0037847418234259814
-2.8538219384978643,0.57,3.0,49.0,-0.0020230715560822805,0.0019042430866192687,-0.004060233157563551,0.0036859240279164098
-2.8538219384978643,0.63,3.0,42.0,-0.0019295581227395447,0.0016349646618410906,-0.00378514646871707,0.0032262644817241033
-2.8538219384978643,0.69,3.0,41.0,-0.0014311378791633219,0.0013944495301768652,-0.0028282720802726303,0.0027420748573345186
-2.8538219384978643,0.75,3.0,48.0,-0.0010472448588567996,0.0011341922910357047,-0.0020939172297284665,0.0022092507335787263
-2.8538219384978643,0.81,3.0,56.0,-0.0009373160898793575,0.00097062839810028,-0.0018807863510740168,0.0019418379787704003
-2.8538219384978643,0.87,3.0,35.0,-0.0009204359311210474,0.0008386088800068544,-0.0018630726212619843,0.0016251815624513874
-2.8538219384978643,0.93,3.0,19.0,-0.0007289718311939406,0.0005721692380332635,-0.0016106754880365532,0.0010269556197489526
-2.8538219384978643,0.99,3.0,30.0,-0.00023711554792156598,0.00021451329996258198,-0.0005021471153156228,0.0004002962762060452
-2.8538219384978643,1.05,3.0,10.0,-8.989184533265053e-05,0.00011337608420116628,-0.00016942636814893457,0.00023701103912234588
-3.625650476828133,0.21,3.0,6.0,-0.002765613916098142,0.002765613916098142,-0.005408436087158297,0.005446012921210182
-3.625650476828133,0.27,3.0,13.0,-0.001774620128601639,0.0019828275160158433,-0.003255674956555946,0.003948035894127638
-3.625650476828133,0.33,3.0,32.0,-0.001510943117991905,0.0015028951149031642,-0.003094389725481008,0.0029322837480522425
-3.625650476828133,0.39,3.0,31.0,-0.0017813446845073241,0.0017696201522262604,-0.003448421609989413,0.003674867507175015
-3.625650476828133,0.45,3.0,48.0,-0.0015260024370675168,0.0014909070751813213,-0.003014914658849855,0.0028787167778441306
-3.625650476828133,0.51,3.0,40.0,-0.002428447180768288,0.002413218683587332,-0.005003500807211886,0.004517824092803801
-3.625650476828133,0.57,3.0,45.0,-0.002019092637565947,0.0019814884143979907,-0.0040982037682174574,0.0038138678202454114
-3.625650476828133,0.63,3.0,38.0,-0.002825314076650004,0.0022390316726300847,-0.005614809802302248,0.004417730773106184
-3.625650476828133,0.69,3.0,50.0,-0.002131547933613164,0.0022474249205953417,-0.00414832910408208,0.004595487259269994
-3.625650476828133,0.75,3.0,46.0,-0.0022114581127122028,0.002171508545498818,-0.004146640457152518,0.004487532121670197
-3.625650476828133,0.81,3.0,56.0,-0.00159716552529127,0.001687988487096385,-0.0030870135276512035,0.003264528040267375
-3.625650476828133,0.87,3.0,36.0,-0.0015144073225483994,0.001460003667720758,-0.002872347303882925,0.0029248567916570663
-3.625650476828133,0.93,3.0,18.0,-0.0014187562284360162,0.0011171951159072693,-0.0028388298815866853,0.002145849033658616
-3.625650476828133,0.99,3.0,22.0,-0.0004779754203863985,0.0004377990077497493,-0.001012107459643712,0.0008208121969791248
-3.625650476828133,1.05,3.0,19.0,-0.00030125702114889647,0.00024143646877502686,-0.0006048438900297578,0.00047592386459244875
-4.606223395648533,0.27,3.0,7.0,-0.0037667709545094056,0.0034409535250635257,-0.007492213107173391,0.006454315777940836
-4.606223395648533,0.33,3.0,29.0,-0.001163246576489436,0.001109372443576458,-0.0021557903313235665,0.002268344004506519
-4.606223395648533,0.39,3.0,32.0,-0.0014510878279759424,0.0013748520804214058,-0.003023858271031837,0.0026235114011097698
-4.606223395648533,0.45,3.0,38.0,-0.0016824588322205867,0.0016954880591260179,-0.003442838362896705,0.0031739788015156313
-4.606223395648533,0.51,3.0,53.0,-0.0014529618185120635,0.001453876300588527,-0.002799549516820557,0.0028574260348585585
-4.606223395648533,0.57,3.0,49.0,-0.002088721098190345,0.0018155273870391617,-0.004183508950553198,0.003563870532658882
-4.606223395648533,0.63,3.0,44.0,-0.0017503653990412211,0.0018095083998206098,-0.0035971203110106544,0.0034652927583013276
-4.606223395648533,0.69,3.0,51.0,-0.0018945341390366583,0.0019232344526694232,-0.003563765143936026,0.004086137175503921
-4.606223395648533,0.75,3.0,49.0,-0.0017612006531089572,0.0018599000394137492,-0.0034166371656622393,0.003739323050751518
-4.606223395648533,0.81,3.0,50.0,-0.0017999492849775343,0.0019936019562536655,-0.003613871308789609,0.003954780479901743
-4.606223395648533,0.87,3.0,36.0,-0.001217825201743143,0.00125368079149614,-0.0023775541127594637,0.0024160696292780215
-4.606223395648533,0.93,3.0,13.0,-0.0016824167752729296,0.0014405624401183778,-0.0034238670849400157,0.0027131338988869293
-4.606223395648533,0.99,3.0,21.0,-0.0008201201888954529,0.0007045563776849829,-0.0017825046590726828,0.0012542079718130424
-4.606223395648533,1.05,3.0,26.0,-0.00039156966739175116,0.0003286661401836219,-0.0008070819234426091,0.000618843617031571
-5.851996519306431,0.33,3.0,13.0,-0.0028475882843552306,0.0030944921980054427,-0.005357123192534382,0.006511834513798949
-5.851996519306431,0.39,3.0,31.0,-0.0020778135747249148,0.0020858079062533934,-0.00407155011277979,0.004100775222473734
-5.851996519306431,0.45,3.0,42.0,-0.0013558709812820618,0.0013629680270365275,-0.0025372035242410885,0.002778984341844809
-5.851996519306431,0.51,3.0,65.0,-0.0015560706554630388,0.0015621354544664713,-0.0030866536101700755,0.0029953723877054724
-5.851996519306431,0.57,3.0,48.0,-0.0018309116455317077,0.0018032742573954857,-0.0036476337432098604,0.0035505043932837375
-5.851996519306431,0.63,3.0,62.0,-0.0019527284277351495,0.0017550203443557663,-0.003960547578893383,0.0033607968211060682
-5.851996519306431,0.69,3.0,57.0,-0.0018137963488079282,0.0018065084506911232,-0.0036779407763634516,0.003386124972229328
-5.851996519306431,0.75,3.0,43.0,-0.001499788590804867,0.0016515773702329801,-0.002898929886709146,0.0033239404893011418
-5.851996519306431,0.81,3.0,37.0,-0.0015364447858124864,0.0013855802474281556,-0.0029410260955044965,0.002818478047068548
-5.851996519306431,0.87,3.0,22.0,-0.0013417914544134669,0.0012879265072994618,-0.00267985156483807,0.0026461232655772666
-5.851996519306431,0.93,3.0,25.0,-0.0009324741960717358,0.0008602698615053713,-0.0018612401426490795,0.0016798074577253784
-5.851996519306431,0.99,3.0,20.0,-0.0017524073475467634,0.001507340042268836,-0.00374557315019568,0.0025828466579137085
-5.851996519306431,1.05,3.0,33.0,-0.0006163646229875866,0.0005577195132058352,-0.0011530683392052695,0.0011306642221496294
-7.434694395049618,0.27,3.0,8.0,-0.001798140315875621,0.0012327282076511764,-0.0036326199524992905,0.0022647716482346036
-7.434694395049618,0.33,3.0,23.0,-0.0014884386490951486,0.0014023862597829194,-0.002855815233137472,0.002655984728073641
-7.434694395049618,0.39,3.0,37.0,-0.0010954017828947121,0.001156556543307491,-0.002139045626317884,0.0022558584393306516
-7.434694395049618,0.45,3.0,39.0,-0.0012014548102372484,0.0012466223342272838,-0.0023473986731171546,0.0023906008264596274
-7.434694395049618,0.51,3.0,57.0,-0.001134617096996713,0.0010710121725610762,-0.0022946832377956734,0.0020410101852908593
-7.434694395049618,0.57,3.0,52.0,-0.0015394408740393624,0.0014979691061381766,-0.0030176084136597343,0.0028773124712518938
-7.434694395049618,0.63,3.0,57.0,-0.0012096585692279625,0.0012396935447763966,-0.0024846990508143553,0.0023781618969312334
-7.434694395049618,0.69,3.0,52.0,-0.0014572435372261477,0.0014383043040988835,-0.0027697727395229535,0.0029300641202596113
-7.434694395049618,0.75,3.0,30.0,-0.0012769942679302956,0.0013796852904992113,-0.002578345556691291,0.0026433855292151654
-7.434694395049618,0.81,3.0,24.0,-0.0019955462355504055,0.0019722336649146293,-0.003907452032365793,0.003850944697730947
-7.434694395049618,0.87,3.0,30.0,-0.001786409995005382,0.0016762272296667914,-0.0035987046272193293,0.003155162481439481
-7.434694395049618,0.93,3.0,22.0,-0.001448485277060887,0.0012647931328401544,-0.0028555653838557068,0.0025015582209259235
-7.434694395049618,0.99,3.0,35.0,-0.0013435393848591467,0.0013451429056031616,-0.002693181737857582,0.0026037606339233757
-7.434694395049618,1.05,3.0,34.0,-0.000854207587260273,0.0008634259013469676,-0.00175319486295242,0.0016604625304038573
-9.445439785451793,0.33,3.0,11.0,-0.0017921245496095085,0.0013837548419758721,-0.0035388012191790805,0.0026526500990764297
-9.445439785451793,0.39,3.0,26.0,-0.0015321280943769834,0.0015275983398299446,-0.003079458851806835,0.0028860635014940923
-9.445439785451793,0.45,3.0,39.0,-0.0013837209144811524,0.0012405450205254648,-0.0027007608153617763,0.0025076129261904054
-9.445439785451793,0.51,3.0,59.0,-0.001038776131776227,0.001107868320955214,-0.002165798162177653,0.002171898698227235
-9.445439785451793,0.57,3.0,66.0,-0.0014652314868734272,0.001413603580249609,-0.0029945941881363777,0.0027173279214080057
-9.445439785451793,0.63,3.0,70.0,-0.0011838581469347453,0.0011287630682182753,-0.002315845455330928,0.002204340129148529
-9.445439785451793,0.69,3.0,53.0,-0.0011804899831469962,0.0012183067088743487,-0.0023234855924725104,0.002389994746804734
-9.445439785451793,0.75,3.0,25.0,-0.0029535159991899967,0.001707193333905697,-0.006522467511475372,0.002992108158963143
-9.445439785451793,0.81,3.0,28.0,-0.001813932413644845,0.0018032913985094414,-0.0036030095708665375,0.003613697563538605
-9.445439785451793,0.87,3.0,25.0,-0.004285338857930844,0.0034570562791586823,-0.008887815598517501,0.0067304029293755304
-9.445439785451793,0.93,3.0,11.0,-0.005171493100329649,0.007274661840861471,-0.009050993262830598,0.015519545100838226
-9.445439785451793,0.99,3.0,23.0,-0.0028178085065718216,0.002621135811472297,-0.005672664025133254,0.005145562339860966
-9.445439785451793,1.05,3.0,39.0,-0.0024835184167351053,0.0024765023074683544,-0.005044233600347458,0.004556006155119635
-9.445439785451793,1.11,3.0,23.0,-0.0014414216184535278,0.0011745887501406185,-0.0028478698658247576,0.0022662121682683607
-11.999999999999991,0.33,3.0,8.0,-0.002363915796001898,0.001961240575887674,-0.0047016373717422896,0.0036160908502781454
-11.999999999999991,0.39,3.0,23.0,-0.001370400489819765,0.0013878805870978853,-0.0026435406489789424,0.002777464540537963
-11.999999999999991,0.45,3.0,39.0,-0.0015205243700502748,0.0014737024523646218,-0.002968502477798154,0.002989919300088416
-11.999999999999991,0.51,3.0,48.0,-0.0010633839256777558,0.0010963489810554062,-0.002147990301249067,0.0022022393592109235
-11.999999999999991,0.57,3.0,58.0,-0.0011204165137969533,0.0011011492504459197,-0.0021995757861887205,0.002110382328942743
-11.999999999999991,0.63,3.0,72.0,-0.0009912329006618052,0.001054818878889676,-0.001909665085157785,0.0020498079233590024
-11.999999999999991,0.69,3.0,53.0,-0.0011197106852969322,0.0010720337430899893,-0.0022750857562292945,0.0020032911616432616
-11.999999999999991,0.75,3.0,45.0,-0.0013666171788090065,0.0013233553958781476,-0.0026100570703992327,0.0025076245459140748
-11.999999999999991,0.81,3.0,26.0,-0.002209278661163164,0.0018073062103036847,-0.004640770208592554,0.003386630939643144
-11.999999999999991,0.87,3.0,21.0,-0.0019320055207562741,0.0014636222101134999,-0.004136321721858508,0.002758500964968875
-11.999999999999991,0.93,3.0,12.0,-0.014873353337881354,0.01565646351786073,-0.029847840334130793,0.028509445178305507
-11.999999999999991,0.99,3.0,10.0,-0.006328029731451571,0.0058268647389617375,-0.012597413382399896,0.011132638679824383
-11.999999999999991,1.05,3.0,34.0,-0.00321720732223463,0.0033233392531542404,-0.006453410750956833,0.00657423532838482
-11.999999999999991,1.11,3.0,32.0,-0.002538356659430037,0.0024902699259830344,-0.005274664500954132,0.00466778228962605
-11.999999999999991,1.17,3.0,18.0,-0.0015636191794953535,0.0013109734968097398,-0.0032400647313034574,0.0024616765274987355
+0.1000000000000023,0.33,0.0,23.0,-0.00018704725675986315,0.00020537158418103017,-0.0003597873592882187,0.00040382740106867577
+0.1000000000000023,0.39,0.0,36.0,-0.00014090624737535435,0.00014429316242699856,-0.0002621817110429632,0.0003076575604555677
+0.1000000000000023,0.45,0.0,32.0,-0.00010998188270020712,0.00015075708039691583,-0.00019913495735542682,0.00033338709269213883
+0.1000000000000023,0.51,0.0,56.0,-0.00011820227774310535,0.00014119026157873602,-0.00022819437438842811,0.0002845450195062872
+0.1000000000000023,0.57,0.0,44.0,-8.32083790850112e-05,0.00012181933380313126,-0.00015792894897780267,0.00025844962203071606
+0.1000000000000023,0.63,0.0,57.0,-8.633636597500157e-05,0.00010842920974392579,-0.0001654091475759964,0.00022104260495034726
+0.1000000000000023,0.69,0.0,104.0,-7.695618675120657e-05,7.87190697640077e-05,-0.0001541692170771733,0.00015977167173008623
+0.1000000000000023,0.75,0.0,96.0,-9.765894460879264e-05,0.00010202479786291022,-0.0001868404424034891,0.00020288776728959263
+0.1000000000000023,0.81,0.0,46.0,-0.0001535909789935542,0.0001147907443185527,-0.0003078270722578158,0.00023634099790745483
+0.1270454343320481,0.33,0.0,24.0,-0.00026119648526909585,0.0002963983215082791,-0.0005273497191543767,0.0006013120714493838
+0.1270454343320481,0.39,0.0,35.0,-0.00018516327765447002,0.0002068852667528463,-0.00037708884328907706,0.000403228788334114
+0.1270454343320481,0.45,0.0,33.0,-0.00013574928526918415,0.00018589210207326065,-0.00025803273089358746,0.0003802549238001651
+0.1270454343320481,0.51,0.0,55.0,-0.00015282926485264727,0.00016757007028416363,-0.0002826497514882095,0.00034825226326561
+0.1270454343320481,0.57,0.0,45.0,-9.623836000494539e-05,0.00013915621532823968,-0.00018497432079125757,0.0002818017777439204
+0.1270454343320481,0.63,0.0,58.0,-0.00010128244249628917,0.00011939267690312273,-0.00018989690279383847,0.00022867961733263694
+0.1270454343320481,0.69,0.0,102.0,-8.45743311866213e-05,8.014361707193834e-05,-0.00015485579238012107,0.00016637371918059584
+0.1270454343320481,0.75,0.0,97.0,-0.00010085042803800607,0.00010054264196551388,-0.00018856170542201693,0.00020954779816524029
+0.1270454343320481,0.81,0.0,45.0,-0.00015774528969505466,0.00012173347625329304,-0.00032984764554085696,0.0002246787776776291
+0.1614054238462149,0.33,0.0,24.0,-0.0004088532957341692,0.0004701928746598259,-0.0008098704038891298,0.0009002506832062307
+0.1614054238462149,0.39,0.0,36.0,-0.00026898892669652584,0.000270745245976299,-0.0005388364319680529,0.00053176559029761
+0.1614054238462149,0.45,0.0,34.0,-0.00020903650410325465,0.00024503716787769225,-0.0003975745095481635,0.0005262766789965275
+0.1614054238462149,0.51,0.0,54.0,-0.00020182276091780893,0.00022001490725164768,-0.0003823206454021191,0.0004425156335745328
+0.1614054238462149,0.57,0.0,44.0,-0.00012943146941996956,0.00017019897224304878,-0.0002408851513538926,0.0003464259436723642
+0.1614054238462149,0.63,0.0,62.0,-0.00011859821620490361,0.00013077748305630692,-0.0002258936561095484,0.0002588165658171471
+0.1614054238462149,0.69,0.0,99.0,-0.00011278764727751317,9.278598904029201e-05,-0.00022399732957717035,0.0001843740859829372
+0.1614054238462149,0.75,0.0,96.0,-0.00011762406648000372,0.00011822148323679634,-0.00023179491353023872,0.00022967240858182266
+0.1614054238462149,0.81,0.0,45.0,-0.0001662144051602667,0.0001294444231188054,-0.0003535005559499135,0.0002439204168718205
+0.2050582217609012,0.33,0.0,24.0,-0.0006038635803381414,0.0007452617781126932,-0.0012223093838838915,0.0014572748819683071
+0.2050582217609012,0.39,0.0,37.0,-0.0004052641723608616,0.00039119303353022034,-0.000818090836314982,0.0007488404907764961
+0.2050582217609012,0.45,0.0,35.0,-0.00032605713750789904,0.00035946502754559385,-0.0006160862450424589,0.0007319307838368165
+0.2050582217609012,0.51,0.0,53.0,-0.00027632755688307534,0.00031174972455754656,-0.0005236530545326366,0.0006314136027244869
+0.2050582217609012,0.57,0.0,44.0,-0.00019034882664265316,0.00022013795071374433,-0.00035059566361916563,0.00047258494840520286
+0.2050582217609012,0.63,0.0,63.0,-0.0001486962982853373,0.00016432248522373752,-0.00027648482929355886,0.000332342906944682
+0.2050582217609012,0.69,0.0,98.0,-0.00019601220406055558,0.00014465782711817814,-0.00042315273056734364,0.000266053155177515
+0.2050582217609012,0.75,0.0,96.0,-0.00016784259323293873,0.00015030875801928329,-0.00035273145777038725,0.0002980415193998783
+0.2050582217609012,0.81,0.0,44.0,-0.00021008681759443636,0.00015614141786832352,-0.00042484300509211694,0.000294351449428868
+0.2605171084697409,0.27,0.0,6.0,-0.0020384999465745683,0.0023123034394535442,-0.0038151614043873505,0.00429737193686223
+0.2605171084697409,0.33,0.0,23.0,-0.0009887144290400085,0.0011032621955082277,-0.0018669051279394762,0.002192466903228137
+0.2605171084697409,0.39,0.0,37.0,-0.0005782794691946535,0.0005070971139286167,-0.0011463824851580852,0.000976194960400617
+0.2605171084697409,0.45,0.0,37.0,-0.00044287280663522516,0.00046439641219672934,-0.0008554807276771332,0.0009085755411898689
+0.2605171084697409,0.51,0.0,51.0,-0.00036753523216245544,0.0003683720697327469,-0.0006624459644917516,0.000770386142157241
+0.2605171084697409,0.57,0.0,45.0,-0.00024702687834311717,0.00027744840441088625,-0.0004834461603269148,0.0005689755647839465
+0.2605171084697409,0.63,0.0,60.0,-0.00019036703086524224,0.00020428530381601725,-0.00036393558383795147,0.0004082893186988444
+0.2605171084697409,0.69,0.0,104.0,-0.00028249067317503296,0.0001876427926610177,-0.0005883113908809864,0.00033963527835511475
+0.2605171084697409,0.75,0.0,94.0,-0.00021806567610504191,0.00018526814210418765,-0.00046040957319312643,0.0003431367648770527
+0.2605171084697409,0.81,0.0,41.0,-0.0002484306322131801,0.00018612501127762845,-0.0005180957680088431,0.0003325829826182648
+0.3309750919646861,0.27,0.0,7.0,-0.002366822635430073,0.002639389371041895,-0.004475304783828834,0.005402438163247447
+0.3309750919646861,0.33,0.0,23.0,-0.0013664547313708801,0.001463749686385487,-0.0025693774820529105,0.0030003318754872645
+0.3309750919646861,0.39,0.0,36.0,-0.0008667263918799406,0.0007439452107067553,-0.0017113268146856863,0.0014455685505947078
+0.3309750919646861,0.45,0.0,41.0,-0.0005528248715115822,0.0005763157676901515,-0.0010805677632718938,0.0011671132300469388
+0.3309750919646861,0.51,0.0,50.0,-0.0004972689891734309,0.0005290525933429301,-0.0009779343163612234,0.0010230184957047345
+0.3309750919646861,0.57,0.0,45.0,-0.0003559180155957173,0.0003854200995838867,-0.0006818971311301458,0.0007779095081751139
+0.3309750919646861,0.63,0.0,58.0,-0.00024734112272776116,0.0002497839623139839,-0.00047174560366212694,0.0005205811842396533
+0.3309750919646861,0.69,0.0,106.0,-0.00026616321224649683,0.00020962375690204235,-0.0005558790375738739,0.00038561276579602373
+0.3309750919646861,0.75,0.0,91.0,-0.00030228078122638137,0.0002265792830295286,-0.0006452846336285126,0.0004381998700097402
+0.3309750919646861,0.81,0.0,41.0,-0.0002980388964109876,0.0002086159017429899,-0.0006199713215981804,0.0003819138543501369
+0.420488743117453,0.27,0.0,10.0,-0.0029780358652744753,0.0040508028399370895,-0.005631072216782257,0.008340161923770777
+0.420488743117453,0.33,0.0,22.0,-0.001570480791858564,0.0018490550510850221,-0.003082871381395679,0.0036574642195197384
+0.420488743117453,0.39,0.0,34.0,-0.0011950377059519023,0.0010591268590288412,-0.0024834079150219497,0.0020350734527053308
+0.420488743117453,0.45,0.0,44.0,-0.0007127666323201564,0.0007740544222494746,-0.0014056659877681199,0.0015000858412872436
+0.420488743117453,0.51,0.0,49.0,-0.0006921601607348367,0.0007285922524131447,-0.0013339502579389673,0.0014353274372843592
+0.420488743117453,0.57,0.0,48.0,-0.0004841049217429677,0.0004958148139559835,-0.0009342530328831604,0.0009761610952317438
+0.420488743117453,0.63,0.0,56.0,-0.00037829988884861246,0.0003613279254480588,-0.000721082930173051,0.0007091072320409
+0.420488743117453,0.69,0.0,108.0,-0.0002623177498679592,0.00023743610860454278,-0.0005680845806887494,0.0004684532294619166
+0.420488743117453,0.75,0.0,90.0,-0.0003872382972883343,0.00029751679280597875,-0.0008365960953338088,0.0005446084089572488
+0.420488743117453,0.81,0.0,36.0,-0.00034766304917670617,0.00023560568401242489,-0.0007748267399830792,0.0004285023766674814
+0.5342117500109828,0.27,0.0,12.0,-0.0034326481076563282,0.004347245238352796,-0.006283596703369399,0.008915315810740652
+0.5342117500109828,0.33,0.0,26.0,-0.0020579729139875652,0.0021795055762662344,-0.004039141929632754,0.004268888942559837
+0.5342117500109828,0.39,0.0,30.0,-0.0014694051099422235,0.001338564985039201,-0.0028179950746761912,0.0027738878331145032
+0.5342117500109828,0.45,0.0,47.0,-0.00099369981717946,0.0009308197946084582,-0.001838336638330258,0.0018862854058937781
+0.5342117500109828,0.51,0.0,47.0,-0.0010029432169209088,0.0009488118909373983,-0.0019056486331515327,0.0019586457224616783
+0.5342117500109828,0.57,0.0,47.0,-0.0006504964613294477,0.0006140067385257691,-0.0012114163412551985,0.0012148359256678495
+0.5342117500109828,0.63,0.0,60.0,-0.0004559244325663706,0.0004988121341979943,-0.0009568572607559747,0.0009178351890096054
+0.5342117500109828,0.69,0.0,109.0,-0.0004250235341418504,0.0003370521710111692,-0.0008703292649786528,0.0006276291543947784
+0.5342117500109828,0.75,0.0,85.0,-0.0003192182668301246,0.00032630524794648326,-0.0006210503689510497,0.0006535615430226667
+0.5342117500109828,0.81,0.0,34.0,-0.00033084508632006256,0.0001981776881172711,-0.0007445484155203563,0.00035402539051629037
+0.678691638054313,0.27,0.0,15.0,-0.003041884394513548,0.0043993002942417396,-0.0060467954284330345,0.009296429509107014
+0.678691638054313,0.33,0.0,24.0,-0.0024254538074686763,0.0025993105005544196,-0.004771713351882953,0.004937618528762218
+0.678691638054313,0.39,0.0,36.0,-0.0017048005134258754,0.0016371790438029523,-0.0033266422695117357,0.0032122465510663447
+0.678691638054313,0.45,0.0,45.0,-0.0011215537920244865,0.0011240387505608003,-0.0021895473983151725,0.002212430691916979
+0.678691638054313,0.51,0.0,46.0,-0.0012608935952027076,0.001140234824239417,-0.0024374675123955275,0.002298773288264328
+0.678691638054313,0.57,0.0,51.0,-0.0006773371845381798,0.0007256507513144606,-0.0013640017277478317,0.001376467577742168
+0.678691638054313,0.63,0.0,58.0,-0.0005996368896890402,0.0005756696945219071,-0.0011919692027830891,0.0011855172020900173
+0.678691638054313,0.69,0.0,114.0,-0.0005056870511198562,0.0003938568440299653,-0.0009960129112427474,0.0007569091127313915
+0.678691638054313,0.75,0.0,76.0,-0.0004185370534338884,0.0004310807855071418,-0.000789418062924632,0.0008638551458617101
+0.678691638054313,0.81,0.0,32.0,-0.00041460463262408154,0.00025489200421748893,-0.0009365735337875025,0.000444021839640311
+0.8622467393414543,0.27,0.0,19.0,-0.0034046623495080537,0.004191010979061386,-0.006282207460509898,0.008786524745029565
+0.8622467393414543,0.33,0.0,20.0,-0.0025412534004300995,0.002823889080436635,-0.004918697200771884,0.005869432105306151
+0.8622467393414543,0.39,0.0,41.0,-0.0018807412587571663,0.0018927386510019337,-0.0038064985296172764,0.0036751627094662957
+0.8622467393414543,0.45,0.0,49.0,-0.0013298028743016948,0.0013354513812840238,-0.002758260554100713,0.002589433702747376
+0.8622467393414543,0.51,0.0,40.0,-0.0015101677250070665,0.001424568323984336,-0.002893286988024571,0.0028964201438288896
+0.8622467393414543,0.57,0.0,54.0,-0.0008083623902378224,0.0008089080456903754,-0.0016349218126955987,0.0015809161743909977
+0.8622467393414543,0.63,0.0,53.0,-0.0006827721667983262,0.0007621621631114058,-0.0014193571557044662,0.0014751072868349397
+0.8622467393414543,0.69,0.0,119.0,-0.000546395773073189,0.0004618965948689147,-0.0011139932368654894,0.0008834829768550889
+0.8622467393414543,0.75,0.0,71.0,-0.0005702687335355516,0.0005516617315766988,-0.001101250942997568,0.001121360470050863
+0.8622467393414543,0.81,0.0,31.0,-0.000548664095239143,0.00034177438121789827,-0.00123176759952081,0.0006083582656358367
+1.0954451150103273,0.27,0.0,20.0,-0.0031656006927711145,0.0037563738501623927,-0.006070846930369755,0.007762911488308389
+1.0954451150103273,0.33,0.0,19.0,-0.0026972324136915428,0.003157264846488419,-0.0051310861593470225,0.006554674116544185
+1.0954451150103273,0.39,0.0,46.0,-0.0020480026491378187,0.0020614156338427717,-0.003886737145624127,0.0041081354356333885
+1.0954451150103273,0.45,0.0,48.0,-0.0016570661694142307,0.0016562879924158665,-0.003193731288286677,0.0032118537304613613
+1.0954451150103273,0.51,0.0,41.0,-0.0018104836114941822,0.0016474607841099815,-0.003502055764752611,0.0034261633787342344
+1.0954451150103273,0.57,0.0,50.0,-0.0010104075032799215,0.0009712010979970518,-0.001955684375373082,0.00191969125846184
+1.0954451150103273,0.63,0.0,52.0,-0.0009519202837818386,0.0008656689108896087,-0.0018178493696891895,0.0017530107786909001
+1.0954451150103273,0.69,0.0,124.0,-0.0006103154174277129,0.0005561627419439345,-0.0012132981530261413,0.0010834494882027534
+1.0954451150103273,0.75,0.0,68.0,-0.0007784620191798471,0.0007790551034005553,-0.0015587840820326952,0.001539777428432005
+1.0954451150103273,0.81,0.0,28.0,-0.0005808557862623904,0.0003339739017323851,-0.0012680523141511766,0.0006047590795551974
+1.391713004234159,0.21,0.0,7.0,-0.0037326554014266112,0.004324913366189612,-0.006895757782764411,0.008837921486606956
+1.391713004234159,0.27,0.0,18.0,-0.0027091867518186687,0.0033781093224262253,-0.004943980538307784,0.007481304492762852
+1.391713004234159,0.33,0.0,21.0,-0.002624158931957067,0.002746905836892422,-0.004665311628428016,0.005947600324936002
+1.391713004234159,0.39,0.0,43.0,-0.00220054391170018,0.0021209063550846866,-0.004121735392751734,0.004140127861770381
+1.391713004234159,0.45,0.0,52.0,-0.0016077782257030602,0.0016207703806908347,-0.003289903916968268,0.0030288204456781717
+1.391713004234159,0.51,0.0,38.0,-0.001954375435564743,0.001822592553793471,-0.0038393100646067256,0.00370239099356441
+1.391713004234159,0.57,0.0,48.0,-0.0012257106057096008,0.001063878407349588,-0.002364083089655715,0.0021799971898025213
+1.391713004234159,0.63,0.0,56.0,-0.0009362669488348911,0.0009148371998731787,-0.001877873969085012,0.0018314316290392388
+1.391713004234159,0.69,0.0,118.0,-0.0006771659050784898,0.0006315534088279902,-0.001351564496274517,0.0012160996076247454
+1.391713004234159,0.75,0.0,70.0,-0.0007362077890007312,0.0007713829540770048,-0.0014974753839416214,0.0014808121350152177
+1.391713004234159,0.81,0.0,28.0,-0.0005641773797975604,0.00039163840455284514,-0.0012798693061102833,0.000722384037788849
+1.7681078308849942,0.21,0.0,6.0,-0.0040668165810938866,0.004186630283036175,-0.0076172438565199245,0.008024960564546694
+1.7681078308849942,0.27,0.0,20.0,-0.001929608653264671,0.002295419746966074,-0.0036859230295385277,0.004907572119406984
+1.7681078308849942,0.33,0.0,25.0,-0.0023970779575311304,0.002428934851234698,-0.004562829183105611,0.004826698908745555
+1.7681078308849942,0.39,0.0,36.0,-0.00211296512595327,0.0022479433019746463,-0.004131016511620587,0.004394176987511492
+1.7681078308849942,0.45,0.0,53.0,-0.0015204834723954834,0.0014404708252783738,-0.002866440732628814,0.002932330239314574
+1.7681078308849942,0.51,0.0,37.0,-0.001710464357999012,0.0016740213674954266,-0.0033212129156442527,0.0033550946851065343
+1.7681078308849942,0.57,0.0,41.0,-0.001384062795301894,0.0012322301476962148,-0.002686002463791814,0.0024879503755134477
+1.7681078308849942,0.63,0.0,71.0,-0.0010035725422154165,0.0008974601661309726,-0.001905897141247482,0.0018275478957986658
+1.7681078308849942,0.69,0.0,112.0,-0.0008087516393716835,0.0007826246528652407,-0.0016434447151732919,0.0014475104701250393
+1.7681078308849942,0.75,0.0,75.0,-0.0008522734122022236,0.0007936879186911238,-0.0016577220826490516,0.0016089603741909868
+1.7681078308849942,0.81,0.0,23.0,-0.0008769255964983282,0.000604665476945411,-0.001844767218968636,0.0011189960348696529
+2.246300273206922,0.21,0.0,7.0,-0.004177419674129831,0.0031999521546861903,-0.008597656578150654,0.005797321234656344
+2.246300273206922,0.27,0.0,21.0,-0.0023112201010542024,0.0021848429434644817,-0.004595183412160135,0.004282712408350901
+2.246300273206922,0.33,0.0,33.0,-0.0022019481577527956,0.0021578935683700846,-0.0041026958212661705,0.004206292063077782
+2.246300273206922,0.39,0.0,33.0,-0.0020981593938953526,0.0020512421498059,-0.003966050223304478,0.004253948132972346
+2.246300273206922,0.45,0.0,50.0,-0.001458999996892421,0.0014504725553804347,-0.002835723817850715,0.0029144387458009103
+2.246300273206922,0.51,0.0,37.0,-0.0016097889662110092,0.0016662428218413138,-0.0031437232412708195,0.003179014949515584
+2.246300273206922,0.57,0.0,37.0,-0.0015532281164614423,0.001567685860452517,-0.003117043912955351,0.002991644885337806
+2.246300273206922,0.63,0.0,73.0,-0.0011733359532628833,0.0011420813449199798,-0.0022707180991095957,0.0022597716379984573
+2.246300273206922,0.69,0.0,104.0,-0.0010558194761250707,0.0010244198645044053,-0.002160251248840702,0.001962124226692687
+2.246300273206922,0.75,0.0,86.0,-0.0011868155890170926,0.0010888102070844303,-0.0024317947033461306,0.002061611985731862
+2.246300273206922,0.81,0.0,17.0,-0.0016573027045802052,0.0011655232702239954,-0.0034658910584156348,0.002147113207071495
+2.8538219384978865,0.21,0.0,11.0,-0.0025436620730526624,0.0027293415392826113,-0.0049037341789247724,0.005263532054223572
+2.8538219384978865,0.27,0.0,24.0,-0.0022934222510193345,0.0024517153857406323,-0.004715505886436312,0.004594324127093003
+2.8538219384978865,0.33,0.0,32.0,-0.0021444416812261033,0.002095254605614247,-0.004254702769428687,0.004141634385981562
+2.8538219384978865,0.39,0.0,43.0,-0.002097594206293578,0.001973555288578306,-0.004168631442834116,0.00375898969780292
+2.8538219384978865,0.45,0.0,43.0,-0.001621532351489908,0.0016741699511454808,-0.003158439285048852,0.003378243496096412
+2.8538219384978865,0.51,0.0,41.0,-0.0016830019241526979,0.001606417360193516,-0.0032584556683920326,0.0033572140156246694
+2.8538219384978865,0.57,0.0,52.0,-0.0013969478392826737,0.0013843501311478629,-0.0028894129715391816,0.002621920636215692
+2.8538219384978865,0.63,0.0,71.0,-0.001137395108798665,0.001170286892089105,-0.0022310526514177026,0.0023202422639505317
+2.8538219384978865,0.69,0.0,110.0,-0.0010801501220515086,0.001008500932688007,-0.0022015280925823406,0.0019758806638924885
+2.8538219384978865,0.75,0.0,64.0,-0.0009650412944337286,0.0008553553324963667,-0.001893834858689974,0.001748674794110703
+2.8538219384978865,0.81,0.0,7.0,-0.0016819391323829455,0.0015383065836188493,-0.00322591145934251,0.003028592712284395
+3.6256504768281146,0.15,0.0,5.0,-0.0024271185048504447,0.0038078554490425407,-0.0038078554490425407,0.008462304514609342
+3.6256504768281146,0.21,0.0,15.0,-0.0027538345219646375,0.0034791432711715206,-0.005134181387898781,0.0070325833938956065
+3.6256504768281146,0.27,0.0,28.0,-0.0021725219536458808,0.0022262401888065134,-0.00438573247288649,0.004330395779160449
+3.6256504768281146,0.33,0.0,39.0,-0.002309885734322173,0.0022860551342116925,-0.004584280433721684,0.004641684717198606
+3.6256504768281146,0.39,0.0,50.0,-0.0023190061293844448,0.00218958823157708,-0.0044710537339160295,0.004307358943868211
+3.6256504768281146,0.45,0.0,53.0,-0.0021270964750271662,0.0020642412441757383,-0.004208133384894715,0.004020943320379492
+3.6256504768281146,0.51,0.0,57.0,-0.0022354816447334603,0.002145593296935973,-0.0045141242913219895,0.004153551803630685
+3.6256504768281146,0.57,0.0,37.0,-0.0027069217877952185,0.0027416016585096693,-0.005161088497724632,0.005503294700609588
+3.6256504768281146,0.63,0.0,92.0,-0.0012310425917124307,0.0011630173183322132,-0.002384366424757414,0.0022082689575161833
+3.6256504768281146,0.69,0.0,83.0,-0.001023513180618154,0.001107784059714224,-0.002093717041869019,0.0022016818456721977
+3.6256504768281146,0.75,0.0,40.0,-0.0009284442201838241,0.0008789457432463205,-0.0017217106440515363,0.0017966144352780026
+4.606223395648531,0.15,0.0,5.0,-0.0018878434365432457,0.0019003252329394375,-0.003397059047047035,0.0037400128535719722
+4.606223395648531,0.21,0.0,23.0,-0.0018639430393224752,0.0016925362523589028,-0.0036206252625864445,0.0033786162853694313
+4.606223395648531,0.27,0.0,37.0,-0.0018249655279961984,0.002119129524954578,-0.003763610558280982,0.00417294398741092
+4.606223395648531,0.33,0.0,55.0,-0.0021123657481500746,0.0019816348496485775,-0.004164467321185218,0.00407379957332916
+4.606223395648531,0.39,0.0,52.0,-0.002579723081050794,0.0024889706799851186,-0.0051082283710543784,0.004850927167236974
+4.606223395648531,0.45,0.0,41.0,-0.0032248254435091653,0.0028214493010931866,-0.006522300388875692,0.005579179448594442
+4.606223395648531,0.51,0.0,48.0,-0.002909213148530393,0.0025268499967249073,-0.005569461472128024,0.00498764240935911
+4.606223395648531,0.57,0.0,45.0,-0.0032595007604201694,0.002898468031338379,-0.006493153620954295,0.005737402000824645
+4.606223395648531,0.63,0.0,88.0,-0.0014701931042174084,0.0014605733655016285,-0.002889302162415846,0.002857808565567137
+4.606223395648531,0.69,0.0,82.0,-0.0012858062212311513,0.0012863180237129962,-0.002481779359692841,0.0025234384552873346
+4.606223395648531,0.75,0.0,24.0,-0.002120191869988792,0.0021052442633107487,-0.004230407910508599,0.003935803817489427
+5.85199651930643,0.15,0.0,8.0,-0.005479000484205077,0.005680104250481232,-0.010732132640969255,0.010707612328679894
+5.85199651930643,0.21,0.0,30.0,-0.002316485403627069,0.0022101047101453605,-0.004767953605708273,0.0042052418727661625
+5.85199651930643,0.27,0.0,38.0,-0.002877675713586701,0.0029809655985844363,-0.005639984385979861,0.005728494685681789
+5.85199651930643,0.33,0.0,57.0,-0.002370606792166885,0.002186918961005441,-0.004503716662726937,0.004141165925671944
+5.85199651930643,0.39,0.0,55.0,-0.0028310147050387697,0.0028857048772083682,-0.005713316427201814,0.005568272317070403
+5.85199651930643,0.45,0.0,49.0,-0.003305173695404673,0.003189976576393847,-0.006846303342913248,0.006056653577636253
+5.85199651930643,0.51,0.0,48.0,-0.0032361576724961334,0.002893167911212997,-0.0065219200349977535,0.00571395012739602
+5.85199651930643,0.57,0.0,54.0,-0.002554099563719374,0.0022611627919655753,-0.005298672795239496,0.004220367546606756
+5.85199651930643,0.63,0.0,97.0,-0.0017773913980844906,0.0018823268645606298,-0.003689002910460654,0.0036371270180333816
+5.85199651930643,0.69,0.0,55.0,-0.0021044130770453582,0.002146639271446641,-0.00409443002751848,0.004278711273456631
+5.85199651930643,0.75,0.0,9.0,-0.003226837583395629,0.002769587289581796,-0.0071507476631701514,0.0049233101831463065
+7.434694395049637,0.15,0.0,13.0,-0.0044688093169098185,0.004451782224816163,-0.008229632308932658,0.008829390025564153
+7.434694395049637,0.21,0.0,34.0,-0.0027531364084412368,0.002586008119491032,-0.005510247956555332,0.005103577605335982
+7.434694395049637,0.27,0.0,59.0,-0.0023436509196579887,0.00196503168654896,-0.004388859944903454,0.004147639725802483
+7.434694395049637,0.33,0.0,59.0,-0.0029961150302121233,0.002815967107491811,-0.005712680534918818,0.005654961156357654
+7.434694395049637,0.39,0.0,58.0,-0.0036886065123699573,0.0032348644730549356,-0.007418130503300849,0.006301258312339435
+7.434694395049637,0.45,0.0,50.0,-0.003940256642172051,0.003615018764418708,-0.008220076794739697,0.00668736783375951
+7.434694395049637,0.51,0.0,50.0,-0.004011773761492228,0.0028871727296014924,-0.007850429179371994,0.005621433302496608
+7.434694395049637,0.57,0.0,74.0,-0.0029920521903580577,0.002704123493429603,-0.006086744276658887,0.005570077845204632
+7.434694395049637,0.63,0.0,64.0,-0.003138325206706999,0.0030650599811292674,-0.006254587963856595,0.005789757501636835
+7.434694395049637,0.69,0.0,33.0,-0.003730424829357435,0.004252444122166958,-0.006779193745259467,0.008971542799648137
+7.434694395049637,0.75,0.0,6.0,-0.005250123801230133,0.003761854741763345,-0.01192413122296163,0.006299500400540651
+9.4454397854518,0.15,0.0,21.0,-0.0033826116276215266,0.0034496473687664316,-0.006518924132556415,0.007230270977868115
+9.4454397854518,0.21,0.0,44.0,-0.0030571114660209206,0.003147134791315705,-0.006295131528395885,0.005927657422327419
+9.4454397854518,0.27,0.0,57.0,-0.0031077736528238565,0.0032117953343487222,-0.006263706069507161,0.0062795792717028915
+9.4454397854518,0.33,0.0,77.0,-0.0032799955962475725,0.003372794823231166,-0.0063525217048269154,0.006527137130899377
+9.4454397854518,0.39,0.0,58.0,-0.003468545152480688,0.0033126521640772116,-0.006937499278419372,0.006603932824352291
+9.4454397854518,0.45,0.0,61.0,-0.003432487222837081,0.0031871026566654835,-0.0071044177667219394,0.006204846988772392
+9.4454397854518,0.51,0.0,48.0,-0.0031997412051943037,0.003220574562987746,-0.006667497273373932,0.005953914437314907
+9.4454397854518,0.57,0.0,64.0,-0.0039760020683784715,0.003710070931817321,-0.007980974897688177,0.007205019113916259
+9.4454397854518,0.63,0.0,53.0,-0.0030770306245681872,0.0031504461292774883,-0.006059066669064462,0.0062168363652220894
+9.4454397854518,0.69,0.0,13.0,-0.005582939843349598,0.006380994118643633,-0.010698329638282994,0.012717006456206765
+12.000000000000009,0.15,0.0,22.0,-0.004131842298703033,0.004004348134843337,-0.008084829839053478,0.007913774401266687
+12.000000000000009,0.21,0.0,53.0,-0.003541742332891243,0.003519379823361593,-0.006879718341776284,0.006841298937109732
+12.000000000000009,0.27,0.0,73.0,-0.003534434612433418,0.0035838642494055756,-0.006973254728071912,0.006827800359525148
+12.000000000000009,0.33,0.0,75.0,-0.0037354512581132034,0.0036720582798629763,-0.007250608672521921,0.007373176313015508
+12.000000000000009,0.39,0.0,58.0,-0.004110864112281992,0.0037938459051556415,-0.008475240330814685,0.007306864221674123
+12.000000000000009,0.45,0.0,65.0,-0.0033803410925892933,0.0027450100366372865,-0.006720426345211365,0.005514606602788141
+12.000000000000009,0.51,0.0,54.0,-0.004871190514952335,0.004881245053511427,-0.009758893912417651,0.009342382653764083
+12.000000000000009,0.57,0.0,46.0,-0.004497514649813838,0.004459464088161194,-0.008629933061741816,0.00846605287399943
+12.000000000000009,0.63,0.0,35.0,-0.005356085162114714,0.004948129766033105,-0.010415485124071458,0.00946599983299847
+12.000000000000009,0.69,0.0,12.0,-0.008324279544066107,0.01008914075489049,-0.015927945362770028,0.020581027038993772
+0.0999999999999997,0.27,0.125,14.0,-0.00015147505541719658,0.0001828957763086969,-0.00027126521404419857,0.00042958321455135627
+0.0999999999999997,0.33,0.125,20.0,-0.0001485945781792029,0.00012353636880034938,-0.0003012712499580436,0.0002461088791684258
+0.0999999999999997,0.39,0.125,34.0,-0.00012100592727590767,0.0001544770729844546,-0.0002263267716343893,0.0003226870777327833
+0.0999999999999997,0.45,0.125,46.0,-0.00010567841684980798,0.00012252004317682454,-0.00019194925388314144,0.0002561783216313341
+0.0999999999999997,0.51,0.125,49.0,-0.000105664159593827,0.00012396932124756314,-0.00019372683664273667,0.0002609088389110856
+0.0999999999999997,0.57,0.125,56.0,-8.826855148765404e-05,0.00011057850726371314,-0.00017252717808682836,0.00023563541854390032
+0.0999999999999997,0.63,0.125,69.0,-8.212151056708074e-05,0.0001004696151544536,-0.00015282924034784647,0.00019659199927355098
+0.0999999999999997,0.69,0.125,103.0,-5.678144532170279e-05,6.756430575086659e-05,-0.00010984934933599104,0.00013502528007948504
+0.0999999999999997,0.75,0.125,76.0,-0.00010676278419269695,0.00011900597693126946,-0.00021412202352294886,0.00022639470485899063
+0.0999999999999997,0.81,0.125,29.0,-0.00016258277995688901,8.487196545762451e-05,-0.000375820931277072,0.00016417230402209133
+0.1270454343320539,0.27,0.125,14.0,-0.0002241945751644419,0.00032112881276966164,-0.00043213557317157584,0.0006135359933024507
+0.1270454343320539,0.33,0.125,20.0,-0.00022035612300028279,0.00018974801478905724,-0.0004511302785246156,0.00037424662108989355
+0.1270454343320539,0.39,0.125,34.0,-0.0001558600019215682,0.00018183707443854036,-0.0002978342477008314,0.0003708173625172659
+0.1270454343320539,0.45,0.125,46.0,-0.00014164990944158954,0.00015373969022819238,-0.00025625667229218867,0.00030822163164347354
+0.1270454343320539,0.51,0.125,50.0,-0.00012263025354330499,0.0001478162990096856,-0.00022993192067713802,0.0003034969760387134
+0.1270454343320539,0.57,0.125,55.0,-0.00011270389794796992,0.00012326641169297227,-0.00020511594815501378,0.00025866779578568146
+0.1270454343320539,0.63,0.125,69.0,-8.536682818621872e-05,0.00010298739676674524,-0.00016948371874676258,0.00019782552162506147
+0.1270454343320539,0.69,0.125,103.0,-5.5802884228397254e-05,6.730924955394924e-05,-0.00011226244514022374,0.00013664013139085896
+0.1270454343320539,0.75,0.125,76.0,-0.00011187208285269152,0.00012053448741251529,-0.0002215355481876053,0.00023334569743361746
+0.1270454343320539,0.81,0.125,29.0,-0.00016501687898700802,8.873011093118699e-05,-0.00039420914311777346,0.00016907641272738023
+0.1614054238462106,0.27,0.125,14.0,-0.00036433739689364144,0.000464812242526021,-0.0006794097315575182,0.000980910552056531
+0.1614054238462106,0.33,0.125,22.0,-0.000326206928908084,0.00027103698243659247,-0.0006616253317572544,0.0005128124194119714
+0.1614054238462106,0.39,0.125,33.0,-0.00023496482910290384,0.00024031719556152445,-0.0004410100607546702,0.0005207652545919373
+0.1614054238462106,0.45,0.125,45.0,-0.00019413880261403326,0.00022280461026614873,-0.00039346016236666774,0.00042115994632298
+0.1614054238462106,0.51,0.125,50.0,-0.00016133973276515255,0.00018722000559412964,-0.0003192782414177174,0.00038329402212614223
+0.1614054238462106,0.57,0.125,55.0,-0.00013669471304757444,0.0001609552090786814,-0.0002602773689014122,0.0003285746455815683
+0.1614054238462106,0.63,0.125,69.0,-0.00010653573125137408,0.00011882911494767784,-0.00019700558798751183,0.0002476356719191398
+0.1614054238462106,0.69,0.125,103.0,-6.959335793248786e-05,7.505399091907084e-05,-0.00013591958132462036,0.00015318554020765483
+0.1614054238462106,0.75,0.125,76.0,-0.00012226493998551813,0.00013053398547985105,-0.00022782417063837,0.00025420760983351637
+0.1614054238462106,0.81,0.125,29.0,-0.00017633717656640748,9.868922774197941e-05,-0.00042014711603004907,0.00018785381258906527
+0.2050582217609065,0.27,0.125,14.0,-0.0005339721609900958,0.0006847241800504045,-0.0009904145315416544,0.0013960898434821052
+0.2050582217609065,0.33,0.125,24.0,-0.00047988836431151887,0.00040099801620495113,-0.0009612411555568862,0.0007447930693660054
+0.2050582217609065,0.39,0.125,31.0,-0.00037999488903541504,0.0004048472307594038,-0.0007464973349618867,0.0007583057506324354
+0.2050582217609065,0.45,0.125,50.0,-0.0002926913481551526,0.0003034657477775603,-0.0005805117560760029,0.0006236434422130442
+0.2050582217609065,0.51,0.125,46.0,-0.00023268526739224832,0.00025919039817822327,-0.00044589573784883485,0.0005176483815377948
+0.2050582217609065,0.57,0.125,54.0,-0.00019849425139190638,0.0002100977691000204,-0.00036586873125463664,0.0004558596940998003
+0.2050582217609065,0.63,0.125,68.0,-0.00013960396615404717,0.00016134673926960878,-0.00026623580003250306,0.00031598980435743735
+0.2050582217609065,0.69,0.125,104.0,-0.00010927700340340983,0.00010369555032655524,-0.0002245520713563875,0.00019687051312025037
+0.2050582217609065,0.75,0.125,76.0,-0.00014004124383136288,0.00015332562463767107,-0.000278795637551713,0.0003025330284261224
+0.2050582217609065,0.81,0.125,29.0,-0.00020730972915310034,0.00012684823000811424,-0.00047617514838793845,0.00022267729388235395
+0.2605171084697262,0.27,0.125,14.0,-0.0007828401281809138,0.0009671838061819596,-0.0014510499700687782,0.00198221848844956
+0.2605171084697262,0.33,0.125,26.0,-0.0006788502132411632,0.0006191549473535825,-0.001465764674848224,0.001155568799960139
+0.2605171084697262,0.39,0.125,31.0,-0.0005215511542659471,0.0005065466282808523,-0.0010241405225996528,0.000986292108157305
+0.2605171084697262,0.45,0.125,49.0,-0.0004071424817902886,0.0004206013032170061,-0.0008367195452475049,0.0008162242557601737
+0.2605171084697262,0.51,0.125,45.0,-0.0002960549629069852,0.0003400710089641283,-0.0005759850843044505,0.0006783460098631729
+0.2605171084697262,0.57,0.125,53.0,-0.00025091791037519485,0.0002720416379440988,-0.000496825978105738,0.0005504240225577004
+0.2605171084697262,0.63,0.125,67.0,-0.0001698070484908596,0.0001960405527644987,-0.0003356715497677386,0.000376644615815683
+0.2605171084697262,0.69,0.125,104.0,-0.00016000028793266267,0.00012502257720983518,-0.0003305350334945181,0.00023232554212059575
+0.2605171084697262,0.75,0.125,80.0,-0.00016398991498754164,0.00016794881231931296,-0.0003110430627491138,0.00032859413140288795
+0.2605171084697262,0.81,0.125,27.0,-0.00024009164096918406,0.00014596899884872051,-0.0005196886846778761,0.00026860086585310305
+0.3309750919646937,0.27,0.125,15.0,-0.0009717236329099161,0.0012487534621310964,-0.001764910715818737,0.0025583057769769583
+0.3309750919646937,0.33,0.125,25.0,-0.0010406535670604703,0.0009378333582498151,-0.002069792032979805,0.0017682773205015343
+0.3309750919646937,0.39,0.125,35.0,-0.0007399354976229863,0.0007115601912105642,-0.0014764518605822647,0.0013749025648599929
+0.3309750919646937,0.45,0.125,46.0,-0.0005838735808271567,0.0005905202040338355,-0.0011455217951107156,0.001156521761240916
+0.3309750919646937,0.51,0.125,45.0,-0.00041767663071332853,0.0004374393833002223,-0.0008025663612467445,0.0009065098277201214
+0.3309750919646937,0.57,0.125,53.0,-0.00035947449514958353,0.00037637271411360476,-0.0006660391945002225,0.0007329160601062536
+0.3309750919646937,0.63,0.125,60.0,-0.0002496446565285841,0.0002697127606706178,-0.00048764377658256313,0.0005153495465490224
+0.3309750919646937,0.69,0.125,107.0,-0.00018823122405299363,0.00015922109955898231,-0.0004045936231932343,0.00029464380380098235
+0.3309750919646937,0.75,0.125,84.0,-0.0001876670792641352,0.00019554797590976884,-0.0003678085394300054,0.00039879141814890424
+0.3309750919646937,0.81,0.125,26.0,-0.0002915851116850681,0.00017107124370692258,-0.0006621425541334067,0.0003090019267041045
+0.4204887431174471,0.27,0.125,15.0,-0.001304348395601325,0.0015847933745940835,-0.0024022707312761726,0.00326551896511289
+0.4204887431174471,0.33,0.125,26.0,-0.0014158772204029143,0.0012559449604280756,-0.0027484104940352218,0.0024958331595671887
+0.4204887431174471,0.39,0.125,36.0,-0.0010811689674128536,0.001001570546017448,-0.0021493558648186836,0.0019629676820223244
+0.4204887431174471,0.45,0.125,46.0,-0.0007812109619469798,0.0008409387206203808,-0.0015307635843691534,0.0016168931160691804
+0.4204887431174471,0.51,0.125,43.0,-0.0006003236825010341,0.00067025621309334,-0.0012057974179858193,0.0013264148432406914
+0.4204887431174471,0.57,0.125,52.0,-0.0004976024752845064,0.0005096039917641004,-0.000993357707479045,0.001015320394047245
+0.4204887431174471,0.63,0.125,58.0,-0.0003381940906002627,0.00036862352622053486,-0.0006798416263357914,0.0007557194664991912
+0.4204887431174471,0.69,0.125,107.0,-0.00023360000791708036,0.0002211548874959636,-0.0005133685917011944,0.00039856616785625146
+0.4204887431174471,0.75,0.125,87.0,-0.00022980943036515346,0.00025031217797970615,-0.00046470242801788773,0.0004767151502697219
+0.4204887431174471,0.81,0.125,26.0,-0.000350883471260509,0.00022050120013614616,-0.0007961396892033509,0.0003998717606350369
+0.5342117500109768,0.27,0.125,15.0,-0.0017051560341153587,0.0021148187473772357,-0.003238643622060035,0.0041073425143649716
+0.5342117500109768,0.33,0.125,28.0,-0.0017452151641038636,0.0015023820068225332,-0.0032590146725648343,0.002973744531648973
+0.5342117500109768,0.39,0.125,36.0,-0.0014630417564118544,0.0014725504013085994,-0.0030415362264483137,0.002861291432984001
+0.5342117500109768,0.45,0.125,46.0,-0.0010725731202283818,0.001057862318376648,-0.002068091828253062,0.002122077371762325
+0.5342117500109768,0.51,0.125,42.0,-0.0009213820848497637,0.0008779831161939022,-0.0017698471324886721,0.0017858838677539488
+0.5342117500109768,0.57,0.125,46.0,-0.0007144428961119417,0.0007546853289778039,-0.001403133912921753,0.0014917943393283667
+0.5342117500109768,0.63,0.125,64.0,-0.0004522777613577228,0.00046550303895524287,-0.0008869812271946673,0.0009231434539731789
+0.5342117500109768,0.69,0.125,100.0,-0.0003442893675323987,0.0002925267936924794,-0.0007006034526723293,0.0006172145890245595
+0.5342117500109768,0.75,0.125,92.0,-0.000299816097899065,0.0003006444876879865,-0.000578777263888649,0.0005959729922539928
+0.5342117500109768,0.81,0.125,27.0,-0.0005554762541966026,0.000431919566780327,-0.0012092133531719548,0.0007631765121204292
+0.6786916380543256,0.27,0.125,15.0,-0.002215947509242777,0.0024681065069314416,-0.00456474883301244,0.004625477305926596
+0.6786916380543256,0.33,0.125,27.0,-0.0020359546790563996,0.0019717184457898377,-0.0041725258713763555,0.003849251851698894
+0.6786916380543256,0.39,0.125,37.0,-0.0018874764086803959,0.0016829833146471563,-0.0037317878622476325,0.0032760663284790038
+0.6786916380543256,0.45,0.125,46.0,-0.0011977455949599113,0.0013324363210157142,-0.0025372438083053877,0.0025616320433524712
+0.6786916380543256,0.51,0.125,41.0,-0.0010735623255735246,0.0010560612487217715,-0.002050991914471546,0.002075879674213711
+0.6786916380543256,0.57,0.125,45.0,-0.000886917374230789,0.0009279246691663251,-0.0017400065039035835,0.001788910035808721
+0.6786916380543256,0.63,0.125,63.0,-0.000563198957550434,0.0006073142599586326,-0.001101865734774823,0.001204309398294217
+0.6786916380543256,0.69,0.125,93.0,-0.00044847503439815673,0.00044937975178656743,-0.0009532833610593177,0.0008310142236500021
+0.6786916380543256,0.75,0.125,104.0,-0.0003777632892426824,0.0003880637064870058,-0.0007065022416638759,0.0007733236390701689
+0.6786916380543256,0.81,0.125,24.0,-0.00083321354505403,0.0005881431443374651,-0.0016624996070627026,0.0011379453698794825
+0.8622467393414558,0.21,0.125,6.0,-0.0023115587273721734,0.0018419611551491553,-0.0047183463668914105,0.0032075348860881032
+0.8622467393414558,0.27,0.125,14.0,-0.003030667127609233,0.003035662611819852,-0.005712733283992016,0.006010676863414581
+0.8622467393414558,0.33,0.125,29.0,-0.0023645671727853335,0.002172716949411023,-0.004752565980216461,0.004078339592061453
+0.8622467393414558,0.39,0.125,35.0,-0.0023070556664064237,0.0018855242075737255,-0.004579323655109793,0.003688118129271567
+0.8622467393414558,0.45,0.125,47.0,-0.0014612812849810488,0.0014771053556173386,-0.0028255146043288724,0.002820197128120546
+0.8622467393414558,0.51,0.125,39.0,-0.001365975200967869,0.0013712830151751368,-0.0027016509828896923,0.0026143199118423576
+0.8622467393414558,0.57,0.125,45.0,-0.0010989910196941071,0.0010876775618062864,-0.002023519497314985,0.0021489872692426774
+0.8622467393414558,0.63,0.125,59.0,-0.0007451425400217947,0.000813490210782186,-0.0014745952246588022,0.0015717175806383345
+0.8622467393414558,0.69,0.125,88.0,-0.0005563407071015415,0.0005906502897813325,-0.00110540915982957,0.0011380789898791475
+0.8622467393414558,0.75,0.125,113.0,-0.0005556059278914457,0.0005617120337319649,-0.0010894243370644183,0.001087959086762282
+0.8622467393414558,0.81,0.125,24.0,-0.0012227735378157313,0.0009511351727535834,-0.002505912107294347,0.0017635971395631325
+1.09544511501034,0.21,0.125,7.0,-0.0033668155695008666,0.0027739408720188286,-0.006785137122305139,0.005210490742303223
+1.09544511501034,0.27,0.125,16.0,-0.0033541975069520153,0.0031477997668650864,-0.006590900543348758,0.0062090656667644906
+1.09544511501034,0.33,0.125,29.0,-0.0025401803312397305,0.0022222073824446453,-0.0050051875160087985,0.004266592676140474
+1.09544511501034,0.39,0.125,32.0,-0.0027809471824673973,0.0023322889383140043,-0.005657755314277252,0.004658689205059988
+1.09544511501034,0.45,0.125,49.0,-0.001712600375864046,0.0016632108710218278,-0.0034814131006928647,0.0031487515494768195
+1.09544511501034,0.51,0.125,39.0,-0.0015664624621559886,0.0015479599708046543,-0.003215181064758746,0.0029611144424378107
+1.09544511501034,0.57,0.125,44.0,-0.001293122289587012,0.001271818270367215,-0.002636173506176938,0.002509228583845762
+1.09544511501034,0.63,0.125,54.0,-0.0011135277540764731,0.0011141213387948986,-0.0021370428773052792,0.002180589353042543
+1.09544511501034,0.69,0.125,81.0,-0.000791844949986758,0.0008048890551789824,-0.001549024999024505,0.001606690947928593
+1.09544511501034,0.75,0.125,113.0,-0.0008093035806836414,0.0007723548571391403,-0.0015310705351970846,0.001543217354390705
+1.09544511501034,0.81,0.125,34.0,-0.0011953668438974662,0.001278990792269791,-0.0024710785966163503,0.0023835669936777414
+1.3917130042341723,0.21,0.125,7.0,-0.003477164510565646,0.002787913920698684,-0.007010877819937969,0.005039334949262454
+1.3917130042341723,0.27,0.125,18.0,-0.0032306212903350203,0.003153394380384728,-0.006706188180559738,0.005865244196131744
+1.3917130042341723,0.33,0.125,34.0,-0.0025524429191040496,0.0022176763051845734,-0.005276343110116947,0.004406046526435405
+1.3917130042341723,0.39,0.125,30.0,-0.0027167207356761014,0.0023670988040021524,-0.0056751224985790785,0.004396579608798624
+1.3917130042341723,0.45,0.125,46.0,-0.001897709106113774,0.0018452719066905075,-0.00382583863926469,0.00353879110046676
+1.3917130042341723,0.51,0.125,39.0,-0.0016364876815079133,0.0017410795186295887,-0.0033749653137093143,0.00324999555412483
+1.3917130042341723,0.57,0.125,42.0,-0.0014906975029303794,0.0015152385457310685,-0.0030369430863199627,0.00296634065123428
+1.3917130042341723,0.63,0.125,53.0,-0.0014092582522624386,0.0013001784328862422,-0.002679018734730565,0.0026237454328621452
+1.3917130042341723,0.69,0.125,78.0,-0.0009556992860647406,0.0009868449624106667,-0.0018637191205504089,0.0019125080032345084
+1.3917130042341723,0.75,0.125,118.0,-0.0009565149711080114,0.0009287996301819886,-0.0018452120197017697,0.0018923686608032725
+1.3917130042341723,0.81,0.125,33.0,-0.001457548179955614,0.001432037998091456,-0.002845794055930471,0.0028230496068694477
+1.7681078308849818,0.21,0.125,8.0,-0.0020754851682640674,0.002276821752711669,-0.0041860321747675495,0.004392894756935911
+1.7681078308849818,0.27,0.125,19.0,-0.0029940889921472886,0.002808257573155126,-0.005962608283896585,0.0055652790118981815
+1.7681078308849818,0.33,0.125,34.0,-0.002325938931900824,0.0019948983741387813,-0.004578392860389947,0.0038659309058942386
+1.7681078308849818,0.39,0.125,37.0,-0.002178549699205912,0.0020975775666846877,-0.004502176471638837,0.003939086686460133
+1.7681078308849818,0.45,0.125,48.0,-0.0017152631502193594,0.0017441395041777365,-0.00346946703483552,0.0033154266778309314
+1.7681078308849818,0.51,0.125,35.0,-0.0019201450825125622,0.001925852804621928,-0.00382584611383182,0.0036239807223020187
+1.7681078308849818,0.57,0.125,44.0,-0.0016184062774849232,0.0015709580883480614,-0.0032738474997371573,0.003048359940801322
+1.7681078308849818,0.63,0.125,57.0,-0.001298302457447353,0.0012936575640998278,-0.0026384893188548405,0.002576105071643808
+1.7681078308849818,0.69,0.125,100.0,-0.0010048215417786553,0.0010359369233983071,-0.002084096056886987,0.0019372125928993722
+1.7681078308849818,0.75,0.125,100.0,-0.0010614215126391745,0.0010602380315174749,-0.002119036452412402,0.002041605054878303
+1.7681078308849818,0.81,0.125,16.0,-0.0023618580886106944,0.0023466065748920626,-0.004844545677127137,0.004417505699607252
+2.246300273206923,0.21,0.125,10.0,-0.0031962833742784423,0.002717467390005712,-0.0065608837767380575,0.00503096885022692
+2.246300273206923,0.27,0.125,21.0,-0.002775272755165704,0.0028394690035728302,-0.005525360193343605,0.005605186577695601
+2.246300273206923,0.33,0.125,33.0,-0.0018113221477753846,0.002094206138369803,-0.003411922478369232,0.004223902121968099
+2.246300273206923,0.39,0.125,41.0,-0.0017872388134097287,0.0019023566576082433,-0.0035816098955550324,0.003578693857011141
+2.246300273206923,0.45,0.125,52.0,-0.0016828374146841507,0.001686381234850189,-0.0033497836047842486,0.0034216670785246948
+2.246300273206923,0.51,0.125,42.0,-0.0017109251230155982,0.0016371025442732995,-0.0034062207355774923,0.0031372389868595564
+2.246300273206923,0.57,0.125,51.0,-0.0014153829511406768,0.0013800851550953269,-0.0029589348421415113,0.002580618510199941
+2.246300273206923,0.63,0.125,62.0,-0.0014475229836305582,0.0013202917489796735,-0.0027300578453224146,0.0027194622214252143
+2.246300273206923,0.69,0.125,124.0,-0.0009389124532220365,0.0009572803081239993,-0.001875124970244766,0.0018047104766965277
+2.246300273206923,0.75,0.125,57.0,-0.0012905003975288017,0.0012433847765360845,-0.0025353900412909357,0.0023197273827939603
+2.246300273206923,0.81,0.125,5.0,-0.0028800011926430223,0.00409295094556128,-0.005690349047845778,0.007579427014663432
+2.853821938497873,0.21,0.125,11.0,-0.0030091179777631477,0.0028739963488880805,-0.006042242631633404,0.005428652939028883
+2.853821938497873,0.27,0.125,24.0,-0.0025936627435090994,0.0024279838301977112,-0.005004602991465934,0.004661894635075489
+2.853821938497873,0.33,0.125,41.0,-0.0016374762224088027,0.0017714869781205525,-0.0032112740505367567,0.0034276728148018272
+2.853821938497873,0.39,0.125,43.0,-0.0018953684873464038,0.0020007143378453513,-0.0036325329672967626,0.003783718831991219
+2.853821938497873,0.45,0.125,51.0,-0.0018130526654613537,0.0018934825179055138,-0.0035369908083413386,0.0036514613518181514
+2.853821938497873,0.51,0.125,47.0,-0.0019152010135606392,0.0018303363004472182,-0.0037833426100319836,0.0035641748124019346
+2.853821938497873,0.57,0.125,52.0,-0.0017991457936729924,0.001743638096620293,-0.0036289527795506315,0.0035257425876683212
+2.853821938497873,0.63,0.125,87.0,-0.001241320356072582,0.0011788832543666611,-0.0023428970892837705,0.0022985411924174304
+2.853821938497873,0.69,0.125,101.0,-0.0008929583027991496,0.0009140525440811229,-0.0018063434922089715,0.0018432308571931714
+2.853821938497873,0.75,0.125,40.0,-0.001259353786397907,0.001291070400707831,-0.0024290736937042793,0.002519938318927148
+3.6256504768281137,0.21,0.125,20.0,-0.0019392370845274674,0.002163872007313508,-0.0041131387110078035,0.004045719219933182
+3.6256504768281137,0.27,0.125,30.0,-0.00232351724200865,0.0021918943429446638,-0.004666590722830187,0.004176127147587628
+3.6256504768281137,0.33,0.125,46.0,-0.001890039678033525,0.0018065692461501504,-0.003460934774691564,0.0037547423269919805
+3.6256504768281137,0.39,0.125,54.0,-0.0015787227058396802,0.0016048243399998698,-0.0032788192023265415,0.00305052345043422
+3.6256504768281137,0.45,0.125,47.0,-0.0017692673542116573,0.001709041048396485,-0.0035037334078239276,0.003412052304149928
+3.6256504768281137,0.51,0.125,58.0,-0.0018471759755311113,0.001620956423300505,-0.0035315879237371077,0.0032912471646926213
+3.6256504768281137,0.57,0.125,34.0,-0.0022128565725363335,0.0023419095022197325,-0.004391789590206584,0.004430036798053395
+3.6256504768281137,0.63,0.125,81.0,-0.0012874404994901662,0.0013943627331289828,-0.00267037685413178,0.0025580924771932364
+3.6256504768281137,0.69,0.125,99.0,-0.0010319918463191947,0.0009787760229828194,-0.002026115594268419,0.0019742993963057635
+3.6256504768281137,0.75,0.125,27.0,-0.0015690860179892244,0.001475177779181384,-0.002962412606514289,0.0030400690366236397
+4.606223395648542,0.15,0.125,5.0,-0.002939879442979443,0.002471822297085713,-0.00599198033996684,0.004637543630567875
+4.606223395648542,0.21,0.125,28.0,-0.001676585895457507,0.0015923531789473154,-0.0032196936893858176,0.003282789754097062
+4.606223395648542,0.27,0.125,36.0,-0.0019980035751954615,0.001950241626357394,-0.003956961131319405,0.003842073305046352
+4.606223395648542,0.33,0.125,52.0,-0.0015973488473263308,0.0017811657465524233,-0.0033506966492577385,0.0032295473356333307
+4.606223395648542,0.39,0.125,49.0,-0.0022266375160187495,0.0022097337166825637,-0.004408955662874204,0.004397447749845864
+4.606223395648542,0.45,0.125,53.0,-0.0019769249198055405,0.0018941191036085522,-0.0038309632251070304,0.0038137668544082318
+4.606223395648542,0.51,0.125,49.0,-0.0024918574715715783,0.002344753246348083,-0.004843146713123678,0.004677488847983824
+4.606223395648542,0.57,0.125,52.0,-0.0022131602788256566,0.0022076765289565296,-0.0043134654063911254,0.004369865229856876
+4.606223395648542,0.63,0.125,82.0,-0.0016011405484058024,0.0015399764957067454,-0.0030300844407109913,0.0030293163805019396
+4.606223395648542,0.69,0.125,80.0,-0.001225015773745085,0.001260977004310037,-0.002367953997573181,0.002497320762201203
+4.606223395648542,0.75,0.125,14.0,-0.0025168487605257152,0.00229483727304172,-0.005088695283594496,0.004351346258656681
+5.851996519306432,0.15,0.125,9.0,-0.0027171808320360547,0.0024332346012579382,-0.005433871140187772,0.004718185337766348
+5.851996519306432,0.21,0.125,30.0,-0.0019076305987499635,0.0017749249376845947,-0.0038359865790474255,0.003491222812419114
+5.851996519306432,0.27,0.125,47.0,-0.0019432085446424786,0.0018343633835071337,-0.0039276213008204094,0.0036885898455856266
+5.851996519306432,0.33,0.125,54.0,-0.0016624660394415972,0.0017013803428267175,-0.0033348496677868406,0.0032713902043996343
+5.851996519306432,0.39,0.125,59.0,-0.0018636473973607964,0.0019759939520096856,-0.003738049321335102,0.0037853854319303154
+5.851996519306432,0.45,0.125,50.0,-0.002368233607133056,0.0022205638474811383,-0.004659828538752888,0.00440822982265739
+5.851996519306432,0.51,0.125,45.0,-0.0027438137832959983,0.002324550488777675,-0.005163964758352847,0.0049561613855029565
+5.851996519306432,0.57,0.125,55.0,-0.002048330760253707,0.0018503601272977614,-0.004065162673134662,0.003790057195682446
+5.851996519306432,0.63,0.125,94.0,-0.001696770937642929,0.0016895107514316146,-0.0033167861616900662,0.003284284693189478
+5.851996519306432,0.69,0.125,48.0,-0.0017091963678310487,0.0018306809602918366,-0.003168572261704021,0.0037505052223212377
+5.851996519306432,0.75,0.125,9.0,-0.0031553979274596936,0.0027636837360107375,-0.006271666912523062,0.004971124339852596
+7.434694395049622,0.15,0.125,15.0,-0.00181730957059693,0.0019965808676678585,-0.003587686498469033,0.0038467373634389753
+7.434694395049622,0.21,0.125,37.0,-0.0019681552166423907,0.0019928347283305753,-0.003960040598115665,0.003849876908575199
+7.434694395049622,0.27,0.125,59.0,-0.0019212181665559987,0.001778738692390468,-0.003818768353950676,0.0034297721796990297
+7.434694395049622,0.33,0.125,60.0,-0.00210672640130535,0.0020933829064534665,-0.004337117836976367,0.003983769023800063
+7.434694395049622,0.39,0.125,60.0,-0.0023013451337037688,0.0022271225584425073,-0.0046061009454995945,0.004329390927307796
+7.434694395049622,0.45,0.125,46.0,-0.002481626445710624,0.0023855369933170846,-0.005119381728297343,0.004465565750840304
+7.434694395049622,0.51,0.125,43.0,-0.0023976809108340134,0.0022265846550129525,-0.004939106033781255,0.004253469232028044
+7.434694395049622,0.57,0.125,73.0,-0.002172078983464842,0.002229210653578707,-0.004237363600825511,0.004262406396159975
+7.434694395049622,0.63,0.125,70.0,-0.002007721962631795,0.0019098684741126058,-0.0039024261608632616,0.0038577882820213048
+7.434694395049622,0.69,0.125,30.0,-0.0025179480774719623,0.002804222511768501,-0.004891410349377743,0.005716922659298108
+7.434694395049622,0.75,0.125,7.0,-0.006610753807100333,0.004250020306328357,-0.013897505500230107,0.007634070262983349
+9.44543978545178,0.15,0.125,20.0,-0.002423012073417808,0.0020975553888638665,-0.004668711034265185,0.004207318325443813
+9.44543978545178,0.21,0.125,38.0,-0.002392201080869158,0.0021886431059201313,-0.004678831414792556,0.004433472457136739
+9.44543978545178,0.27,0.125,61.0,-0.0024802142454950957,0.0026089884915251513,-0.0051671793892071926,0.004821463202361648
+9.44543978545178,0.33,0.125,76.0,-0.0020879186793526005,0.002070287426939025,-0.003989239462113312,0.004090785319257546
+9.44543978545178,0.39,0.125,63.0,-0.002234995573230223,0.0021943127786855057,-0.004352737251879768,0.004484573308384186
+9.44543978545178,0.45,0.125,50.0,-0.002220008060759562,0.0023762863390292305,-0.004473139239800801,0.004930389402428354
+9.44543978545178,0.51,0.125,56.0,-0.0023312139502711534,0.0025542680044943894,-0.004714373780162616,0.005011587053286559
+9.44543978545178,0.57,0.125,63.0,-0.0022646159711896957,0.0022519238866682044,-0.004660513765231647,0.004267668824805253
+9.44543978545178,0.63,0.125,52.0,-0.0022860945274317105,0.0024241153910951733,-0.00459428842687757,0.004545330311563693
+9.44543978545178,0.69,0.125,17.0,-0.004987406628720824,0.004211457088832267,-0.010308961149776755,0.007662962642336185
+12.000000000000004,0.15,0.125,21.0,-0.0017819863749228455,0.0017898488719976947,-0.0034454037101238144,0.0035768973168359033
+12.000000000000004,0.21,0.125,49.0,-0.0025691632635687,0.0026806183821818583,-0.005172474251083013,0.005227682684732318
+12.000000000000004,0.27,0.125,67.0,-0.0029990243326920006,0.0030366405455811416,-0.005963714458155438,0.005926082789868002
+12.000000000000004,0.33,0.125,74.0,-0.002364827510698807,0.002078160065531272,-0.0045815448506025995,0.004380224930640815
+12.000000000000004,0.39,0.125,67.0,-0.0019676269899195848,0.0018722501396367403,-0.003865046383547238,0.003934112207982525
+12.000000000000004,0.45,0.125,62.0,-0.0022479664687142867,0.0021292059220142934,-0.004296001860934637,0.004143550991997108
+12.000000000000004,0.51,0.125,57.0,-0.0034338237457870267,0.003329905019101133,-0.00661496286393032,0.006571294156260095
+12.000000000000004,0.57,0.125,44.0,-0.003263047182396169,0.0031692391431608824,-0.00640085374120022,0.006410579416591491
+12.000000000000004,0.63,0.125,32.0,-0.003332828918054523,0.0032851205848458457,-0.00657484150176472,0.006713033480272642
+12.000000000000004,0.69,0.125,19.0,-0.006167548760063428,0.00539655043140614,-0.013018062509661739,0.010283471772452518
+0.1000000000000023,0.21,0.5,13.0,-0.00014088953560106545,0.00013685911529355942,-0.0002855015757403872,0.0002546347248003258
+0.1000000000000023,0.27,0.5,20.0,-0.00011678383930250163,0.0001048203543976331,-0.00024334450994143342,0.000190354620357037
+0.1000000000000023,0.33,0.5,31.0,-0.0001035506747714556,0.00014234927707692025,-0.0001942899052769135,0.0002951440145257229
+0.1000000000000023,0.39,0.5,46.0,-7.709937184802061e-05,0.00010165677823128983,-0.00014133689836624637,0.00020772023569701426
+0.1000000000000023,0.45,0.5,43.0,-9.552142450305504e-05,0.00012019255369494869,-0.0001764569757031221,0.0002523916937470092
+0.1000000000000023,0.51,0.5,45.0,-7.608296706250732e-05,0.00010026543829827145,-0.00014008816934857427,0.000205668466500508
+0.1000000000000023,0.57,0.5,44.0,-0.00010295654428165647,0.00011843242274397456,-0.0001919913096652644,0.00023808644037002732
+0.1000000000000023,0.63,0.5,47.0,-9.296543320046457e-05,0.00010975636910310535,-0.00017515982449522528,0.0002242483722192486
+0.1000000000000023,0.69,0.5,106.0,-5.3202882393850563e-05,5.993795112345888e-05,-9.757687834567536e-05,0.00012694760825950497
+0.1000000000000023,0.75,0.5,93.0,-7.636087167888015e-05,8.549072582511912e-05,-0.0001537699357990117,0.00016222929999954876
+0.1000000000000023,0.81,0.5,11.0,-0.000323307688024022,0.0001620829424597727,-0.0006669541416285085,0.00017405139862953353
+0.1270454343320577,0.21,0.5,13.0,-0.0002354303035248844,0.0002151927341162463,-0.0004485118111153017,0.00042741847652356767
+0.1270454343320577,0.27,0.5,20.0,-0.00018829485394485538,0.0001650024443538876,-0.00039121264763009364,0.0003176879021335334
+0.1270454343320577,0.33,0.5,31.0,-0.00013678380407181577,0.00016090696862977268,-0.00026721415138792107,0.0003289458854881233
+0.1270454343320577,0.39,0.5,47.0,-9.470918089053593e-05,0.00011776052308459624,-0.00018023339976708786,0.0002454078065590848
+0.1270454343320577,0.45,0.5,42.0,-0.00012123051620667241,0.00014146031237494779,-0.00022019662779530376,0.000293100508034287
+0.1270454343320577,0.51,0.5,46.0,-8.593022485204482e-05,0.00011465370072221249,-0.00015692299112953366,0.00024095118831659394
+0.1270454343320577,0.57,0.5,43.0,-0.00011466873757539692,0.00013094338943932043,-0.00022023747459507176,0.00026703646449581
+0.1270454343320577,0.63,0.5,48.0,-0.00010026184519505387,0.00011721022066409566,-0.0001813614691518948,0.00023403371931795516
+0.1270454343320577,0.69,0.5,105.0,-5.55418778989236e-05,6.194861616796706e-05,-0.00010282017710312765,0.00013093022867056233
+0.1270454343320577,0.75,0.5,93.0,-7.825034027625332e-05,8.11087049024205e-05,-0.00015632430563754953,0.0001611097339740855
+0.1270454343320577,0.81,0.5,11.0,-0.00032282761379132194,0.0001616639757401786,-0.0006795876847739155,0.0001782627126874129
+0.161405423846198,0.21,0.5,13.0,-0.0003736256695911168,0.00035535656482705777,-0.0006917479564626229,0.0006941550601295508
+0.161405423846198,0.27,0.5,20.0,-0.0003080839824311793,0.00027642506794588303,-0.0005836217077049445,0.0005281748022922156
+0.161405423846198,0.33,0.5,31.0,-0.00020891602065383787,0.00021839186879947753,-0.0004163505195735091,0.00045558488193726745
+0.161405423846198,0.39,0.5,48.0,-0.00013416765945054704,0.00015490244710395168,-0.0002474950910970511,0.0003371624389793191
+0.161405423846198,0.45,0.5,41.0,-0.00016417893708275738,0.0001894773103697828,-0.00030121625194054664,0.0003951159765069991
+0.161405423846198,0.51,0.5,47.0,-0.00011057661775031038,0.00013964407497997017,-0.00020703665884046711,0.0002910431584431168
+0.161405423846198,0.57,0.5,44.0,-0.0001379761191040098,0.00015071583711404846,-0.0002549200510157881,0.000314315088226364
+0.161405423846198,0.63,0.5,47.0,-0.00011469925610080663,0.000141716519359848,-0.00022959963778023044,0.00028681513270259815
+0.161405423846198,0.69,0.5,104.0,-6.555354670469459e-05,6.952281714174387e-05,-0.00011611739091981442,0.00014938616372375674
+0.161405423846198,0.75,0.5,93.0,-8.368671315568969e-05,8.686093328191897e-05,-0.00015958522155844242,0.00017890030268982227
+0.161405423846198,0.81,0.5,11.0,-0.000333306168904908,0.00016605148555098601,-0.00071482963649044,0.00019386508720311584
+0.2050582217609056,0.21,0.5,13.0,-0.0005800904065686201,0.000580275976310609,-0.0011611951318165172,0.001096825126759912
+0.2050582217609056,0.27,0.5,20.0,-0.0005033643689052059,0.0004657442683767457,-0.0010340386359911846,0.0008742826603845269
+0.2050582217609056,0.33,0.5,31.0,-0.0003386690845891666,0.0003535902385018972,-0.0006636405024697333,0.0007103744998208334
+0.2050582217609056,0.39,0.5,48.0,-0.0002079729419260711,0.0002365126805227271,-0.0003962189000498492,0.0004937003728009489
+0.2050582217609056,0.45,0.5,41.0,-0.00024268888455554593,0.0002924122852285282,-0.00046130341803642935,0.0005517245053739478
+0.2050582217609056,0.51,0.5,47.0,-0.0001611048870233562,0.000196774972534001,-0.00029911472615638503,0.000396368612761826
+0.2050582217609056,0.57,0.5,44.0,-0.00018563199833109117,0.00020486811045609775,-0.00034323665741219247,0.0004285151544849576
+0.2050582217609056,0.63,0.5,48.0,-0.0001519331754947954,0.00017291350797406571,-0.00028561930939753654,0.00036369819298470154
+0.2050582217609056,0.69,0.5,103.0,-7.644897027143928e-05,9.074888593839859e-05,-0.0001491324778235055,0.0001817170365262785
+0.2050582217609056,0.75,0.5,93.0,-0.00010017144533808062,0.00010846861117424003,-0.0001959692520064966,0.00020964435930981393
+0.2050582217609056,0.81,0.5,11.0,-0.00036107566456596853,0.00018119750133608608,-0.0008034039433065303,0.0002262050303792561
+0.260517108469725,0.21,0.5,13.0,-0.0009016226605798679,0.000906326078174892,-0.001824432991820047,0.0017354202309217337
+0.260517108469725,0.27,0.5,21.0,-0.0007942852104224498,0.000690286306238704,-0.0016439546578355356,0.0013102285428785163
+0.260517108469725,0.33,0.5,31.0,-0.000547781256084764,0.00047776242668138224,-0.0010811215541020214,0.0009429466218595264
+0.260517108469725,0.39,0.5,48.0,-0.00029681953501473697,0.0003411426761276957,-0.0006014994514118847,0.0006742747290598354
+0.260517108469725,0.45,0.5,40.0,-0.0003540296967217558,0.0003664193276801359,-0.0006681944489161217,0.0007548494203047153
+0.260517108469725,0.51,0.5,47.0,-0.00022364988742884943,0.00023594808972087663,-0.00040038094416814453,0.0005132829956243116
+0.260517108469725,0.57,0.5,47.0,-0.00022589644326648272,0.000247207419567046,-0.00044086415382221767,0.0004877390204896429
+0.260517108469725,0.63,0.5,50.0,-0.00016511515952642123,0.00019581146620758688,-0.0003199170558139534,0.00039257455687374246
+0.260517108469725,0.69,0.5,99.0,-9.159709154374731e-05,0.00010836945202951772,-0.00018343616311336774,0.00021106378343621873
+0.260517108469725,0.75,0.5,93.0,-0.00011160058477754354,0.00012050378791428428,-0.00022359400628163076,0.00023536101694537377
+0.260517108469725,0.81,0.5,10.0,-0.00029193158951209544,0.00023492287609740416,-0.0007824545629000953,0.0002703646821234474
+0.3309750919646987,0.21,0.5,13.0,-0.0014109363312373624,0.001362027600518875,-0.0029292762461283124,0.002611358160652785
+0.3309750919646987,0.27,0.5,21.0,-0.0011870545004816946,0.0010674531765338124,-0.002328205671452734,0.0021164518883395452
+0.3309750919646987,0.33,0.5,32.0,-0.0008235083878377086,0.0007171972365741751,-0.0017108964646717789,0.0013678098909669855
+0.3309750919646987,0.39,0.5,48.0,-0.00046462144856453856,0.0005007052177459787,-0.0009056762996403422,0.0009937870889762156
+0.3309750919646987,0.45,0.5,40.0,-0.0005180092561422468,0.0004943704463613369,-0.0010203783627193007,0.0009822148474376558
+0.3309750919646987,0.51,0.5,46.0,-0.00030739571652958915,0.0003505991297323301,-0.0005768407507032693,0.0007066515297850746
+0.3309750919646987,0.57,0.5,50.0,-0.0002909007014203442,0.00030474667613305617,-0.0005541288759425149,0.000620520858740517
+0.3309750919646987,0.63,0.5,54.0,-0.00020166198061800008,0.00023936040185464338,-0.000390054855796046,0.00048321837871231237
+0.3309750919646987,0.69,0.5,92.0,-0.00012363036358201989,0.0001360908794315037,-0.00023679604702495698,0.000270718199472821
+0.3309750919646987,0.75,0.5,93.0,-0.00014045084591808834,0.00013618964882617087,-0.00025952276196324,0.0002711263884443404
+0.3309750919646987,0.81,0.5,10.0,-0.0003260139559494633,0.0002579533454401675,-0.0010216289243221148,0.0003019863007684023
+0.420488743117445,0.21,0.5,13.0,-0.002082756982297899,0.001906448654321589,-0.004290816244487302,0.0036713922481136506
+0.420488743117445,0.27,0.5,21.0,-0.0017609356781686449,0.0014988078027999914,-0.0036429038565438886,0.0028016472845259345
+0.420488743117445,0.33,0.5,32.0,-0.001268981753553438,0.0011097327022097428,-0.002593233769203948,0.0021969228086104594
+0.420488743117445,0.39,0.5,48.0,-0.0007452838534365293,0.0007081439086433084,-0.0013959322990712167,0.0014433407222991482
+0.420488743117445,0.45,0.5,40.0,-0.000755587931226556,0.0006850434255765917,-0.0014542139850983237,0.001414476015954531
+0.420488743117445,0.51,0.5,47.0,-0.00044773047704859884,0.0004740187745391708,-0.0008757046663472822,0.0009447269909869573
+0.420488743117445,0.57,0.5,53.0,-0.0003652980422238975,0.0004210416688073179,-0.0007504026618877275,0.000815719032827978
+0.420488743117445,0.63,0.5,54.0,-0.0002875019088797294,0.0003085512693607745,-0.0005581281643650177,0.000628767369999616
+0.420488743117445,0.69,0.5,91.0,-0.00016664563761409858,0.00017536420885149365,-0.00031125361273436796,0.00035961307953965194
+0.420488743117445,0.75,0.5,90.0,-0.0001705952915724237,0.00017075306876618786,-0.0003260985410063516,0.0003436521597488523
+0.420488743117445,0.81,0.5,10.0,-0.0003877310836817143,0.0002829034191699664,-0.0012141788022607314,0.000352904446387595
+0.534211750010975,0.21,0.5,13.0,-0.002916485923058068,0.0026770360375788344,-0.0059748599926445455,0.005028777816297821
+0.534211750010975,0.27,0.5,22.0,-0.0023993771479273564,0.00203170768882598,-0.004954432197648841,0.003840245092740577
+0.534211750010975,0.33,0.5,33.0,-0.0017315612570448342,0.0015185801609968407,-0.0035246444410144614,0.0028890463936857916
+0.534211750010975,0.39,0.5,46.0,-0.0010606725677865904,0.0010803077422497807,-0.0020642223911372876,0.0021198921570105655
+0.534211750010975,0.45,0.5,41.0,-0.0010246606610200815,0.0009908380573501894,-0.0020856598528277634,0.001913758494930707
+0.534211750010975,0.51,0.5,49.0,-0.0006205169706534118,0.0006446526154012886,-0.0012073085129657931,0.0012991981582230515
+0.534211750010975,0.57,0.5,51.0,-0.0005488404935584684,0.0005906137763122229,-0.0010548039131561954,0.001174594829824721
+0.534211750010975,0.63,0.5,57.0,-0.00039316272057892575,0.00043262740634596945,-0.0007668212778236899,0.0008621891664220272
+0.534211750010975,0.69,0.5,89.0,-0.0002184589557901026,0.00023561219082958283,-0.00042478189956557584,0.0004732610063131865
+0.534211750010975,0.75,0.5,88.0,-0.00022236472000267848,0.00023527315919018678,-0.0004497671036278354,0.0004623967076274263
+0.534211750010975,0.81,0.5,10.0,-0.0005101766853280905,0.0003356433191620221,-0.0013097174561167786,0.00044275231682028895
+0.6786916380543087,0.21,0.5,13.0,-0.0036363639066434336,0.0029822124557245568,-0.007267320255279984,0.005751656776638269
+0.6786916380543087,0.27,0.5,23.0,-0.002868136919175861,0.002670195354861992,-0.005984110953400747,0.004996530225868662
+0.6786916380543087,0.33,0.5,33.0,-0.0023679207204174903,0.001927819356149444,-0.004637987448209531,0.003710399353589642
+0.6786916380543087,0.39,0.5,47.0,-0.00134681585639847,0.0013130245643083406,-0.0027333372633782356,0.002609149882698294
+0.6786916380543087,0.45,0.5,43.0,-0.0012987021603353501,0.0013089989642506169,-0.002602942276052125,0.0024404590897749837
+0.6786916380543087,0.51,0.5,46.0,-0.0009108664482165002,0.0008392404885210621,-0.001837198906575315,0.0016439062939239395
+0.6786916380543087,0.57,0.5,52.0,-0.0007189380185762048,0.000736709506855566,-0.0014114257162754704,0.0015206946591334533
+0.6786916380543087,0.63,0.5,57.0,-0.0005114065306413679,0.0005298904676029247,-0.0009774573355180436,0.0011086396415892535
+0.6786916380543087,0.69,0.5,88.0,-0.00030030155032602417,0.0003113266260026901,-0.0005677057065852856,0.0006331350428357647
+0.6786916380543087,0.75,0.5,86.0,-0.0003209443916744643,0.00032095631260820604,-0.0006525838285355016,0.0006191845514750729
+0.6786916380543087,0.81,0.5,11.0,-0.000939251907320971,0.0005178364956414,-0.001950836997267935,0.0009741345090676493
+0.8622467393414631,0.21,0.5,13.0,-0.003734624466756839,0.0033597281671411535,-0.0071902995033083705,0.006428322323810652
+0.8622467393414631,0.27,0.5,23.0,-0.003482980020922902,0.003066344810041164,-0.00695634801377641,0.0059633977817294135
+0.8622467393414631,0.33,0.5,36.0,-0.002665403040122164,0.002276290818003147,-0.005746114548673678,0.004254677145944546
+0.8622467393414631,0.39,0.5,46.0,-0.001671682529052229,0.0015221593720513506,-0.0032611888548132817,0.0029424993172877064
+0.8622467393414631,0.45,0.5,42.0,-0.0016541895624853312,0.0015734221839346328,-0.003231856014229699,0.0030755206709700963
+0.8622467393414631,0.51,0.5,46.0,-0.0011569503444192758,0.0010958677837353827,-0.0024585761204914676,0.0020531130266181336
+0.8622467393414631,0.57,0.5,53.0,-0.000906925089891388,0.0009644725264415441,-0.0018207731070856862,0.0018202774872616086
+0.8622467393414631,0.63,0.5,58.0,-0.000615953053272021,0.0006866229427200467,-0.0012637533658231617,0.001336848019639403
+0.8622467393414631,0.69,0.5,86.0,-0.00041899157966442574,0.000425348145027021,-0.0008481992257809135,0.0008570348437286322
+0.8622467393414631,0.75,0.5,85.0,-0.0004686523137738776,0.00046295629008719053,-0.0008863515210015795,0.0009089643115764243
+0.8622467393414631,0.81,0.5,11.0,-0.001380620616328528,0.000775837790160776,-0.002867346394456777,0.0014742271430893666
+1.0954451150103472,0.21,0.5,14.0,-0.0036783471371409243,0.003364257373159071,-0.007189927051716508,0.006525721832682112
+1.0954451150103472,0.27,0.5,24.0,-0.003398601731166396,0.003051839733306186,-0.00674022194009315,0.005932903156363215
+1.0954451150103472,0.33,0.5,36.0,-0.0030420832741442595,0.0025440959134703325,-0.00605926776739194,0.004932119058642846
+1.0954451150103472,0.39,0.5,47.0,-0.001877780360092129,0.001709071340014373,-0.003783777182340101,0.0034547963421155802
+1.0954451150103472,0.45,0.5,42.0,-0.00186460672596041,0.001977917463476568,-0.003945671759586198,0.003719481305099038
+1.0954451150103472,0.51,0.5,47.0,-0.0014675026703338295,0.0014117823174016105,-0.002959462203716347,0.0026891362925195966
+1.0954451150103472,0.57,0.5,56.0,-0.0010912504646924002,0.0010899449165242426,-0.0021644925844890883,0.002244298008950281
+1.0954451150103472,0.63,0.5,58.0,-0.0008604029833960955,0.0008574008479886874,-0.0016296007521118736,0.0016970635309640578
+1.0954451150103472,0.69,0.5,83.0,-0.00054920903455386,0.000625432770791085,-0.0011054081690212221,0.0011929793974061668
+1.0954451150103472,0.75,0.5,83.0,-0.0006661047913622569,0.0006606388006140943,-0.0012743142128749363,0.0012665714554565134
+1.0954451150103472,0.81,0.5,9.0,-0.0017334025227949705,0.001320833297222358,-0.00411566265224973,0.0025232609331779987
+1.391713004234159,0.21,0.5,13.0,-0.0033698748560850723,0.0034952033487097986,-0.006502529881211022,0.006673993016617625
+1.391713004234159,0.27,0.5,27.0,-0.002971842797146482,0.002722582140038135,-0.005732973302930387,0.005350182014578461
+1.391713004234159,0.33,0.5,33.0,-0.002965369656030248,0.0026659092505073347,-0.006173504797710425,0.004906260215646475
+1.391713004234159,0.39,0.5,51.0,-0.0018200795235505571,0.0016973652906516368,-0.0036337977436919403,0.0033140766225205056
+1.391713004234159,0.45,0.5,45.0,-0.0021283722955777323,0.0019544864635317317,-0.00422246560472042,0.0038676467894268683
+1.391713004234159,0.51,0.5,50.0,-0.0017991248886090137,0.0015890010662942843,-0.003662580753253015,0.0031550814991557776
+1.391713004234159,0.57,0.5,54.0,-0.0012366267676283754,0.0012025208322152146,-0.002368391907169734,0.002405792468050632
+1.391713004234159,0.63,0.5,56.0,-0.0009880869569258428,0.0009569982126138651,-0.0019083605801074757,0.0018907847025472074
+1.391713004234159,0.69,0.5,92.0,-0.0007253195734617157,0.0006939111135046455,-0.001406077485835505,0.0014069321422638368
+1.391713004234159,0.75,0.5,71.0,-0.0008710795866985355,0.0008292351091759385,-0.00171744131382644,0.0016446216063853466
+1.391713004234159,0.81,0.5,6.0,-0.00015209892337673483,0.00017409517126630117,-0.0003749796468255166,0.00039698705645626237
+1.7681078308849858,0.21,0.5,14.0,-0.0030048176861491873,0.0031034968168193477,-0.005914813550845552,0.005762872122565723
+1.7681078308849858,0.27,0.5,32.0,-0.0029427406980165175,0.0025949235868870458,-0.005794631087317944,0.00525013753981949
+1.7681078308849858,0.33,0.5,34.0,-0.0022953620635008764,0.002369291563435302,-0.0044967493993599535,0.004524590058523953
+1.7681078308849858,0.39,0.5,53.0,-0.0018572917165704896,0.0016856817151675988,-0.0036186469202908384,0.0033681266314716865
+1.7681078308849858,0.45,0.5,51.0,-0.0020509555751343036,0.0018845433625795875,-0.004132094595344406,0.0037968033119854276
+1.7681078308849858,0.51,0.5,49.0,-0.0017676698983243725,0.0016129024301858555,-0.0034777756120045293,0.003023307448424721
+1.7681078308849858,0.57,0.5,51.0,-0.0015254980497710312,0.001485438594775114,-0.0030587382876296368,0.0028234889076227654
+1.7681078308849858,0.63,0.5,60.0,-0.0009294639281146025,0.0009742676647529223,-0.001838612067821218,0.0018671101330660022
+1.7681078308849858,0.69,0.5,101.0,-0.0007702485214657045,0.0007552137737377276,-0.0015164247959691113,0.0015328439522218
+1.7681078308849858,0.75,0.5,49.0,-0.0012027889186755703,0.0010833068087470299,-0.0024667019206261924,0.0020785892117345267
+2.2463002732069293,0.21,0.5,15.0,-0.003551758233224311,0.00330827033551763,-0.006880060446751559,0.006384560492944749
+2.2463002732069293,0.27,0.5,34.0,-0.002413338453235885,0.002359366990184548,-0.004892978794890064,0.004746462316043185
+2.2463002732069293,0.33,0.5,38.0,-0.00205314896299799,0.0020489454237541493,-0.004052479683222713,0.003953208326238531
+2.2463002732069293,0.39,0.5,49.0,-0.0022095214799961915,0.002151100045197068,-0.004315654740874292,0.004222283690502381
+2.2463002732069293,0.45,0.5,56.0,-0.0017923814114834075,0.0018089494272520185,-0.003606934588035148,0.003362257824573414
+2.2463002732069293,0.51,0.5,51.0,-0.002127568456494537,0.0019698885297037383,-0.004450346713070935,0.0036473227934794416
+2.2463002732069293,0.57,0.5,48.0,-0.0017211381372830238,0.0017004628840137962,-0.0036272445268787615,0.0030865305556439537
+2.2463002732069293,0.63,0.5,67.0,-0.0010583053393894686,0.0009376110108166037,-0.0020622766505269128,0.001863218429486916
+2.2463002732069293,0.69,0.5,100.0,-0.0009132285314978304,0.0008934887506850118,-0.0017494303900023231,0.001771841469735514
+2.2463002732069293,0.75,0.5,36.0,-0.0014489047726835454,0.0012131167912297785,-0.0029080019148220136,0.002274795116575197
+2.853821938497884,0.21,0.5,17.0,-0.0029139803268383316,0.0027849096231677343,-0.005678642923602732,0.005626122741617419
+2.853821938497884,0.27,0.5,34.0,-0.0022669090120196623,0.0021752427788872975,-0.004387190586664019,0.004286020588784302
+2.853821938497884,0.33,0.5,46.0,-0.001751819969380436,0.0018328983943958971,-0.0034396430035106354,0.003551348004107762
+2.853821938497884,0.39,0.5,50.0,-0.0021897601453964902,0.0021077828364107214,-0.004364422233777666,0.004094880490283786
+2.853821938497884,0.45,0.5,54.0,-0.0020003104866410425,0.0017452423708697058,-0.0038840870194610097,0.003341282362726006
+2.853821938497884,0.51,0.5,53.0,-0.001978554084136321,0.0017414931912755147,-0.003966559394661802,0.003435815776940722
+2.853821938497884,0.57,0.5,45.0,-0.0017903449719321313,0.0015358509907545887,-0.0034429838600979323,0.0030872931085461903
+2.853821938497884,0.63,0.5,68.0,-0.0011313231539702916,0.0011393448582226462,-0.00236499986388756,0.002150227908604761
+2.853821938497884,0.69,0.5,98.0,-0.0011026478277482118,0.0010335506576895032,-0.0022210276329604657,0.0020096431164819215
+2.853821938497884,0.75,0.5,30.0,-0.0018310568102289748,0.001575699467069024,-0.003834008826893295,0.002945732404681843
+3.625650476828123,0.15,0.5,9.0,-0.001870962034876359,0.0018667760258650715,-0.0035300245835492294,0.0036131940907462973
+3.625650476828123,0.21,0.5,17.0,-0.002122238158250323,0.002149547203406812,-0.003953470209131434,0.004223956571403396
+3.625650476828123,0.27,0.5,36.0,-0.0020361368467661555,0.0017412155003332086,-0.004192586565441976,0.003361558733991561
+3.625650476828123,0.33,0.5,58.0,-0.0013807844912928516,0.0013307963072129987,-0.0028001649341155735,0.002587532564165583
+3.625650476828123,0.39,0.5,49.0,-0.0019393148838704355,0.0018118046393262525,-0.0038860403410479697,0.0035698084732656353
+3.625650476828123,0.45,0.5,51.0,-0.0013796022356330775,0.0013218020224782042,-0.0027715762879580936,0.0025467101071574866
+3.625650476828123,0.51,0.5,47.0,-0.0013416912168944205,0.0013237348758077905,-0.0026667297027306606,0.0025921607978518385
+3.625650476828123,0.57,0.5,45.0,-0.0017413550964999833,0.001789463016931289,-0.003433802132231108,0.003514526842449405
+3.625650476828123,0.63,0.5,67.0,-0.0013754700930605727,0.0013354728097109512,-0.0027677478122524954,0.0025804317614262955
+3.625650476828123,0.69,0.5,95.0,-0.001177885848949016,0.0011298837771364792,-0.0023984810286472005,0.0021884551485762548
+3.625650476828123,0.75,0.5,26.0,-0.0031140555440440044,0.0027140006290446578,-0.00619886612005896,0.005012744596470631
+4.606223395648525,0.15,0.5,9.0,-0.00213407847867903,0.00217202644506905,-0.004007727470685757,0.004203607985896193
+4.606223395648525,0.21,0.5,22.0,-0.001551212946304252,0.0018098151113754163,-0.0030411663813862634,0.00358859162154308
+4.606223395648525,0.27,0.5,41.0,-0.0019878070074636164,0.0018102514348666216,-0.003951756610085492,0.0033748032684783194
+4.606223395648525,0.33,0.5,53.0,-0.0014379442403381563,0.001452316793320157,-0.002959236331211844,0.0029182512339700887
+4.606223395648525,0.39,0.5,54.0,-0.0016590327681175957,0.0013885839660638705,-0.0032264713733278416,0.0028372420724612694
+4.606223395648525,0.45,0.5,54.0,-0.0012361246562966,0.0011821470811921976,-0.002457473355785646,0.002377155858178266
+4.606223395648525,0.51,0.5,42.0,-0.0017191152974805732,0.0014793684786840755,-0.0034446402784582206,0.002886582345160743
+4.606223395648525,0.57,0.5,42.0,-0.0018370856804507776,0.00198956645510079,-0.003357082073613866,0.004009689911216863
+4.606223395648525,0.63,0.5,78.0,-0.0014036086108003803,0.0012649221717034049,-0.002611443025357724,0.0025835553005561958
+4.606223395648525,0.69,0.5,80.0,-0.001368257519848771,0.0013448852894266349,-0.002739863326398594,0.0025024748026608494
+4.606223395648525,0.75,0.5,23.0,-0.0033645521495273252,0.0033890458873797984,-0.006585507949012495,0.006494486905909346
+5.85199651930643,0.15,0.5,11.0,-0.002568168855375556,0.0025424532878839854,-0.00521159776195888,0.004688761903537786
+5.85199651930643,0.21,0.5,24.0,-0.0024203061069344306,0.0024984361561779743,-0.004871343658052136,0.004834434618436434
+5.85199651930643,0.27,0.5,42.0,-0.0018351960243089603,0.001966991176339487,-0.003550562584107309,0.003938850726327077
+5.85199651930643,0.33,0.5,52.0,-0.0013825265699841983,0.001501315853432353,-0.002878058743422798,0.002972080670573622
+5.85199651930643,0.39,0.5,56.0,-0.0016490875294503373,0.001518836583590845,-0.0033849458567029094,0.0028521417983976413
+5.85199651930643,0.45,0.5,62.0,-0.0018039828030795046,0.001705240312783338,-0.003531930681695563,0.0034309659401621758
+5.85199651930643,0.51,0.5,48.0,-0.0017611006033400737,0.001844671598438632,-0.0036234332425141235,0.0034577931726043902
+5.85199651930643,0.57,0.5,50.0,-0.001962356729866996,0.0018251728213337882,-0.0037676565660721725,0.0037471832741934976
+5.85199651930643,0.63,0.5,65.0,-0.0018203982551820805,0.0016935723253246034,-0.0036655432153363077,0.0032618891848857803
+5.85199651930643,0.69,0.5,70.0,-0.0016178720142823576,0.0016343002646696384,-0.0032488373063732025,0.0031338311056391213
+5.85199651930643,0.75,0.5,17.0,-0.0029949538755950677,0.003455084453193372,-0.006065084615647303,0.006658415213178723
+7.434694395049619,0.15,0.5,12.0,-0.0017291752792880657,0.0025031149992689986,-0.0032172059115459727,0.0052158449199299
+7.434694395049619,0.21,0.5,29.0,-0.0018969941738325668,0.002246928226294584,-0.0035785789341532754,0.004330252838172466
+7.434694395049619,0.27,0.5,58.0,-0.0015328197460049303,0.0014532796523718326,-0.00294516536966658,0.002969832244400047
+7.434694395049619,0.33,0.5,60.0,-0.0015948464412691241,0.001606706513376739,-0.0032900515297670115,0.0030344214739774647
+7.434694395049619,0.39,0.5,52.0,-0.0018041721804816183,0.0017657498512890556,-0.003481952613124358,0.00352566423417895
+7.434694395049619,0.45,0.5,55.0,-0.002022619838695802,0.0019444459497014069,-0.003962048429960672,0.00376666857689726
+7.434694395049619,0.51,0.5,51.0,-0.0022103080545111888,0.002115615800648187,-0.00437018604332527,0.004199842016962025
+7.434694395049619,0.57,0.5,61.0,-0.0024035000068523,0.0023031881392631395,-0.004669011670420161,0.004562216879579845
+7.434694395049619,0.63,0.5,65.0,-0.0022110318935754953,0.002091789581668007,-0.00444909360024201,0.0041349207012691186
+7.434694395049619,0.69,0.5,46.0,-0.0033635574201190967,0.0028561090492171715,-0.006315899723244817,0.005925443729299359
+7.434694395049619,0.75,0.5,7.0,-0.006815880308679281,0.005346113144263046,-0.013697211103365496,0.009978842608218954
+9.44543978545178,0.15,0.5,13.0,-0.002408009933915766,0.00274271582556013,-0.004705202282924212,0.0052712062522867874
+9.44543978545178,0.21,0.5,36.0,-0.0022977429120207304,0.0021136558956367235,-0.004561454841562762,0.004157513456563003
+9.44543978545178,0.27,0.5,52.0,-0.001809064679657837,0.0016258903992006554,-0.0036060822664138155,0.0032582708262085523
+9.44543978545178,0.33,0.5,69.0,-0.0019083508292321544,0.001836709767211145,-0.0036422680965225236,0.0036289453104446654
+9.44543978545178,0.39,0.5,70.0,-0.0020459122530994385,0.001992065442843721,-0.004031622778612427,0.003870813004126251
+9.44543978545178,0.45,0.5,55.0,-0.0024890698494763643,0.0021074619699311217,-0.00472100272658335,0.004333720234957476
+9.44543978545178,0.51,0.5,55.0,-0.002616950213729354,0.0025679394777637183,-0.005199795310685964,0.005001544413641422
+9.44543978545178,0.57,0.5,49.0,-0.0034924055164432615,0.0031808151454395827,-0.006937465427275243,0.006227823606700601
+9.44543978545178,0.63,0.5,56.0,-0.003597602253635147,0.0033108470563384855,-0.007137064915220214,0.006504846334814207
+9.44543978545178,0.69,0.5,34.0,-0.004550372816795669,0.004419990926005116,-0.00852966884636828,0.008585474820677823
+9.44543978545178,0.75,0.5,7.0,-0.011149376196850858,0.010033624291347817,-0.020998763897258976,0.019604622526969102
+12.000000000000004,0.15,0.5,14.0,-0.0027258542848209747,0.0031137912931876,-0.004989559709487944,0.006115373666664247
+12.000000000000004,0.21,0.5,38.0,-0.0017604332838869897,0.0016964013214811752,-0.003471060797346072,0.003323362673904191
+12.000000000000004,0.27,0.5,55.0,-0.00216586673081793,0.002104498736351069,-0.004525563420813549,0.003973096654193856
+12.000000000000004,0.33,0.5,69.0,-0.0019342957813413741,0.0017883786446623617,-0.003845824945010516,0.0034122409970355457
+12.000000000000004,0.39,0.5,80.0,-0.002056626673205368,0.0020736251800277084,-0.004197830332801134,0.003977304194115365
+12.000000000000004,0.45,0.5,56.0,-0.0022526022213359364,0.002283922059326829,-0.004362578157788527,0.004343503646784428
+12.000000000000004,0.51,0.5,48.0,-0.003858181132400322,0.0033869239166510463,-0.00761237077501284,0.006535043051495436
+12.000000000000004,0.57,0.5,47.0,-0.004733981426136582,0.003969725222908433,-0.009166836419887628,0.008098474810948712
+12.000000000000004,0.63,0.5,44.0,-0.005226047573556978,0.004597975750924846,-0.010118808426693838,0.009167703577117771
+12.000000000000004,0.69,0.5,27.0,-0.006389955062104781,0.005800523713446416,-0.012402700932955703,0.011744460412327655
+12.000000000000004,0.75,0.5,13.0,-0.010148359935548886,0.008685063147566022,-0.020248856837627886,0.016152532258748995
+0.1000000000000051,0.21,1.0,12.0,-8.981800804662394e-05,0.00010828731663162501,-0.00017391335595408073,0.0002123798709823636
+0.1000000000000051,0.27,1.0,28.0,-6.572975141133476e-05,6.599759401963608e-05,-0.0001331979995488841,0.0001287758402777232
+0.1000000000000051,0.33,1.0,35.0,-8.049508380363746e-05,6.57423867272947e-05,-0.00017453209956291342,0.0001224765797433133
+0.1000000000000051,0.39,1.0,51.0,-5.8600409468941983e-05,7.041536880749508e-05,-0.0001089797704785188,0.00014759771636082547
+0.1000000000000051,0.45,1.0,51.0,-6.400755906618381e-05,7.801594007036556e-05,-0.00012308590065977573,0.0001638058689515976
+0.1000000000000051,0.51,1.0,49.0,-7.418178983809971e-05,8.368877938274378e-05,-0.0001312744515705406,0.00017966555322063507
+0.1000000000000051,0.57,1.0,61.0,-6.247050693672102e-05,7.183730144583945e-05,-0.00011862582653128915,0.00014482841821019968
+0.1000000000000051,0.63,1.0,57.0,-5.4599472866910664e-05,6.609507136517092e-05,-9.834302602249346e-05,0.00014071587589844063
+0.1000000000000051,0.69,1.0,91.0,-4.44751551891699e-05,5.121851515337165e-05,-8.523169498118545e-05,0.00010722467887333296
+0.1000000000000051,0.75,1.0,51.0,-8.131783339427816e-05,8.712176698803112e-05,-0.00017209531557954645,0.00016741074118309764
+0.1000000000000051,0.81,1.0,11.0,-2.7856229962833847e-06,2.9147312166989665e-06,-5.535858715828931e-06,5.5959265965038546e-06
+0.1270454343320773,0.21,1.0,12.0,-0.00011925451258258278,0.00013667560692871725,-0.0002235627621989307,0.000282250972400914
+0.1270454343320773,0.27,1.0,28.0,-0.00010347473507083254,9.397327149376989e-05,-0.000203032081608538,0.00018443015324141014
+0.1270454343320773,0.33,1.0,35.0,-0.00011978198801173887,9.186788367491428e-05,-0.00023983716072103152,0.00017760949971449758
+0.1270454343320773,0.39,1.0,51.0,-7.509325170934057e-05,8.488486649590101e-05,-0.00014434181649718392,0.0001661879230696129
+0.1270454343320773,0.45,1.0,51.0,-7.802398888845351e-05,8.964834788500774e-05,-0.00014964815383203072,0.0001878688164312219
+0.1270454343320773,0.51,1.0,52.0,-7.931528454482566e-05,9.588611316231842e-05,-0.00014957604346034107,0.00020471897421972516
+0.1270454343320773,0.57,1.0,58.0,-6.816580987644215e-05,7.692974071720871e-05,-0.00013119864631990302,0.00015978101729742123
+0.1270454343320773,0.63,1.0,58.0,-5.660047555813941e-05,6.667063583491812e-05,-0.00010740107697165595,0.00013980152896763431
+0.1270454343320773,0.69,1.0,90.0,-4.6488468080663706e-05,5.3007731655267536e-05,-9.001357976491348e-05,0.00010699950759423925
+0.1270454343320773,0.75,1.0,52.0,-8.687055298445975e-05,8.141141646918013e-05,-0.0001646786812222045,0.0001593791874877388
+0.1270454343320773,0.81,1.0,10.0,-3.508541145356606e-06,3.116579949113961e-06,-6.664419579304332e-06,6.195220305054949e-06
+0.1614054238461892,0.21,1.0,12.0,-0.00017856720906143632,0.0001978855378957053,-0.0003201844764897874,0.00042136501843360614
+0.1614054238461892,0.27,1.0,28.0,-0.0001574474227387835,0.00016575764604671078,-0.00032947603258194467,0.00031768043090398793
+0.1614054238461892,0.33,1.0,35.0,-0.000180377409145631,0.0001465242069720509,-0.00038599368852897494,0.00026879692381450414
+0.1614054238461892,0.39,1.0,51.0,-0.00011135560660987238,0.00011002916208773523,-0.00021861767680042484,0.00021858183747928725
+0.1614054238461892,0.45,1.0,51.0,-0.00010824638728157745,0.0001178781347722602,-0.00020353059792387282,0.00023726910696950887
+0.1614054238461892,0.51,1.0,54.0,-9.882519763792153e-05,0.00011544922587817531,-0.00019260490619590792,0.00022914517346072695
+0.1614054238461892,0.57,1.0,56.0,-8.284958996726069e-05,9.709648108532675e-05,-0.00015972699558694257,0.0001985021932517295
+0.1614054238461892,0.63,1.0,58.0,-6.399733454519141e-05,7.696419847159642e-05,-0.00011742647092396849,0.0001609290501879093
+0.1614054238461892,0.69,1.0,90.0,-5.10597173216538e-05,5.665656456164655e-05,-9.232866808360568e-05,0.00011996865459450451
+0.1614054238461892,0.75,1.0,52.0,-9.202323582652096e-05,8.397431602992125e-05,-0.00017781049121938996,0.0001688547566809357
+0.1614054238461892,0.81,1.0,10.0,-4.348784203306676e-06,3.528719249090706e-06,-8.633860777487783e-06,6.526661229964468e-06
+0.2050582217608948,0.21,1.0,12.0,-0.0003029495078270915,0.0003332769145060203,-0.0005588710074567773,0.0007014183189471327
+0.2050582217608948,0.27,1.0,28.0,-0.00029219463926815123,0.0002698459104236296,-0.000574204089561727,0.0005448643467889439
+0.2050582217608948,0.33,1.0,36.0,-0.00029973441491753486,0.0002451415797281208,-0.0006219144174760823,0.0004565953480111721
+0.2050582217608948,0.39,1.0,51.0,-0.00019007976458086822,0.00017173939871628402,-0.00035373418966627316,0.0003510460450799803
+0.2050582217608948,0.45,1.0,52.0,-0.00016415356933323117,0.00016471106662050144,-0.00032438211600033457,0.00033879825198262196
+0.2050582217608948,0.51,1.0,52.0,-0.00014780017191122954,0.00016492418018978738,-0.0002742922739160424,0.00032193917956503155
+0.2050582217608948,0.57,1.0,56.0,-0.00011328676640951879,0.00012855391347515153,-0.00021595160930404361,0.0002685813373738302
+0.2050582217608948,0.63,1.0,58.0,-8.160413698394131e-05,9.97454972572196e-05,-0.00015028257235582133,0.00020251382732060902
+0.2050582217608948,0.69,1.0,90.0,-6.0485401373979105e-05,7.003834699725463e-05,-0.00011421116556335438,0.0001392836697360542
+0.2050582217608948,0.75,1.0,52.0,-0.00010348223107482419,9.79325002188757e-05,-0.00019607714811367414,0.00019559250877428588
+0.2050582217608948,0.81,1.0,10.0,-1.0015599765830797e-05,7.650358473165775e-06,-2.0235097476661835e-05,1.3700072480516829e-05
+0.2605171084697166,0.21,1.0,12.0,-0.0004898151279176122,0.0005663797215278053,-0.000970223969235475,0.0010821881693934715
+0.2605171084697166,0.27,1.0,28.0,-0.0004988861750466264,0.000463433781455484,-0.001018169627189372,0.0008864896866640474
+0.2605171084697166,0.33,1.0,37.0,-0.0004924866278021822,0.0003833863718500108,-0.000991595901137859,0.000717217821207667
+0.2605171084697166,0.39,1.0,50.0,-0.0002917064892448641,0.00027249742298316316,-0.0005838369684998405,0.0005171639558125296
+0.2605171084697166,0.45,1.0,52.0,-0.00025446901215136304,0.00023791529482339365,-0.00048165101241912745,0.00048763907400480635
+0.2605171084697166,0.51,1.0,54.0,-0.00019843946523137983,0.00022885862681156204,-0.0003985613849450534,0.00044483869980572327
+0.2605171084697166,0.57,1.0,55.0,-0.0001600814247636166,0.00017014324758529738,-0.00029695495015642955,0.00034850126859339316
+0.2605171084697166,0.63,1.0,57.0,-0.00010355880243180485,0.00013449616320191236,-0.0002018945222819357,0.0002597914495309339
+0.2605171084697166,0.69,1.0,91.0,-7.55059741381338e-05,8.739354746902772e-05,-0.00014789295993276059,0.00017651771641109508
+0.2605171084697166,0.75,1.0,51.0,-0.0001300170583083465,0.00011926383498665972,-0.0002518784279237022,0.0002324610339944769
+0.2605171084697166,0.81,1.0,10.0,-1.558559760356466e-05,1.0879330673836148e-05,-3.251125745888372e-05,1.9902427628253602e-05
+0.3309750919646659,0.21,1.0,12.0,-0.0008616743271188065,0.0008805180718652612,-0.001629708418422763,0.0017486943255844841
+0.3309750919646659,0.27,1.0,29.0,-0.0009351237642220879,0.0007840527811021821,-0.0019095890602856308,0.0015388536993235372
+0.3309750919646659,0.33,1.0,36.0,-0.0007152248492381158,0.000554456293649131,-0.001450409912028956,0.00108330393832548
+0.3309750919646659,0.39,1.0,51.0,-0.00045360851275599184,0.0004174493429478182,-0.0009209731718406825,0.000791631027138214
+0.3309750919646659,0.45,1.0,51.0,-0.000388563376938702,0.00037898585167270906,-0.0007556922518898059,0.0007426925359073305
+0.3309750919646659,0.51,1.0,54.0,-0.00029243196395079707,0.0003123974115778045,-0.0005743905647402116,0.0006276183607800766
+0.3309750919646659,0.57,1.0,58.0,-0.00020962043135197694,0.00023206448599246275,-0.00041362142815537517,0.00045557372772887604
+0.3309750919646659,0.63,1.0,55.0,-0.00012744477748855525,0.0001711904470858174,-0.00025133756093753565,0.0003354438929231392
+0.3309750919646659,0.69,1.0,90.0,-9.527179146233411e-05,0.00010371789665519487,-0.0001808666344486871,0.00021392137268674935
+0.3309750919646659,0.75,1.0,51.0,-0.0001527539953624492,0.00013124618975204997,-0.0002876307706170413,0.0002711567451620178
+0.3309750919646659,0.81,1.0,10.0,-2.3818754097060774e-05,2.051743715942726e-05,-4.855094662128912e-05,3.759832932052416e-05
+0.4204887431174512,0.21,1.0,13.0,-0.001259925909672052,0.0013894948542713444,-0.0023924876167094257,0.00263383502708431
+0.4204887431174512,0.27,1.0,29.0,-0.0013531129901382618,0.001289037909706345,-0.0029124882492640447,0.0023432508883958762
+0.4204887431174512,0.33,1.0,35.0,-0.00114008161924429,0.0008625201550548686,-0.0022888194719876387,0.001661936954814998
+0.4204887431174512,0.39,1.0,52.0,-0.0006940860750947986,0.0006089399644193536,-0.0014022752143868142,0.0011747546653694744
+0.4204887431174512,0.45,1.0,53.0,-0.0005489658491499013,0.0005364669173419563,-0.0011373019638681444,0.0010206849406504091
+0.4204887431174512,0.51,1.0,53.0,-0.00045851039455254984,0.00046346773535243846,-0.0009174964290208481,0.0009443692294082585
+0.4204887431174512,0.57,1.0,57.0,-0.00029133611904412607,0.00029778706731504534,-0.0005539429039301607,0.0006321004735247885
+0.4204887431174512,0.63,1.0,57.0,-0.00017015517930964034,0.0002025204561234622,-0.0003271820020943712,0.00041875564060600074
+0.4204887431174512,0.69,1.0,88.0,-0.000122581644016862,0.00013688468062309173,-0.00024247649110212727,0.00027222840279835333
+0.4204887431174512,0.75,1.0,50.0,-0.00017053568863653726,0.0001617617227640018,-0.0003205507397762648,0.0003262791043199001
+0.4204887431174512,0.81,1.0,10.0,-4.4449514860189795e-05,3.996338283563936e-05,-8.97241618210701e-05,7.429831077128035e-05
+0.534211750010956,0.21,1.0,13.0,-0.00198094123440909,0.002007636078536401,-0.0038525267138686836,0.004015229525904618
+0.534211750010956,0.27,1.0,30.0,-0.001955014920256275,0.001788099703351316,-0.004197318979304969,0.0032111487450703206
+0.534211750010956,0.33,1.0,35.0,-0.0015342456469924662,0.0013583463688737589,-0.003299049770884159,0.0025177055622660365
+0.534211750010956,0.39,1.0,52.0,-0.000990496189600039,0.0008901031209920656,-0.0019937145541164465,0.0017283946925559929
+0.534211750010956,0.45,1.0,52.0,-0.0008616447971995048,0.0007634250323203513,-0.0016653944388589173,0.0014981083571904252
+0.534211750010956,0.51,1.0,54.0,-0.0006809701999924191,0.0006679700438902982,-0.0013023250135815055,0.0013336794393900746
+0.534211750010956,0.57,1.0,57.0,-0.0004162717316340118,0.0004392796535995453,-0.0007772722032914171,0.0008818010512436711
+0.534211750010956,0.63,1.0,60.0,-0.00024877417996121466,0.0002708433287137004,-0.00044568463863167164,0.0005621851308350494
+0.534211750010956,0.69,1.0,85.0,-0.00016671579582384194,0.00017684372471624612,-0.00033344893152479976,0.00034769180013871637
+0.534211750010956,0.75,1.0,49.0,-0.00020879331142069113,0.0002119567648267669,-0.0004188218246010598,0.0004000793604715514
+0.534211750010956,0.81,1.0,10.0,-8.961503894663943e-05,8.082627816715503e-05,-0.00018138428304011314,0.00015042917219333838
+0.6786916380542969,0.21,1.0,14.0,-0.002803637988312798,0.0028595778376100294,-0.005544289919248514,0.0055572371306858385
+0.6786916380542969,0.27,1.0,29.0,-0.0026017018419168918,0.002322218949302564,-0.005324329271876218,0.00437007810294163
+0.6786916380542969,0.33,1.0,36.0,-0.0023142927425653884,0.0017420525287963025,-0.004553166802885131,0.0034965390654711106
+0.6786916380542969,0.39,1.0,52.0,-0.001333641983843818,0.0012297046187465896,-0.0026944738781859994,0.002254130378611207
+0.6786916380542969,0.45,1.0,54.0,-0.001132058243763309,0.0010315164275137608,-0.0022758580119684358,0.0020284755518075554
+0.6786916380542969,0.51,1.0,54.0,-0.0009206488281855123,0.0008919955144489764,-0.001757966247920847,0.0017116624733975227
+0.6786916380542969,0.57,1.0,57.0,-0.0005717487863582299,0.000611015970319599,-0.0011036500296524832,0.0012170349994926244
+0.6786916380542969,0.63,1.0,57.0,-0.00029408789144624186,0.00033839398205625596,-0.0005712745898935967,0.000678513697844616
+0.6786916380542969,0.69,1.0,86.0,-0.00022053441897770823,0.00022357382688280222,-0.0004351826231547909,0.0004351137021696224
+0.6786916380542969,0.75,1.0,50.0,-0.0002487680636699821,0.00023399663924785028,-0.00047939261147678244,0.0004581629618528596
+0.6786916380542969,0.81,1.0,8.0,-0.0001662959006541176,0.0001627416546716165,-0.000319996643592127,0.00031575769634285285
+0.8622467393414539,0.21,1.0,15.0,-0.0038232917631787584,0.00366461110480297,-0.00739663734954125,0.007248317389007747
+0.8622467393414539,0.27,1.0,28.0,-0.0033330035170424715,0.0026942757783328885,-0.006816215888298102,0.005158083750737444
+0.8622467393414539,0.33,1.0,41.0,-0.0026355645730401973,0.0021414535237384204,-0.0053389589062391545,0.004127902512129049
+0.8622467393414539,0.39,1.0,52.0,-0.0016900137439331683,0.0016122369162207262,-0.0036120121251620213,0.0029339562826243832
+0.8622467393414539,0.45,1.0,52.0,-0.0015065984333524575,0.0014629514790295672,-0.0031599367055214433,0.0027568639137248506
+0.8622467393414539,0.51,1.0,55.0,-0.0012860830400390304,0.0011835337150727255,-0.002483242518541558,0.0022874784507430405
+0.8622467393414539,0.57,1.0,53.0,-0.0007443858884711018,0.0007654550997357236,-0.0014777879545899977,0.0015744435043521525
+0.8622467393414539,0.63,1.0,60.0,-0.000377025994548298,0.0004125051809209225,-0.0007423169257984567,0.0008150479758821957
+0.8622467393414539,0.69,1.0,86.0,-0.00028845541470185306,0.00029388727877469793,-0.0005830632434834417,0.0005714041238548249
+0.8622467393414539,0.75,1.0,47.0,-0.0003170652632738863,0.0002967065750933188,-0.0006222750591045508,0.0005751003622517988
+0.8622467393414539,0.81,1.0,8.0,-0.0002554370907092061,0.0002656321458266858,-0.0005125404115148602,0.0004878555099748494
+1.095445115010339,0.21,1.0,15.0,-0.00393736418107412,0.004606397228983365,-0.008160271834618376,0.008458159353237474
+1.095445115010339,0.27,1.0,29.0,-0.0037768005595458,0.0033009713146281757,-0.008076225493577,0.00612335002173377
+1.095445115010339,0.33,1.0,44.0,-0.0026536740147591353,0.0023297652712243777,-0.005552663437183514,0.004500042838902408
+1.095445115010339,0.39,1.0,51.0,-0.00226496061359153,0.0020837148318930093,-0.004845309486445686,0.003952924422119971
+1.095445115010339,0.45,1.0,52.0,-0.001985128554886096,0.001726398483146008,-0.0038339591526274437,0.0033119013491024196
+1.095445115010339,0.51,1.0,54.0,-0.001701652427799334,0.001692490241971985,-0.003498528065816099,0.003336344202984436
+1.095445115010339,0.57,1.0,54.0,-0.000959255451266736,0.0010080499068153112,-0.0018672807259580055,0.0020229712162597915
+1.095445115010339,0.63,1.0,61.0,-0.0005765785823718196,0.0005780937786715852,-0.0010451732441007497,0.0011622492789701148
+1.095445115010339,0.69,1.0,81.0,-0.0004119586406285921,0.0004027275743804307,-0.0008348060423923069,0.0007854435723891691
+1.095445115010339,0.75,1.0,47.0,-0.0004456920732999463,0.00042603130404428145,-0.0008961643522685154,0.0008268028619523922
+1.095445115010339,0.81,1.0,8.0,-0.00038198790112899117,0.000375004533879994,-0.0007422461001972331,0.0007275756905984754
+1.3917130042341683,0.15,1.0,5.0,-0.0064589305065142506,0.006060091598823969,-0.013750365788424456,0.011702570266561206
+1.3917130042341683,0.21,1.0,14.0,-0.0037419923034763213,0.004431038048408865,-0.007357258421144567,0.008449084871921699
+1.3917130042341683,0.27,1.0,30.0,-0.003501105241244222,0.003106405051917243,-0.0073517758362143144,0.005763184368696835
+1.3917130042341683,0.33,1.0,49.0,-0.002880493229816016,0.00242329447422375,-0.0055951295376762125,0.0048299971345038715
+1.3917130042341683,0.39,1.0,48.0,-0.0025556660241222466,0.0024405573426701244,-0.005211985866355685,0.004691296348775968
+1.3917130042341683,0.45,1.0,55.0,-0.002395011637863527,0.0021691545033030385,-0.0048531412380834115,0.004239697555490724
+1.3917130042341683,0.51,1.0,53.0,-0.0022717159468495784,0.0021792158655669046,-0.004515814995539571,0.004197211365167237
+1.3917130042341683,0.57,1.0,52.0,-0.0013040759337882464,0.0014393687069607416,-0.0026409558707374907,0.0027869468278466235
+1.3917130042341683,0.63,1.0,59.0,-0.0008549438286234354,0.0008705476640289378,-0.0016342407468309826,0.0017237042351869165
+1.3917130042341683,0.69,1.0,82.0,-0.0005860540438880922,0.0006124861866969518,-0.0012077901670566032,0.0011868903136646126
+1.3917130042341683,0.75,1.0,45.0,-0.000701181898714247,0.0006354514202446743,-0.0014329287360639914,0.0011861158857878467
+1.3917130042341683,0.81,1.0,8.0,-0.0005059199845315952,0.000507319037447676,-0.0009847880993988174,0.0009668979602883709
+1.768107830884997,0.15,1.0,5.0,-0.006005651633028619,0.006005651633028619,-0.011910403646333357,0.010846690730674657
+1.768107830884997,0.21,1.0,14.0,-0.003351613872980473,0.003683701924572251,-0.00651113843548951,0.007437677079829196
+1.768107830884997,0.27,1.0,34.0,-0.002969005529390139,0.002522002285859518,-0.006219471168534371,0.004704311897464221
+1.768107830884997,0.33,1.0,51.0,-0.0026082454299116934,0.002457198690997943,-0.0052312258058039044,0.00466756218136683
+1.768107830884997,0.39,1.0,43.0,-0.0026598819576218523,0.002496268710615408,-0.0052266959986575,0.0048702537689933115
+1.768107830884997,0.45,1.0,56.0,-0.002403890223292667,0.0023614597756475646,-0.004941702158895104,0.004468369240310798
+1.768107830884997,0.51,1.0,53.0,-0.0025928803948260895,0.0025381260110844584,-0.005233729441459026,0.004915511867058335
+1.768107830884997,0.57,1.0,53.0,-0.0016746708625205082,0.0017272432754521648,-0.0033022919846819984,0.0035238855146012653
+1.768107830884997,0.63,1.0,58.0,-0.0010932709483159966,0.001047107397933116,-0.0020808421112136805,0.0021865049748057562
+1.768107830884997,0.69,1.0,83.0,-0.0008143698874344555,0.0007675986837708305,-0.0016006651756933408,0.0014963493099226222
+1.768107830884997,0.75,1.0,42.0,-0.0009814897216909682,0.0009010487133734856,-0.0019830470042565603,0.0016846188535647362
+1.768107830884997,0.81,1.0,8.0,-0.0005782265749029725,0.0006063085527059642,-0.0011384037994586072,0.0011334766019924574
+2.246300273206941,0.15,1.0,6.0,-0.004661333572824872,0.006024421926580517,-0.008573102186716938,0.011880038727559696
+2.246300273206941,0.21,1.0,14.0,-0.0028046577530557106,0.003119963261189137,-0.005313302618372182,0.006231046405994895
+2.246300273206941,0.27,1.0,36.0,-0.0025659784490052375,0.0022449176062658382,-0.005450820294736863,0.00424062144547918
+2.246300273206941,0.33,1.0,51.0,-0.002235233748869493,0.002130659804769898,-0.004606509117999363,0.0042102798768783
+2.246300273206941,0.39,1.0,49.0,-0.0020954147675049492,0.001957115456385643,-0.0042891738349639195,0.003701078230948151
+2.246300273206941,0.45,1.0,58.0,-0.0023568243769875883,0.0022206160476152233,-0.0045609016901721755,0.004307985097597185
+2.246300273206941,0.51,1.0,44.0,-0.002542365549646467,0.002722753448135287,-0.005419218539278253,0.005204642776111294
+2.246300273206941,0.57,1.0,56.0,-0.001752451307931949,0.001843117668189095,-0.003474789991815972,0.0035217739694092852
+2.246300273206941,0.63,1.0,55.0,-0.001264536572616563,0.0012336957254720684,-0.0024297573724658297,0.0023935745523555227
+2.246300273206941,0.69,1.0,81.0,-0.0009218020076400073,0.0009173359377557162,-0.001903906396388504,0.0018080960225410028
+2.246300273206941,0.75,1.0,42.0,-0.001209199376051708,0.0010475305459890856,-0.002404225774671985,0.00201772955322283
+2.246300273206941,0.81,1.0,8.0,-0.0006984496756031328,0.0006997229965938351,-0.0014080427374650734,0.0012749458240914058
+2.853821938497898,0.15,1.0,6.0,-0.005385474960895843,0.005385474960895847,-0.01135505101421458,0.010969593547837239
+2.853821938497898,0.21,1.0,16.0,-0.0021358455034013084,0.0020786205048206165,-0.004303467224591073,0.004141097946268528
+2.853821938497898,0.27,1.0,36.0,-0.002240007052099285,0.0021201412666814103,-0.004559921217536945,0.004085804175613722
+2.853821938497898,0.33,1.0,59.0,-0.0020107939811367073,0.001757911983302249,-0.0039764742607804856,0.003535537574218262
+2.853821938497898,0.39,1.0,45.0,-0.0020990988021676532,0.0017968749965886998,-0.004273344562955954,0.0032338113616318487
+2.853821938497898,0.45,1.0,58.0,-0.0020067384297347978,0.001981350358798947,-0.0040634664026409015,0.0037703826251001523
+2.853821938497898,0.51,1.0,51.0,-0.0019135159674989204,0.0019826138265239325,-0.003837926630456428,0.0038844064850068524
+2.853821938497898,0.57,1.0,50.0,-0.0018578037161045952,0.0018359066605919047,-0.0037546954889749137,0.0036865208095532434
+2.853821938497898,0.63,1.0,50.0,-0.0014617873510478743,0.0013904418762563026,-0.0029288385098015534,0.0027226540043216218
+2.853821938497898,0.69,1.0,80.0,-0.0010692339248070028,0.0009661640938298473,-0.0020986793488447972,0.0019010581189856375
+2.853821938497898,0.75,1.0,41.0,-0.0014391815070720067,0.00121133076405522,-0.0030732754114218093,0.0022462950274367735
+2.853821938497898,0.81,1.0,6.0,-0.0009051825187802818,0.0007756562534616361,-0.0018049754433031764,0.0014293977735864351
+3.625650476828133,0.15,1.0,5.0,-0.003540575143775105,0.0048923285445425565,-0.004892328544542557,0.012524944678055872
+3.625650476828133,0.21,1.0,21.0,-0.002182421588976519,0.00197602412838834,-0.004605741673012002,0.0036569316689897538
+3.625650476828133,0.27,1.0,35.0,-0.001918359345582971,0.0018350154185601563,-0.0035568572669334403,0.0036863011526002253
+3.625650476828133,0.33,1.0,67.0,-0.0015870513936507538,0.0014744327993168346,-0.0031482370144717982,0.0028791338533395616
+3.625650476828133,0.39,1.0,48.0,-0.002365449221571151,0.001878272101832803,-0.004802315973560378,0.003626992144955445
+3.625650476828133,0.45,1.0,50.0,-0.001970272502456049,0.0019058550626548558,-0.00376453999604512,0.0038870775852134845
+3.625650476828133,0.51,1.0,54.0,-0.0014253832093100486,0.0014597080905591558,-0.0029663489418765465,0.0028181119937931262
+3.625650476828133,0.57,1.0,51.0,-0.0017711428194530344,0.0017241059230832946,-0.0034671453701631623,0.0034807447806530925
+3.625650476828133,0.63,1.0,43.0,-0.0018107096578942607,0.0016259164728421821,-0.003906514106926058,0.0029491873917385993
+3.625650476828133,0.69,1.0,77.0,-0.0010871531454733796,0.0011473435939807414,-0.0021747768725436556,0.002181165561682485
+3.625650476828133,0.75,1.0,38.0,-0.0017052128866372784,0.001359475153450085,-0.003298456927365378,0.0026239623353534434
+3.625650476828133,0.81,1.0,9.0,-0.004214194799927592,0.0026248551454182787,-0.008832515883292548,0.004781279210900485
+4.606223395648514,0.15,1.0,5.0,-0.002493144074089094,0.00427490718195409,-0.0041517074324147535,0.009459337856133909
+4.606223395648514,0.21,1.0,23.0,-0.0019737018529867433,0.0016411021780488554,-0.003927998407095677,0.0032679806285231205
+4.606223395648514,0.27,1.0,42.0,-0.0013128875390076488,0.001323218828081256,-0.0026725599921661905,0.0025879351931942327
+4.606223395648514,0.33,1.0,57.0,-0.0015417716810727069,0.0013464617016887537,-0.003042991832181969,0.002645151400243194
+4.606223395648514,0.39,1.0,54.0,-0.0018190438889176255,0.0015734224749528616,-0.0035962099682064095,0.002984041587194203
+4.606223395648514,0.45,1.0,52.0,-0.001783151379883096,0.0017410160121411342,-0.003641497441649185,0.003250284720602264
+4.606223395648514,0.51,1.0,51.0,-0.0013730721398597875,0.0013303797942578746,-0.0027398862808305805,0.002536530485755165
+4.606223395648514,0.57,1.0,49.0,-0.0016972664526567287,0.0017528654278187658,-0.003410250993190016,0.003388320790514438
+4.606223395648514,0.63,1.0,53.0,-0.00163475054928579,0.001412606638094664,-0.003086448515804017,0.0027562253397751674
+4.606223395648514,0.69,1.0,65.0,-0.0012644970799804375,0.0012652255928275813,-0.002588284770887609,0.0023712065255328905
+4.606223395648514,0.75,1.0,38.0,-0.001794669399955994,0.0016556813783257108,-0.003504040751635895,0.0031940453623850043
+4.606223395648514,0.81,1.0,7.0,-0.004571770446303619,0.0029799556401114364,-0.009840152708649857,0.005178179297075759
+5.851996519306434,0.15,1.0,9.0,-0.0020365461021729396,0.0022264658658747534,-0.003915602905514527,0.004337467521752545
+5.851996519306434,0.21,1.0,21.0,-0.0022444332021509246,0.00188289514402688,-0.004619412256706936,0.0037064465037824302
+5.851996519306434,0.27,1.0,51.0,-0.001481660342163012,0.001317457959341755,-0.002893815326675942,0.0026310581926052784
+5.851996519306434,0.33,1.0,49.0,-0.0016845031733528297,0.0013231400858029606,-0.003354762680646553,0.0025900446228529048
+5.851996519306434,0.39,1.0,55.0,-0.0013309202765109543,0.0012551360379791645,-0.0026953368307948227,0.0024494747225050225
+5.851996519306434,0.45,1.0,56.0,-0.00158340636136164,0.0015253377526684747,-0.003121218958495585,0.002879208155073992
+5.851996519306434,0.51,1.0,55.0,-0.0013420082156208333,0.0012610721983918978,-0.0026071140735412527,0.002515211441829038
+5.851996519306434,0.57,1.0,49.0,-0.0018453280767043155,0.0018108882589693922,-0.0034294676786381156,0.003756940722156494
+5.851996519306434,0.63,1.0,52.0,-0.0015899022159585484,0.0015102604299363797,-0.0031058506084574253,0.0029933874055667452
+5.851996519306434,0.69,1.0,55.0,-0.001716678667890124,0.0016081794739965093,-0.0033942974112240528,0.0031193687952986325
+5.851996519306434,0.75,1.0,34.0,-0.0024269785710924773,0.002447211766626559,-0.005111370379200967,0.004562020332114852
+5.851996519306434,0.81,1.0,9.0,-0.00412731551339248,0.002914206567844703,-0.00837061087465084,0.005355961506577654
+5.851996519306434,0.87,1.0,5.0,-0.0005825059182106067,0.0007949183655467714,-0.0010496260397874207,0.0014950830895517526
+7.434694395049644,0.15,1.0,8.0,-0.0014098512247225083,0.0016546708095394186,-0.002825849083761465,0.003166385095674009
+7.434694395049644,0.21,1.0,26.0,-0.001509418541020555,0.0015908640640975307,-0.0031141236186194004,0.00298054413565889
+7.434694395049644,0.27,1.0,50.0,-0.0014239058904363697,0.0012084336119363118,-0.002880205541996483,0.0024190594579789134
+7.434694395049644,0.33,1.0,51.0,-0.0011649610558332943,0.0010501035128061382,-0.00232252680509125,0.002054293031814348
+7.434694395049644,0.39,1.0,58.0,-0.0009934610940260584,0.0009690009538400386,-0.0018537314080636755,0.001967565245167108
+7.434694395049644,0.45,1.0,56.0,-0.0016241516069092586,0.001621839161443115,-0.003233223722328332,0.00308491552479553
+7.434694395049644,0.51,1.0,58.0,-0.0016155776066287546,0.0016925240545873845,-0.0032034225955568057,0.003250878414881183
+7.434694395049644,0.57,1.0,48.0,-0.0022249539577629857,0.002283283920121347,-0.004376881631029457,0.004453374932754906
+7.434694395049644,0.63,1.0,50.0,-0.002370437898125558,0.0021878762823316837,-0.004761876521772099,0.004160206193901234
+7.434694395049644,0.69,1.0,50.0,-0.0030500240877279956,0.002704157909280559,-0.006346583702454352,0.0049392859491483
+7.434694395049644,0.75,1.0,29.0,-0.004433155081370028,0.0041132556339667945,-0.008976334776014925,0.008137401037302401
+7.434694395049644,0.81,1.0,10.0,-0.005331453363953242,0.004133025929534948,-0.010902998175978666,0.007806937199272523
+9.44543978545179,0.15,1.0,6.0,-0.002011134157968738,0.0017836923156201816,-0.004769730578522406,0.0029223915580534054
+9.44543978545179,0.21,1.0,26.0,-0.001659875088671142,0.001524547279015663,-0.0031751650974109914,0.0030427932979458557
+9.44543978545179,0.27,1.0,52.0,-0.0014107503581150468,0.0013943798844370916,-0.002911393121980368,0.002652001480922464
+9.44543978545179,0.33,1.0,61.0,-0.0010990256590393038,0.0011853639007145843,-0.0022280571909618096,0.0023105559352801053
+9.44543978545179,0.39,1.0,54.0,-0.001708615402074697,0.0017388145423855533,-0.0033903787145609654,0.0032413697353885075
+9.44543978545179,0.45,1.0,59.0,-0.002613286851701523,0.0024899757796105417,-0.005275931183627892,0.004890341831475502
+9.44543978545179,0.51,1.0,68.0,-0.0021332091912120185,0.0021294069039428046,-0.004130222103340916,0.0041928965464091954
+9.44543978545179,0.57,1.0,41.0,-0.003395921521051179,0.0029963432636322626,-0.0068312524810401455,0.005601797121099693
+9.44543978545179,0.63,1.0,46.0,-0.004348529537467151,0.0036460969487226713,-0.009047327901482542,0.006903855361050496
+9.44543978545179,0.69,1.0,43.0,-0.006159362329097519,0.005550800937636874,-0.011938631905333631,0.010851081450654663
+9.44543978545179,0.75,1.0,24.0,-0.00866584839178922,0.008573770853059428,-0.01721389482316669,0.016457418255095075
+9.44543978545179,0.81,1.0,8.0,-0.006187326719057492,0.007688113365115989,-0.011262373548344834,0.016091946303468493
+9.44543978545179,0.87,1.0,8.0,-0.008211422972863619,0.006897385825062441,-0.017562942021668027,0.012355899033363253
+12.000000000000009,0.15,1.0,6.0,-0.004526757754130785,0.003108188516277831,-0.011026193357830852,0.004950729828320438
+12.000000000000009,0.21,1.0,26.0,-0.0019883930565449998,0.0018326595022059929,-0.003976647304531013,0.003488782909878458
+12.000000000000009,0.27,1.0,57.0,-0.0015558048110612442,0.0015227637946874939,-0.0030821952914543926,0.003014798452007991
+12.000000000000009,0.33,1.0,69.0,-0.0016465366543695838,0.0017484241286278425,-0.0032611107818177835,0.003364209950917797
+12.000000000000009,0.39,1.0,47.0,-0.00308185270914833,0.002878812166850226,-0.00649032193207337,0.005281475813819468
+12.000000000000009,0.45,1.0,56.0,-0.004188060232752683,0.00392067191949935,-0.008612353691465032,0.007403714867634718
+12.000000000000009,0.51,1.0,70.0,-0.0032485223638774397,0.003490571991225721,-0.00662774711200682,0.006707501657339887
+12.000000000000009,0.57,1.0,45.0,-0.0051041683807396985,0.004605156767089912,-0.009681326683354748,0.00879716867241895
+12.000000000000009,0.63,1.0,37.0,-0.007979517800704826,0.00617280166475389,-0.01686910886687354,0.011188188697631198
+12.000000000000009,0.69,1.0,37.0,-0.011185558754913017,0.009528719944032284,-0.02158682539268302,0.018714457720351386
+12.000000000000009,0.75,1.0,16.0,-0.015956697438081504,0.01758286840568067,-0.02927983474045416,0.03680446819279188
+12.000000000000009,0.81,1.0,12.0,-0.010589678661752639,0.009249800747604441,-0.022060664030687956,0.01686689913571717
+12.000000000000009,0.87,1.0,11.0,-0.007229462597695795,0.007010024827804577,-0.013080633577375876,0.014258635315407596
+12.000000000000009,0.93,1.0,9.0,-0.010729810996418586,0.0096804912979453,-0.021845795935398205,0.017602528693318766
+0.1000000000000366,0.27,2.0,20.0,-5.523002361556651e-05,4.9907923019239134e-05,-0.0001076991823311386,9.751440655317508e-05
+0.1000000000000366,0.33,2.0,35.0,-3.3905646753570256e-05,3.234424930502959e-05,-6.716176403751189e-05,6.444748989701086e-05
+0.1000000000000366,0.39,2.0,54.0,-2.5886078235510707e-05,2.3076339581102303e-05,-5.263652376061529e-05,4.332686068836225e-05
+0.1000000000000366,0.45,2.0,58.0,-1.842774567865027e-05,1.6068740894939444e-05,-3.474002636589896e-05,3.1495613092013e-05
+0.1000000000000366,0.51,2.0,51.0,-2.1076269726442668e-05,2.4261888507096897e-05,-3.9852432455539156e-05,4.999453709166591e-05
+0.1000000000000366,0.57,2.0,51.0,-2.138235692820742e-05,2.7854569964483594e-05,-3.960166909133364e-05,5.690768285328146e-05
+0.1000000000000366,0.63,2.0,58.0,-2.665809772513907e-05,3.138590247146068e-05,-5.137324600011336e-05,6.350621337927036e-05
+0.1000000000000366,0.69,2.0,52.0,-2.91753059489171e-05,3.5611658777438865e-05,-5.5864365842675983e-05,7.193469504681064e-05
+0.1000000000000366,0.75,2.0,38.0,-3.270496999262289e-05,3.9983893849380797e-05,-6.122980726389375e-05,8.432820270441671e-05
+0.1000000000000366,0.81,2.0,32.0,-4.589743912765183e-05,4.718216345963142e-05,-9.052322131235946e-05,9.20829911351204e-05
+0.1000000000000366,0.87,2.0,19.0,-5.702052961073453e-05,2.830180027542074e-05,-0.00011900937967279417,3.029795812715461e-05
+0.1000000000000366,0.93,2.0,24.0,-7.336242652442312e-07,7.158564847674038e-07,-1.467272575788024e-06,1.3656830187944076e-06
+0.1270454343320758,0.27,2.0,20.0,-7.722397237077456e-05,6.988945138153571e-05,-0.00015500331807084903,0.00012973517868318524
+0.1270454343320758,0.33,2.0,35.0,-4.810443137936222e-05,4.752954816985436e-05,-9.714246396283084e-05,9.01208617479088e-05
+0.1270454343320758,0.39,2.0,54.0,-3.727169358645666e-05,3.136842764486954e-05,-7.69636124581343e-05,6.0167541157614334e-05
+0.1270454343320758,0.45,2.0,58.0,-2.4821473704584657e-05,2.1706453922583805e-05,-4.9210145799414024e-05,4.2543919865251145e-05
+0.1270454343320758,0.51,2.0,51.0,-2.6555317324325283e-05,2.7138557958444462e-05,-5.421604077382534e-05,5.406664341092282e-05
+0.1270454343320758,0.57,2.0,51.0,-2.3085942443626818e-05,2.884828768074663e-05,-4.446671732812876e-05,5.8164181151075424e-05
+0.1270454343320758,0.63,2.0,58.0,-2.7455128178213287e-05,3.2719778231616956e-05,-5.2545878314316655e-05,6.647300068157631e-05
+0.1270454343320758,0.69,2.0,52.0,-3.0179069401015256e-05,3.491190181554538e-05,-5.7074638580809646e-05,7.343100223225986e-05
+0.1270454343320758,0.75,2.0,38.0,-3.299474447362026e-05,4.032660664205538e-05,-6.268759938701161e-05,8.735401177087523e-05
+0.1270454343320758,0.81,2.0,32.0,-4.5598382389333664e-05,4.87859139184532e-05,-8.897862096748343e-05,9.347630450970116e-05
+0.1270454343320758,0.87,2.0,19.0,-5.625347051947813e-05,2.8422050786923895e-05,-0.00011994365937571549,3.096644447901016e-05
+0.1270454343320758,0.93,2.0,24.0,-1.126879204450139e-06,1.0910947021308332e-06,-2.2737288722330904e-06,2.0438791608576656e-06
+0.1614054238461723,0.27,2.0,20.0,-0.0001121856913959188,0.00011138394099586077,-0.00024178256193747502,0.0002036425137449154
+0.1614054238461723,0.33,2.0,35.0,-7.285782370385133e-05,7.399971049103568e-05,-0.00014992150467200706,0.00013963927277183186
+0.1614054238461723,0.39,2.0,54.0,-5.8910067128679375e-05,5.1721235618322896e-05,-0.0001215523006588347,9.664571280226728e-05
+0.1614054238461723,0.45,2.0,59.0,-3.7983456586672325e-05,3.312282974805984e-05,-7.428203531895909e-05,6.25217592888425e-05
+0.1614054238461723,0.51,2.0,50.0,-4.1429254645874055e-05,3.496561104234405e-05,-8.29472775121661e-05,6.798924347186378e-05
+0.1614054238461723,0.57,2.0,51.0,-2.8096848823356347e-05,3.106373320801373e-05,-5.408595113788542e-05,6.169887462028594e-05
+0.1614054238461723,0.63,2.0,58.0,-3.149535334619933e-05,3.40661223674219e-05,-5.789923443199546e-05,7.004294476209431e-05
+0.1614054238461723,0.69,2.0,52.0,-3.1718585972276564e-05,3.623595906525535e-05,-5.9771280120891964e-05,7.561456011678393e-05
+0.1614054238461723,0.75,2.0,39.0,-3.225846346089908e-05,3.938421669850004e-05,-6.044040487314523e-05,8.407097188963865e-05
+0.1614054238461723,0.81,2.0,31.0,-4.731828807947166e-05,5.016303276144919e-05,-9.48949477482087e-05,9.286355330854648e-05
+0.1614054238461723,0.87,2.0,19.0,-5.7455891566537846e-05,2.84053105441343e-05,-0.0001242461396327118,3.215349904861195e-05
+0.1614054238461723,0.93,2.0,24.0,-1.5950949614128284e-06,1.3855570715643077e-06,-3.073784950557337e-06,2.7859949794478456e-06
+0.2050582217609406,0.27,2.0,20.0,-0.00020491101148738025,0.00018393908303517405,-0.0004250416762101468,0.00035704066654974306
+0.2050582217609406,0.33,2.0,37.0,-0.00012337828096281537,0.00012336377177201108,-0.00025793544408465315,0.00023455354399371702
+0.2050582217609406,0.39,2.0,52.0,-9.979730077593508e-05,9.383998355237837e-05,-0.00021893906962380604,0.00016807902947253047
+0.2050582217609406,0.45,2.0,60.0,-6.494236964945454e-05,6.143375960607961e-05,-0.00013469870953671832,0.00011278378247880391
+0.2050582217609406,0.51,2.0,49.0,-5.635278887562987e-05,5.1852328186411204e-05,-0.00011204134875519876,0.00010114655092107761
+0.2050582217609406,0.57,2.0,51.0,-4.225654776338237e-05,4.128295835207668e-05,-8.445503722149192e-05,8.010773422930997e-05
+0.2050582217609406,0.63,2.0,58.0,-3.8217511119203104e-05,4.3402655906198253e-05,-7.463261740916862e-05,8.370985480141438e-05
+0.2050582217609406,0.69,2.0,52.0,-3.764007755857197e-05,4.215008845935545e-05,-7.4259166323918e-05,8.509093035926772e-05
+0.2050582217609406,0.75,2.0,39.0,-3.60751616722334e-05,4.467719372682879e-05,-7.005826887569268e-05,9.439025657363554e-05
+0.2050582217609406,0.81,2.0,31.0,-5.614591489149028e-05,5.232638205082551e-05,-0.00010644466840637059,0.00010319295094292748
+0.2050582217609406,0.87,2.0,19.0,-6.301993452517471e-05,3.12978797805067e-05,-0.00013976474232541312,3.646598854467998e-05
+0.2050582217609406,0.93,2.0,24.0,-2.30060706704885e-06,2.197223256698892e-06,-4.717615225176905e-06,4.31875316738657e-06
+0.2605171084697874,0.27,2.0,21.0,-0.0003267044050197467,0.00031052856391227334,-0.0006736785723775545,0.0005636806504579591
+0.2605171084697874,0.33,2.0,36.0,-0.00022798445634337517,0.00021150354510426537,-0.00044064648149736286,0.00041120376140987874
+0.2605171084697874,0.39,2.0,53.0,-0.00017284508048944402,0.00015090333492796966,-0.0003513294666391599,0.0002897088935383112
+0.2605171084697874,0.45,2.0,60.0,-0.00011198639222638435,0.0001033415828399368,-0.00023175629579431388,0.00019067076939623446
+0.2605171084697874,0.51,2.0,48.0,-9.025244511858314e-05,8.403305319318372e-05,-0.0001783864665302962,0.00015946304984647427
+0.2605171084697874,0.57,2.0,51.0,-6.836264343690802e-05,6.169540799507025e-05,-0.00013971574128025753,0.00011995753440722139
+0.2605171084697874,0.63,2.0,58.0,-5.571842036181208e-05,5.995362383291787e-05,-0.00011021205848717567,0.00012041833936496447
+0.2605171084697874,0.69,2.0,52.0,-5.251445978423955e-05,5.879217446749549e-05,-9.939380699426896e-05,0.00012082294129227282
+0.2605171084697874,0.75,2.0,39.0,-4.990418149755371e-05,6.06903936083157e-05,-9.506090167473656e-05,0.0001232973959960906
+0.2605171084697874,0.81,2.0,31.0,-7.38730616469352e-05,7.494287866158968e-05,-0.00014537309817392674,0.00013878469976264386
+0.2605171084697874,0.87,2.0,19.0,-8.139210441135055e-05,3.954650317888978e-05,-0.0001824682693007746,5.0836912051578534e-05
+0.2605171084697874,0.93,2.0,24.0,-4.599907448651115e-06,4.599902934739401e-06,-9.371198043026288e-06,8.618096932126059e-06
+0.3309750919646709,0.27,2.0,21.0,-0.0005264678895411637,0.000506897530579974,-0.0010883697468538232,0.0009259670526443567
+0.3309750919646709,0.33,2.0,36.0,-0.0003870215947908857,0.00034980224239963527,-0.0007540682673148005,0.000700070121572675
+0.3309750919646709,0.39,2.0,54.0,-0.0002889365781291621,0.0002544703347687864,-0.0006161665155760525,0.00048417489820188323
+0.3309750919646709,0.45,2.0,60.0,-0.00019591228535121154,0.000167892821940353,-0.00037913372401217603,0.00032008532045615636
+0.3309750919646709,0.51,2.0,48.0,-0.00015257007395163283,0.00013228527244540632,-0.0003067540296307114,0.0002525954823260371
+0.3309750919646709,0.57,2.0,50.0,-0.00011132139571468128,9.43912035457969e-05,-0.00023544748329850198,0.00018323711297820014
+0.3309750919646709,0.63,2.0,58.0,-7.83874258969009e-05,8.619909689494555e-05,-0.00015705356117187488,0.00016074904842097815
+0.3309750919646709,0.69,2.0,52.0,-6.922062370750138e-05,7.559445436032621e-05,-0.0001282503468481905,0.00015479021239728943
+0.3309750919646709,0.75,2.0,39.0,-6.226809162296233e-05,7.639017122481851e-05,-0.00012084648920972256,0.00014883271053124864
+0.3309750919646709,0.81,2.0,31.0,-8.93728928918568e-05,8.737412361336539e-05,-0.00017304846191118573,0.00016997731842970592
+0.3309750919646709,0.87,2.0,19.0,-8.41616649152029e-05,4.206039097871818e-05,-0.00020982322702441854,6.140668840080938e-05
+0.3309750919646709,0.93,2.0,24.0,-9.447479847733423e-06,8.540044384597122e-06,-1.9621193411545993e-05,1.594564649156558e-05
+0.4204887431174289,0.27,2.0,21.0,-0.0008486707358973444,0.0008180433615547116,-0.001755366833835199,0.001478842902738507
+0.4204887431174289,0.33,2.0,36.0,-0.0006266920360262808,0.0005951199288965355,-0.001186771493696103,0.0011707004077059163
+0.4204887431174289,0.39,2.0,56.0,-0.00047646134067020344,0.0004066826110050274,-0.0009521952678148224,0.0007722195530316031
+0.4204887431174289,0.45,2.0,58.0,-0.00032403770290807636,0.0002904615050385616,-0.0006561648897338158,0.0005640656597951306
+0.4204887431174289,0.51,2.0,50.0,-0.00022935419906893866,0.00020764009395579883,-0.00046532915734564053,0.0003906824603256893
+0.4204887431174289,0.57,2.0,47.0,-0.0001773581063602152,0.0001605790824970324,-0.0003664587940324481,0.00029080404571531703
+0.4204887431174289,0.63,2.0,59.0,-0.00011315341210368879,0.00010305355764824466,-0.00022838395670225306,0.00020355452966208627
+0.4204887431174289,0.69,2.0,53.0,-8.427154728812813e-05,9.164961304522441e-05,-0.00016802694075970865,0.0001798391267413113
+0.4204887431174289,0.75,2.0,38.0,-7.530439984486887e-05,8.900943364911461e-05,-0.0001405632670498221,0.00018211534597808082
+0.4204887431174289,0.81,2.0,31.0,-0.00010170674025870666,0.00010547171717190705,-0.00019809212959380338,0.00019689497994115858
+0.4204887431174289,0.87,2.0,19.0,-8.745349733184608e-05,4.593731746178118e-05,-0.00021202543780891015,7.139736437711155e-05
+0.4204887431174289,0.93,2.0,24.0,-1.238147779122759e-05,1.0858271943765322e-05,-2.5104777081753656e-05,2.078718603669077e-05
+0.5342117500110221,0.27,2.0,21.0,-0.0013240460711206688,0.0012253107863222927,-0.0026498852632287307,0.002259172259382866
+0.5342117500110221,0.33,2.0,37.0,-0.0009471623484658936,0.0008853422762517677,-0.0018409364981561021,0.0017564536462815982
+0.5342117500110221,0.39,2.0,56.0,-0.0007491178790162229,0.0006272146652949252,-0.0014970481858637102,0.0011752424443473998
+0.5342117500110221,0.45,2.0,57.0,-0.0005244570880116735,0.0004758361895375916,-0.0011083202798781487,0.000913015897171252
+0.5342117500110221,0.51,2.0,52.0,-0.0003487785671851888,0.0003165468351633412,-0.0007101490175215988,0.0006063155344559597
+0.5342117500110221,0.57,2.0,47.0,-0.00026907756042719407,0.00021899643951870437,-0.0005711842375002592,0.00042002493796883304
+0.5342117500110221,0.63,2.0,57.0,-0.0001591087193370057,0.00015583483661435197,-0.00033660437881965024,0.00028745166269311613
+0.5342117500110221,0.69,2.0,54.0,-0.0001155421987615926,0.00011650398965805115,-0.00021403353751659753,0.00023156295913463458
+0.5342117500110221,0.75,2.0,38.0,-9.748772109379033e-05,0.00011285913888613259,-0.00018534901801071615,0.0002256577860600606
+0.5342117500110221,0.81,2.0,30.0,-0.00012627050800078163,0.00013194740738778373,-0.00024182959322955081,0.0002492514526069106
+0.5342117500110221,0.87,2.0,19.0,-0.00010804002778920426,5.557715200793769e-05,-0.0002564122786994198,9.193018623013222e-05
+0.5342117500110221,0.93,2.0,24.0,-1.925864211687658e-05,1.5724925344722793e-05,-3.8897933054456015e-05,2.8856196601681457e-05
+0.6786916380543664,0.21,2.0,5.0,-0.004055358165627699,0.006309116741982135,-0.007938798500775546,0.011851670205615793
+0.6786916380543664,0.27,2.0,20.0,-0.00201083203136042,0.0017626001544437224,-0.004065830025036115,0.0034103827154562793
+0.6786916380543664,0.33,2.0,37.0,-0.001460972958858673,0.001332575704549553,-0.002797795631432754,0.0026196416075920746
+0.6786916380543664,0.39,2.0,57.0,-0.001109275701995618,0.0009291290409436872,-0.002262451155627537,0.0018568701742296219
+0.6786916380543664,0.45,2.0,56.0,-0.0008498688219351636,0.0007171503920504599,-0.001672730440986145,0.0013789885719665785
+0.6786916380543664,0.51,2.0,53.0,-0.0005439986492830601,0.0004546017267090654,-0.0010834191133243006,0.0009431491430148055
+0.6786916380543664,0.57,2.0,47.0,-0.00041651541046455005,0.00034907614221263525,-0.0008423136869141835,0.0006674497741667085
+0.6786916380543664,0.63,2.0,56.0,-0.00023000538562849274,0.00021414734622783393,-0.00048823230233188426,0.0004186093034817171
+0.6786916380543664,0.69,2.0,56.0,-0.00015144780974020577,0.00015599660954089228,-0.0002940452215718939,0.0003145501212464429
+0.6786916380543664,0.75,2.0,37.0,-0.00013758622144357125,0.0001403990685924833,-0.00024638529946932565,0.00029778599243763236
+0.6786916380543664,0.81,2.0,30.0,-0.00015647201198872048,0.00015324614684262392,-0.0002955058069519245,0.00030729616645922036
+0.6786916380543664,0.87,2.0,18.0,-0.0001326856717384743,7.83100162833048e-05,-0.00030744553410713633,0.0001412426605042865
+0.6786916380543664,0.93,2.0,23.0,-3.175628747841411e-05,2.4659665570391087e-05,-6.854390915991509e-05,4.4836013425415736e-05
+0.6786916380543664,0.99,2.0,5.0,-9.244015756637536e-06,9.03706225865446e-06,-1.8281078015291953e-05,1.753885884738797e-05
+0.862246739341487,0.21,2.0,5.0,-0.00557524776708398,0.007033097141185228,-0.009858024718720106,0.014275261201784396
+0.862246739341487,0.27,2.0,21.0,-0.0026893392299972584,0.0023965366201113693,-0.005460753116804345,0.004322018835538025
+0.862246739341487,0.33,2.0,39.0,-0.001836975311161425,0.0019391625686294054,-0.003777322444286805,0.003557500689634635
+0.862246739341487,0.39,2.0,56.0,-0.0016726501691752581,0.0013752572978351731,-0.0034146020575440625,0.002620315444989627
+0.862246739341487,0.45,2.0,55.0,-0.0011836597132191106,0.0010654757154055627,-0.002386869109386466,0.002046952531308928
+0.862246739341487,0.51,2.0,53.0,-0.0009500284515024149,0.0007897740921376903,-0.001840215567026836,0.0015000263316276004
+0.862246739341487,0.57,2.0,47.0,-0.0005969586521103561,0.0005580658021095825,-0.0012975668335966685,0.0009987655958853185
+0.862246739341487,0.63,2.0,56.0,-0.00037144770438633063,0.00030373680615552177,-0.00072356279145906,0.0006085164907591708
+0.862246739341487,0.69,2.0,55.0,-0.00023219634584878087,0.0002242571773768959,-0.00044312578009916186,0.00045488829688482345
+0.862246739341487,0.75,2.0,37.0,-0.0001837967095001206,0.0002054858162629307,-0.0003673638814471538,0.00040496451016038394
+0.862246739341487,0.81,2.0,30.0,-0.00019022783175263368,0.000200156169630948,-0.00039265426721772113,0.0003748348141143324
+0.862246739341487,0.87,2.0,17.0,-0.00017606358619934374,0.00013135856542271525,-0.0003604659446295401,0.00023565397424925072
+0.862246739341487,0.93,2.0,24.0,-5.844645991921704e-05,4.090746102295211e-05,-0.00012997087405359353,7.481494190063841e-05
+0.862246739341487,0.99,2.0,5.0,-2.6485448441437875e-05,1.8603755683077574e-05,-5.5135587348598157e-05,3.270288824892551e-05
+1.0954451150103786,0.21,2.0,5.0,-0.006896822649353785,0.006843992281562716,-0.012604760329879162,0.014282724553490533
+1.0954451150103786,0.27,2.0,22.0,-0.003469632784723403,0.002969914246449843,-0.006614539361264403,0.00579380488936331
+1.0954451150103786,0.33,2.0,40.0,-0.0026192693901753916,0.0025135722404257994,-0.005139241138498828,0.005028365922671389
+1.0954451150103786,0.39,2.0,56.0,-0.0022339301438612097,0.0019303736731549833,-0.004522466863125303,0.0038207829555161423
+1.0954451150103786,0.45,2.0,55.0,-0.001755106436101372,0.001534246707888388,-0.0034599306523096876,0.002978316095340588
+1.0954451150103786,0.51,2.0,54.0,-0.0013801730607752181,0.0011425829112766857,-0.0027327493500138847,0.002268031847669479
+1.0954451150103786,0.57,2.0,43.0,-0.0009965112030420622,0.0008159847170132048,-0.0020091980505237386,0.0016437200238894401
+1.0954451150103786,0.63,2.0,56.0,-0.0005479535627514175,0.0004766931552870174,-0.0010839863349710423,0.0009155923730667985
+1.0954451150103786,0.69,2.0,55.0,-0.00033298613576321736,0.0003211888402484538,-0.0006556607999462875,0.0006275052941703967
+1.0954451150103786,0.75,2.0,41.0,-0.00023192216231365394,0.000271267616145251,-0.00046367605194216834,0.0005337802373525832
+1.0954451150103786,0.81,2.0,26.0,-0.0002837661085319537,0.00025884818589621476,-0.0005481836351812335,0.0005094815759627878
+1.0954451150103786,0.87,2.0,18.0,-0.00022772616350869658,0.00018668829171894803,-0.00048150794370651413,0.00034286960450766705
+1.0954451150103786,0.93,2.0,24.0,-0.00010813732940297985,6.866065959469447e-05,-0.00022608270419852985,0.00013013080450540923
+1.0954451150103786,0.99,2.0,5.0,-6.19148526773472e-05,4.110935616701282e-05,-0.00011453886494967591,7.120569308236568e-05
+1.3917130042342023,0.21,2.0,5.0,-0.0065561944861561635,0.006077575173239746,-0.01263376965939591,0.01204090958300923
+1.3917130042342023,0.27,2.0,23.0,-0.003583669385267379,0.0029425903391525187,-0.00682042371640905,0.006040842497876397
+1.3917130042342023,0.33,2.0,42.0,-0.002876455923530322,0.0029362610681258334,-0.005684159739838847,0.005735785399697291
+1.3917130042342023,0.39,2.0,53.0,-0.0030193425825022443,0.0026287050061298356,-0.005948347272826019,0.004909857938104298
+1.3917130042342023,0.45,2.0,56.0,-0.002258891152746819,0.001958711827379995,-0.0044589179558895495,0.0038161143191748933
+1.3917130042342023,0.51,2.0,57.0,-0.001959190134968791,0.001700923005626483,-0.003955249833815874,0.003297974812798483
+1.3917130042342023,0.57,2.0,42.0,-0.0012012863449513231,0.0010830052302918244,-0.002436949153823323,0.0020079977091711247
+1.3917130042342023,0.63,2.0,56.0,-0.0007905854307872899,0.000672416909832134,-0.0015966610078415584,0.0012830017044560794
+1.3917130042342023,0.69,2.0,53.0,-0.0004634103108329697,0.00046803227750267596,-0.0009493970953141424,0.0009238065899717746
+1.3917130042342023,0.75,2.0,40.0,-0.0003592434307466125,0.00036867169814840117,-0.0007041400171280934,0.0007184226643520247
+1.3917130042342023,0.81,2.0,26.0,-0.0003290393655082147,0.0002985077830459612,-0.0007088968603508127,0.0005634784578217321
+1.3917130042342023,0.87,2.0,18.0,-0.0003368975655104345,0.00027047101848112233,-0.0007135909831527937,0.0005050075043199742
+1.3917130042342023,0.93,2.0,24.0,-0.00019067886575611063,0.00011690724808056161,-0.0004374024892141555,0.0002097941134200702
+1.3917130042342023,0.99,2.0,5.0,-0.00013265290817292548,8.340399285888815e-05,-0.00023389474594288635,0.0001657149966957317
+1.768107830885019,0.21,2.0,5.0,-0.006127145894093222,0.005235702777261864,-0.01077626819651003,0.010412830991231692
+1.768107830885019,0.27,2.0,23.0,-0.0027420776852450078,0.0028223984499695124,-0.005706360273982593,0.005268403286867687
+1.768107830885019,0.33,2.0,46.0,-0.002813752237124929,0.0027378344563080224,-0.005431003175300432,0.0052561119016628355
+1.768107830885019,0.39,2.0,53.0,-0.003239316667727374,0.002914195538253925,-0.006505154238304575,0.005619592891729201
+1.768107830885019,0.45,2.0,52.0,-0.0027639094228803633,0.002278087873566273,-0.005355929809498644,0.0044738704176700075
+1.768107830885019,0.51,2.0,56.0,-0.002548155956095733,0.002172057583064258,-0.004895662119577792,0.004314464173703155
+1.768107830885019,0.57,2.0,44.0,-0.0015728494799311637,0.001460316755986712,-0.0031070197112149692,0.0028804321081149892
+1.768107830885019,0.63,2.0,55.0,-0.0010969167751348527,0.0009795709850570818,-0.002257158491990941,0.001832116855159183
+1.768107830885019,0.69,2.0,53.0,-0.0006170860195656352,0.0006581849624627612,-0.0012646366379202663,0.0012219176135389552
+1.768107830885019,0.75,2.0,38.0,-0.0005486506171312264,0.0005244527646314775,-0.0010799798202044662,0.0010280001713498291
+1.768107830885019,0.81,2.0,28.0,-0.0004497365880881377,0.00036915378194387314,-0.0008905818782504108,0.0006854082145731421
+1.768107830885019,0.87,2.0,17.0,-0.0005517410334599333,0.0004151942634629817,-0.0011211944602998497,0.0007657761810193993
+1.768107830885019,0.93,2.0,23.0,-0.0003239838407162422,0.00019691305884669401,-0.0008027554444455223,0.00033889324781506133
+1.768107830885019,0.99,2.0,7.0,-0.00014420984707570167,0.00012365976499766645,-0.00028483372492195614,0.0002336436235963467
+2.246300273206961,0.21,2.0,7.0,-0.003994828849062214,0.003994828849062217,-0.008007112871696784,0.0072421000231399635
+2.246300273206961,0.27,2.0,22.0,-0.0026654450113295547,0.0026428167893553394,-0.00518332604800743,0.005444214639919574
+2.246300273206961,0.33,2.0,48.0,-0.0023074842395455343,0.0023750770354120337,-0.0047281484112495645,0.004547740127344796
+2.246300273206961,0.39,2.0,55.0,-0.002928230437661617,0.002767408860336831,-0.005658436706593688,0.00527483723064795
+2.246300273206961,0.45,2.0,51.0,-0.0026368709101819284,0.0023791568191749092,-0.005362011586436617,0.004566228976935511
+2.246300273206961,0.51,2.0,53.0,-0.0029048492133511043,0.0027249344715879033,-0.0060394827029313205,0.004951831494084353
+2.246300273206961,0.57,2.0,44.0,-0.0020155453764040014,0.0018602118763552684,-0.0040537112807777905,0.003634277172112779
+2.246300273206961,0.63,2.0,55.0,-0.0013304442696715109,0.00126592282946087,-0.00278006614751669,0.0023822689358555405
+2.246300273206961,0.69,2.0,52.0,-0.0008723973078907176,0.0008091647655676809,-0.0016489061949190634,0.0016345627396540502
+2.246300273206961,0.75,2.0,37.0,-0.0008013656845957459,0.0007547849799753736,-0.0016323401693701153,0.0014707934237242484
+2.246300273206961,0.81,2.0,27.0,-0.0006992338222680661,0.0005827402118001843,-0.0014833117130239083,0.0010625866869580284
+2.246300273206961,0.87,2.0,18.0,-0.0008029293216026537,0.000603183340154419,-0.0017500673902866898,0.0010638841245627635
+2.246300273206961,0.93,2.0,22.0,-0.0005374163596763048,0.00032499097505337446,-0.001170145173923017,0.0005766459928486874
+2.246300273206961,0.99,2.0,9.0,-0.00017821806745329106,0.00018550126473957664,-0.00033166056350108185,0.0003868516850341663
+2.8538219384979215,0.21,2.0,7.0,-0.0031877194894360636,0.0034961122302431275,-0.006073797710526311,0.006935328736583645
+2.8538219384979215,0.27,2.0,22.0,-0.0025515840444986088,0.0027704832120812994,-0.005206629414964156,0.005267829403314913
+2.8538219384979215,0.33,2.0,50.0,-0.0019559220506149837,0.0020513989439010813,-0.0038928033921754018,0.003921627575458039
+2.8538219384979215,0.39,2.0,56.0,-0.002411077867097368,0.002385171672714442,-0.0048409788121073355,0.004688874393812374
+2.8538219384979215,0.45,2.0,50.0,-0.0023886564927342855,0.002170689426793789,-0.004728325175613083,0.004215808211733094
+2.8538219384979215,0.51,2.0,53.0,-0.0027097511385959314,0.0023599079054272658,-0.005508527396902692,0.004641041287906042
+2.8538219384979215,0.57,2.0,43.0,-0.0025428940788811824,0.0020894369748500514,-0.004937984582223873,0.0042253722521527134
+2.8538219384979215,0.63,2.0,55.0,-0.00164346855650752,0.0014948257762142315,-0.0033220183975861996,0.0029068654130602724
+2.8538219384979215,0.69,2.0,52.0,-0.0011303043533219487,0.001074453315584622,-0.002182864742823549,0.0021211518014364753
+2.8538219384979215,0.75,2.0,38.0,-0.0011097349449333018,0.0010187571030090307,-0.00229847665939194,0.001949648715946847
+2.8538219384979215,0.81,2.0,25.0,-0.0011029239538916835,0.0009082559090031497,-0.0022996640652962527,0.0017117500249895217
+2.8538219384979215,0.87,2.0,18.0,-0.0011281206412366036,0.0008554735312095467,-0.0024112161587532058,0.0015628405287576375
+2.8538219384979215,0.93,2.0,22.0,-0.0007335662383797211,0.00047343576309924625,-0.0016075579102323365,0.0008532445080546747
+2.8538219384979215,0.99,2.0,9.0,-0.00034664744659279557,0.000375669370418369,-0.0006335288525023347,0.0008053965970517148
+3.6256504768281186,0.21,2.0,7.0,-0.003391813110933854,0.003491219090153327,-0.006373383247968487,0.00701900394353533
+3.6256504768281186,0.27,2.0,23.0,-0.0024316259484363,0.0023596801762857484,-0.004560683143538813,0.00486381528208812
+3.6256504768281186,0.33,2.0,50.0,-0.0018414943597126797,0.0017679386604832128,-0.003570554875978348,0.0035494608431344173
+3.6256504768281186,0.39,2.0,56.0,-0.001954541849463597,0.0020524025718425955,-0.0041857694090283604,0.0037540626570833043
+3.6256504768281186,0.45,2.0,50.0,-0.002002844111068317,0.0018928680733123922,-0.004231671216050029,0.003454542147425519
+3.6256504768281186,0.51,2.0,53.0,-0.0022712519149384333,0.0020478244034641668,-0.004570448239409831,0.003919386761718374
+3.6256504768281186,0.57,2.0,42.0,-0.0022403431424316464,0.0021246876721436347,-0.004486214151206767,0.004053561982346077
+3.6256504768281186,0.63,2.0,54.0,-0.0016849134589687464,0.0015955832639269255,-0.003281806983526158,0.0030766805007901013
+3.6256504768281186,0.69,2.0,53.0,-0.001245861902017658,0.001213366946899979,-0.0024016094803332878,0.002388094035516781
+3.6256504768281186,0.75,2.0,37.0,-0.001513645852136088,0.001256311136163665,-0.002921656341147956,0.0026071259810176513
+3.6256504768281186,0.81,2.0,25.0,-0.0013167803915979392,0.001090865017260445,-0.0025756872729796646,0.002100608710081054
+3.6256504768281186,0.87,2.0,17.0,-0.0011056903458732672,0.0009004801771443714,-0.002277811127913221,0.001686356580511025
+3.6256504768281186,0.93,2.0,24.0,-0.000968353134963596,0.0007536891536810941,-0.002045630663487634,0.0013875377547836285
+3.6256504768281186,0.99,2.0,9.0,-0.0006161288488756114,0.000704739405556183,-0.0011386967361833485,0.0013807806527971424
+4.606223395648502,0.21,2.0,8.0,-0.004243471607500257,0.003209281730074913,-0.008147601459636817,0.006475872965873814
+4.606223395648502,0.27,2.0,22.0,-0.001900864728992268,0.001902616656206449,-0.0035408173978170223,0.003980959868002201
+4.606223395648502,0.33,2.0,52.0,-0.0016946729440667696,0.0017081956242764806,-0.0035170990992277346,0.0032810296467583916
+4.606223395648502,0.39,2.0,58.0,-0.0014980550948278074,0.0015027789060718768,-0.0030998972544463823,0.002929970886725154
+4.606223395648502,0.45,2.0,48.0,-0.0016138585364244057,0.0014851939886129258,-0.0032923658689049595,0.002813629294232319
+4.606223395648502,0.51,2.0,49.0,-0.0019242811451212361,0.001794963111926508,-0.004007746755904075,0.003533471307361229
+4.606223395648502,0.57,2.0,44.0,-0.0018921486623158597,0.001802617179066726,-0.003730495831019993,0.0035164804960261037
+4.606223395648502,0.63,2.0,53.0,-0.0013893195584661175,0.001392520543200606,-0.0028113314390889464,0.0025950104171908388
+4.606223395648502,0.69,2.0,50.0,-0.0011697352296147373,0.0011480151061114383,-0.0023048488833578165,0.0023646425078306696
+4.606223395648502,0.75,2.0,38.0,-0.0015805553312723626,0.001623218857892701,-0.0031636458209716796,0.003051178738974632
+4.606223395648502,0.81,2.0,27.0,-0.0015546478307036028,0.0015530820068880113,-0.0029594838987596177,0.003339078871536082
+4.606223395648502,0.87,2.0,18.0,-0.0012994082397109429,0.001253231084714523,-0.0027060354162684965,0.00244096710775008
+4.606223395648502,0.93,2.0,23.0,-0.0013525680410032064,0.001074347582740813,-0.0028201958157992807,0.0020106456606270758
+4.606223395648502,0.99,2.0,10.0,-0.0012918228136819013,0.001058641575168171,-0.002634988456703251,0.002146793621924362
+5.851996519306452,0.21,2.0,8.0,-0.002265023749723719,0.0025798576356124737,-0.004250199372535318,0.00519705161951542
+5.851996519306452,0.27,2.0,24.0,-0.0013311756166813121,0.0013378473747782734,-0.002588631267444424,0.002590062678815728
+5.851996519306452,0.33,2.0,53.0,-0.0014420718420485132,0.0015404344396293967,-0.003003681284951605,0.0029051070536928823
+5.851996519306452,0.39,2.0,54.0,-0.0010714119330681002,0.0010917560757849887,-0.002334601183971058,0.0020680044886858717
+5.851996519306452,0.45,2.0,52.0,-0.0013544505731972081,0.0012164330309016747,-0.00270685558233877,0.002380171772793393
+5.851996519306452,0.51,2.0,46.0,-0.001610939656549177,0.0014456438196930174,-0.0030078016774859485,0.002888891010147279
+5.851996519306452,0.57,2.0,47.0,-0.0012050749426900469,0.0011789397134711213,-0.0022338458994976707,0.00239860068832475
+5.851996519306452,0.63,2.0,51.0,-0.001335503418083888,0.001204598968673889,-0.0025830932332693343,0.0023644217780429545
+5.851996519306452,0.69,2.0,43.0,-0.0011283766028977779,0.001217763565825567,-0.00221059496482225,0.0023310860337788473
+5.851996519306452,0.75,2.0,38.0,-0.0014880671042394457,0.0015957201549091058,-0.0028239844790151005,0.003354647814096937
+5.851996519306452,0.81,2.0,27.0,-0.002354289950772498,0.0023662515594181747,-0.0048154362313875335,0.0045203009771860045
+5.851996519306452,0.87,2.0,17.0,-0.0019009533435758457,0.0023112007624070206,-0.0036368657776356984,0.004666881955590552
+5.851996519306452,0.93,2.0,24.0,-0.0016094845278377854,0.0013016926744211133,-0.003344781464104963,0.002458128049020709
+5.851996519306452,0.99,2.0,16.0,-0.002044563897545991,0.0016986876943594798,-0.00407227139710246,0.0032281577130574843
+7.434694395049665,0.21,2.0,10.0,-0.0020906532493655044,0.002161566360234891,-0.0039133710626358936,0.004518108871273785
+7.434694395049665,0.27,2.0,22.0,-0.0015566622304000776,0.0016095647740633216,-0.0030391576988743458,0.0032322802376623105
+7.434694395049665,0.33,2.0,48.0,-0.001578773670688652,0.0017018009302852616,-0.0031029891747261285,0.003313661398174328
+7.434694395049665,0.39,2.0,55.0,-0.0014612701650035158,0.0014617540683343672,-0.0027290412362794853,0.0028697973396889223
+7.434694395049665,0.45,2.0,56.0,-0.0013500502394078924,0.0014588171084570119,-0.0025396458638019138,0.0028434497979707507
+7.434694395049665,0.51,2.0,45.0,-0.0016263085866713134,0.001682691496108719,-0.0030368578032768188,0.0032742761678125963
+7.434694395049665,0.57,2.0,50.0,-0.001320978855003313,0.0013450367475069524,-0.002573500703396086,0.0027119798183187385
+7.434694395049665,0.63,2.0,47.0,-0.001507324883260897,0.0015778619644226213,-0.003118656983186219,0.0029974259285460857
+7.434694395049665,0.69,2.0,41.0,-0.002057090179534431,0.0018700829324366415,-0.003976052727893433,0.0035525486556045533
+7.434694395049665,0.75,2.0,31.0,-0.002657374117871723,0.0024618226323704162,-0.00537737266022579,0.004989480886412475
+7.434694395049665,0.81,2.0,36.0,-0.003569581733492773,0.003653662604831638,-0.007371035966311583,0.007031428287467374
+7.434694395049665,0.87,2.0,17.0,-0.003601660316090118,0.004490517206047479,-0.00683642249255343,0.009574303494504659
+7.434694395049665,0.93,2.0,24.0,-0.0021871965019621873,0.0018513073327847162,-0.004495205241279331,0.003587648059950179
+7.434694395049665,0.99,2.0,18.0,-0.0024368461880253027,0.0024166135913909485,-0.004905619484515045,0.004879088295184132
+9.445439785451784,0.21,2.0,10.0,-0.0013966010039905665,0.0013347231410571448,-0.0026643604061257057,0.002612779679214538
+9.445439785451784,0.27,2.0,22.0,-0.0013155896422267662,0.001290615513489183,-0.0025825157362949387,0.0025509656593263094
+9.445439785451784,0.33,2.0,51.0,-0.0015320653838202115,0.0016414967124753798,-0.0030097952635115303,0.0032945204286326008
+9.445439785451784,0.39,2.0,59.0,-0.0015167151231435467,0.0014485075855893252,-0.0028993244121299075,0.002940492870378181
+9.445439785451784,0.45,2.0,55.0,-0.0016435299333749497,0.0016687811386818857,-0.0031674547387487094,0.0033957515640768167
+9.445439785451784,0.51,2.0,43.0,-0.002118748334229589,0.002133732861536354,-0.004209497703301144,0.004345161396187754
+9.445439785451784,0.57,2.0,53.0,-0.001563759743908879,0.001511734768092686,-0.0031027066909980762,0.002898105905342673
+9.445439785451784,0.63,2.0,46.0,-0.00254988428875577,0.0024796066827104243,-0.004926047601703806,0.004779969423586385
+9.445439785451784,0.69,2.0,34.0,-0.0040712962742179785,0.0031983092099030393,-0.008297166797672617,0.00608317150244303
+9.445439785451784,0.75,2.0,34.0,-0.0045766091251356064,0.0040173704670797205,-0.009009524534742209,0.007403247945478165
+9.445439785451784,0.81,2.0,29.0,-0.007120916773473349,0.00704249606124573,-0.014978384022357356,0.01326252978650704
+9.445439785451784,0.87,2.0,20.0,-0.004776176556060614,0.00742370175607383,-0.00849665252200414,0.01700244122035844
+9.445439785451784,0.93,2.0,20.0,-0.0030491741951737925,0.002415490091572382,-0.006321726257016381,0.0044278213333108635
+9.445439785451784,0.99,2.0,24.0,-0.0033316827219337167,0.003166540286292617,-0.006490960195469653,0.006465207609471434
+11.99999999999998,0.21,2.0,8.0,-0.004260326640328728,0.002671503743497664,-0.00946944342832022,0.004642482389007929
+11.99999999999998,0.27,2.0,24.0,-0.002345671580031537,0.0022320543476668517,-0.004728091705443303,0.004322199497421979
+11.99999999999998,0.33,2.0,55.0,-0.0020051053850031063,0.0018110179204085728,-0.0039003750371902346,0.003784730067919907
+11.99999999999998,0.39,2.0,56.0,-0.002423907154272764,0.0023124483618876964,-0.004580246040818312,0.004654953714269163
+11.99999999999998,0.45,2.0,58.0,-0.002706506738866088,0.0026791389211879763,-0.005108005687768726,0.005413460511562771
+11.99999999999998,0.51,2.0,55.0,-0.002427167422103561,0.0023901672146821673,-0.004708299437933261,0.00477813123176738
+11.99999999999998,0.57,2.0,52.0,-0.0031835579604377793,0.0030877982943113536,-0.006173994307602324,0.0061283987270611
+11.99999999999998,0.63,2.0,37.0,-0.004741365150088763,0.0040808933950552346,-0.009388604456117458,0.008053785933760335
+11.99999999999998,0.69,2.0,40.0,-0.007041285290543102,0.005547580383776432,-0.014031062897591602,0.010711387921999408
+11.99999999999998,0.75,2.0,27.0,-0.012057893342286461,0.010555334479789185,-0.02357759906520257,0.020616350885852303
+11.99999999999998,0.81,2.0,20.0,-0.014546005765182373,0.014633905986676752,-0.02782965878174534,0.028768711608480095
+11.99999999999998,0.87,2.0,20.0,-0.00647466757126571,0.01237834650062079,-0.011217035985715025,0.02845350125485016
+11.99999999999998,0.93,2.0,18.0,-0.0041844600446628065,0.0036754728992189033,-0.008679189281057053,0.006939180467794353
+11.99999999999998,0.99,2.0,27.0,-0.00419420071699596,0.00397573814270377,-0.007677787336587695,0.008364159673603272
+0.0999999999999749,0.27,3.0,21.0,-2.0856140441774307e-05,1.9219025447200818e-05,-4.251092964839089e-05,3.6137753347988446e-05
+0.0999999999999749,0.33,3.0,18.0,-1.356690532789041e-05,1.4550813256535556e-05,-2.7093163051213667e-05,2.7641116411466843e-05
+0.0999999999999749,0.39,3.0,42.0,-9.585754502697855e-06,9.686685023917175e-06,-1.8980407199634303e-05,1.8667555311982727e-05
+0.0999999999999749,0.45,3.0,40.0,-1.042962079760858e-05,8.33838924562531e-06,-2.1514593916971966e-05,1.5482743114982108e-05
+0.0999999999999749,0.51,3.0,49.0,-7.563945855534819e-06,7.040499854044785e-06,-1.5770499972698086e-05,1.271188013080634e-05
+0.0999999999999749,0.57,3.0,51.0,-5.389671341054439e-06,4.900676363762806e-06,-1.0833019169942707e-05,9.369852031255799e-06
+0.0999999999999749,0.63,3.0,46.0,-4.615980656503093e-06,4.041059764970586e-06,-8.762774475683074e-06,8.099507572152804e-06
+0.0999999999999749,0.69,3.0,47.0,-5.6310638167719395e-06,9.747498911275918e-06,-9.85610952868519e-06,2.2750123978272104e-05
+0.0999999999999749,0.75,3.0,49.0,-9.060746399544944e-06,1.2307371920601371e-05,-1.683423265597764e-05,2.6911048797340013e-05
+0.0999999999999749,0.81,3.0,37.0,-1.3034965708121323e-05,1.677803343438943e-05,-2.329045210840993e-05,3.5348249518988304e-05
+0.0999999999999749,0.87,3.0,25.0,-2.4116225995873607e-05,2.2198338614789074e-05,-4.732910011464703e-05,4.69300415380064e-05
+0.0999999999999749,0.93,3.0,40.0,-4.624595074927328e-07,4.0238627634031077e-07,-9.312888847563502e-07,8.023333872251881e-07
+0.0999999999999749,0.99,3.0,34.0,-1.8084798128327142e-07,1.4829209253120298e-07,-3.4518198351281944e-07,2.932935876455401e-07
+0.1270454343320595,0.27,3.0,21.0,-2.931661364518603e-05,2.492163139217671e-05,-5.6800496624830105e-05,4.810313909792542e-05
+0.1270454343320595,0.33,3.0,18.0,-1.8823376716607618e-05,1.89635944365805e-05,-3.5714642409391915e-05,3.7595013427798405e-05
+0.1270454343320595,0.39,3.0,42.0,-1.3176048973609226e-05,1.2504726452737718e-05,-2.5403412813998585e-05,2.458821919643282e-05
+0.1270454343320595,0.45,3.0,40.0,-1.3125505423240592e-05,1.1316987911319288e-05,-2.8262565344688654e-05,2.1024734136960195e-05
+0.1270454343320595,0.51,3.0,49.0,-1.042355565032139e-05,9.018971985881964e-06,-2.1750055079256524e-05,1.6677179389475727e-05
+0.1270454343320595,0.57,3.0,51.0,-7.453765504530108e-06,6.276200400139357e-06,-1.4851935182390148e-05,1.2267091067634978e-05
+0.1270454343320595,0.63,3.0,46.0,-5.383304643156025e-06,5.098046249479686e-06,-1.0740794028703476e-05,9.637810988476143e-06
+0.1270454343320595,0.69,3.0,47.0,-5.953993630486766e-06,8.981835693513418e-06,-9.958577968179852e-06,2.203966176448028e-05
+0.1270454343320595,0.75,3.0,49.0,-9.578105015274988e-06,1.2516535650904884e-05,-1.657288160404001e-05,2.7500516691381715e-05
+0.1270454343320595,0.81,3.0,37.0,-1.3343311664696615e-05,1.652161485395508e-05,-2.3977561314312973e-05,3.5796921537866064e-05
+0.1270454343320595,0.87,3.0,25.0,-2.326131359028507e-05,2.2906710179726655e-05,-4.803228210586593e-05,4.657985488593069e-05
+0.1270454343320595,0.93,3.0,40.0,-6.405025109853846e-07,5.921664277152174e-07,-1.3446792120355106e-06,1.0971515590822924e-06
+0.1270454343320595,0.99,3.0,34.0,-2.3478266039740348e-07,2.0625557676057345e-07,-4.7299740440688235e-07,4.03440149447407e-07
+0.1614054238462204,0.27,3.0,21.0,-4.228697484180607e-05,3.7426869789001284e-05,-8.302807877881198e-05,7.306689411129421e-05
+0.1614054238462204,0.33,3.0,18.0,-2.7082169592236958e-05,2.7751903482466293e-05,-5.29025787556441e-05,5.251586316003794e-05
+0.1614054238462204,0.39,3.0,42.0,-1.9533468430852014e-05,1.7691927842636524e-05,-3.807864587785307e-05,3.443236825365748e-05
+0.1614054238462204,0.45,3.0,40.0,-1.94697226696722e-05,1.6377148763354536e-05,-3.9722153546330554e-05,2.9913831737589416e-05
+0.1614054238462204,0.51,3.0,49.0,-1.621511616088064e-05,1.2900361496188337e-05,-3.3508132054200574e-05,2.3844207669753414e-05
+0.1614054238462204,0.57,3.0,51.0,-1.0197135458911224e-05,9.645790195867771e-06,-2.094020323887493e-05,1.801976041167313e-05
+0.1614054238462204,0.63,3.0,46.0,-7.400707771191535e-06,6.844423641017224e-06,-1.5224860340189148e-05,1.305978837509376e-05
+0.1614054238462204,0.69,3.0,47.0,-5.954057525379936e-06,9.340856011744319e-06,-1.0834152329635368e-05,2.0239608761584132e-05
+0.1614054238462204,0.75,3.0,49.0,-9.346003296335232e-06,1.2502503758353108e-05,-1.6954629927559063e-05,2.6556043271957443e-05
+0.1614054238462204,0.81,3.0,37.0,-1.2745940523194791e-05,1.7380956749130624e-05,-2.3211645649758414e-05,3.672746208505764e-05
+0.1614054238462204,0.87,3.0,25.0,-2.3035492303617034e-05,2.4343643752324492e-05,-4.7111707220187926e-05,4.800144212262961e-05
+0.1614054238462204,0.93,3.0,40.0,-8.780054527312427e-07,7.748087764802801e-07,-1.728702871291956e-06,1.4841715907643822e-06
+0.1614054238462204,0.99,3.0,34.0,-2.8282877662811093e-07,2.759444600582544e-07,-5.704353338800835e-07,5.43625756399351e-07
+0.2050582217609579,0.27,3.0,21.0,-6.775092946616584e-05,6.149698303869131e-05,-0.0001313020411637332,0.0001217465396931038
+0.2050582217609579,0.33,3.0,18.0,-4.418092382192577e-05,4.6367681742701095e-05,-9.061757709261935e-05,8.894827550903623e-05
+0.2050582217609579,0.39,3.0,42.0,-3.2896523210658235e-05,3.143364633052993e-05,-6.484758420876219e-05,6.032383528722519e-05
+0.2050582217609579,0.45,3.0,40.0,-3.150007843792715e-05,2.842370962057272e-05,-6.658406116090728e-05,5.0738103359552045e-05
+0.2050582217609579,0.51,3.0,49.0,-2.6612870537534564e-05,2.2170337653475095e-05,-5.66631898839415e-05,4.056604808501808e-05
+0.2050582217609579,0.57,3.0,50.0,-1.8033362855980456e-05,1.610456134753222e-05,-3.5820184581059136e-05,3.030821308134893e-05
+0.2050582217609579,0.63,3.0,47.0,-1.2093945349752854e-05,1.0904029642201724e-05,-2.395374479830387e-05,2.1121756880269596e-05
+0.2050582217609579,0.69,3.0,46.0,-7.83362448538509e-06,9.866844746117107e-06,-1.4552575743238602e-05,2.1333088782630438e-05
+0.2050582217609579,0.75,3.0,50.0,-1.1000835025741218e-05,1.3556675018258932e-05,-2.047382390321351e-05,2.9992287143977788e-05
+0.2050582217609579,0.81,3.0,37.0,-1.4522126821553594e-05,1.8774945169665397e-05,-2.706006967893947e-05,3.8725150569354774e-05
+0.2050582217609579,0.87,3.0,24.0,-2.7500979985991354e-05,2.6253758156410344e-05,-5.4764419363536606e-05,5.305511047308971e-05
+0.2050582217609579,0.93,3.0,41.0,-1.3286396772549276e-06,1.1058752659617714e-06,-2.618528213644588e-06,2.175910172337139e-06
+0.2050582217609579,0.99,3.0,34.0,-4.340732911997843e-07,4.5169530913420997e-07,-8.748184819596123e-07,8.390768797412911e-07
+0.2605171084697316,0.27,3.0,21.0,-0.00011853622136999234,0.0001102887172242268,-0.00025126043660376985,0.00020843738191433518
+0.2605171084697316,0.33,3.0,18.0,-8.409651238975141e-05,8.901632978901766e-05,-0.00017058992217845736,0.0001690075766701103
+0.2605171084697316,0.39,3.0,43.0,-6.13884238963926e-05,5.647181593912546e-05,-0.00012048499231124982,0.00010649765252458029
+0.2605171084697316,0.45,3.0,39.0,-6.327442491970442e-05,5.0857173119416187e-05,-0.00012820986333226555,9.809832863109461e-05
+0.2605171084697316,0.51,3.0,49.0,-5.076690816449887e-05,3.967972812298675e-05,-0.00010223555089235911,7.682891417609172e-05
+0.2605171084697316,0.57,3.0,51.0,-3.260125579691532e-05,2.8809692916600896e-05,-6.628663017738485e-05,5.451750408739902e-05
+0.2605171084697316,0.63,3.0,45.0,-2.6813809188274775e-05,2.217510353413486e-05,-5.67073827157304e-05,4.236755796351658e-05
+0.2605171084697316,0.69,3.0,47.0,-1.4876560363268048e-05,1.5250885552969538e-05,-2.910821040313818e-05,2.9879354610286586e-05
+0.2605171084697316,0.75,3.0,49.0,-1.4934921574120648e-05,1.9080855257898377e-05,-2.8145366142349694e-05,3.9355087880161676e-05
+0.2605171084697316,0.81,3.0,38.0,-2.1027574359927143e-05,2.5892437142179882e-05,-3.865480397406991e-05,5.514324998180501e-05
+0.2605171084697316,0.87,3.0,24.0,-3.981915588789903e-05,3.462157882991145e-05,-7.331137407077364e-05,7.286126859363623e-05
+0.2605171084697316,0.93,3.0,40.0,-2.3877337029266995e-06,2.1298969376363538e-06,-4.9230325937221965e-06,3.986210335396747e-06
+0.2605171084697316,0.99,3.0,35.0,-2.300102180788062e-06,1.2890121908255582e-06,-5.27615764003721e-06,2.2308038890465317e-06
+0.3309750919646482,0.27,3.0,21.0,-0.00019435715903671843,0.00017540992372748034,-0.0003807771389311742,0.000339829039593272
+0.3309750919646482,0.33,3.0,19.0,-0.00014788189902906773,0.0001585529836223856,-0.0002968539372165288,0.0003073812611452056
+0.3309750919646482,0.39,3.0,42.0,-0.00010700893399791933,9.71023089430131e-05,-0.0002127228031428099,0.00018315327426957686
+0.3309750919646482,0.45,3.0,38.0,-0.00011765386073235505,9.042902423145106e-05,-0.00024544571571579523,0.00017024164700973527
+0.3309750919646482,0.51,3.0,49.0,-8.877194154232346e-05,6.900042544639182e-05,-0.00018370099370900142,0.00012978497446539502
+0.3309750919646482,0.57,3.0,53.0,-5.927865792349373e-05,4.784157418030619e-05,-0.00011371163410161502,9.76951207416116e-05
+0.3309750919646482,0.63,3.0,44.0,-5.0527269756496924e-05,4.013956308614411e-05,-0.00010313831074074179,7.139580729634984e-05
+0.3309750919646482,0.69,3.0,45.0,-2.6263455277879283e-05,2.0740488132569763e-05,-5.2331853232289026e-05,3.9915744552144236e-05
+0.3309750919646482,0.75,3.0,51.0,-2.3591297324658527e-05,2.3804226393431353e-05,-4.521134140763452e-05,4.681314584179283e-05
+0.3309750919646482,0.81,3.0,38.0,-2.546288331333281e-05,3.2775054970976187e-05,-4.9281433186294986e-05,6.633103137752926e-05
+0.3309750919646482,0.87,3.0,24.0,-4.573594681058427e-05,4.654511363903382e-05,-8.925207929377424e-05,9.012944677103936e-05
+0.3309750919646482,0.93,3.0,39.0,-4.940297919462844e-06,4.242296606039832e-06,-1.0619938357087944e-05,7.849543989980568e-06
+0.3309750919646482,0.99,3.0,36.0,-4.967885432086393e-06,2.460261889537933e-06,-1.176296022340652e-05,4.176015199763803e-06
+0.4204887431175071,0.27,3.0,21.0,-0.00030027118479222407,0.00029214770548897787,-0.0006076981422347942,0.0005553149162381752
+0.4204887431175071,0.33,3.0,19.0,-0.00029006555144500267,0.00029002189032764815,-0.0005292710661451034,0.000571310042988742
+0.4204887431175071,0.39,3.0,42.0,-0.00017849953004939537,0.0001677501733908685,-0.00036421247582257897,0.0003276618567876181
+0.4204887431175071,0.45,3.0,38.0,-0.00019236665582099427,0.000160610671068591,-0.00040503680414091337,0.0003027268388121993
+0.4204887431175071,0.51,3.0,50.0,-0.00014668821782555055,0.00011812779877568015,-0.00030715715429993206,0.0002232741556551618
+0.4204887431175071,0.57,3.0,53.0,-9.746641066916032e-05,8.548508431304507e-05,-0.00019478753668127223,0.00016575050398449448
+0.4204887431175071,0.63,3.0,42.0,-9.06372639259434e-05,6.915557268911064e-05,-0.00018550549341842063,0.00013206867040063848
+0.4204887431175071,0.69,3.0,46.0,-4.218824711150398e-05,3.1889839238761235e-05,-8.183292136015297e-05,6.490126674933633e-05
+0.4204887431175071,0.75,3.0,51.0,-3.2750143408599174e-05,3.36567969410858e-05,-6.929453587462376e-05,6.426892762544815e-05
+0.4204887431175071,0.81,3.0,38.0,-3.380023007775605e-05,4.008130460483713e-05,-6.422729928685027e-05,8.046203710594924e-05
+0.4204887431175071,0.87,3.0,24.0,-5.4763240431744e-05,5.543784325051009e-05,-0.00010539781117957038,0.00010922973097893039
+0.4204887431175071,0.93,3.0,39.0,-8.646485124132399e-06,6.968637845249483e-06,-1.711774104331492e-05,1.3663604685689527e-05
+0.4204887431175071,0.99,3.0,36.0,-8.109565342261381e-06,3.912176290205535e-06,-1.795499984046743e-05,6.7456804167162965e-06
+0.5342117500109386,0.27,3.0,21.0,-0.0005018639404720541,0.000489265580007648,-0.0009932849199707715,0.000938449417308108
+0.5342117500109386,0.33,3.0,18.0,-0.0004797375559519943,0.0005239574629480871,-0.0009418092779995397,0.001068432295481521
+0.5342117500109386,0.39,3.0,41.0,-0.00030960883053640767,0.0002734818125208453,-0.000593660733080904,0.0005457169822816018
+0.5342117500109386,0.45,3.0,41.0,-0.0003219161782772774,0.00027042892747555135,-0.0006695223121075293,0.0005298417072246298
+0.5342117500109386,0.51,3.0,49.0,-0.0002482251262296407,0.0002078977116918361,-0.000543249331019299,0.0003740917358569433
+0.5342117500109386,0.57,3.0,51.0,-0.00016783802371537552,0.00015077520470031897,-0.00034453773320279103,0.00028393485253409357
+0.5342117500109386,0.63,3.0,44.0,-0.00014361851392610033,0.00011398802062557226,-0.0002859698843072981,0.0002177761746748311
+0.5342117500109386,0.69,3.0,45.0,-6.885677562679075e-05,5.1864160530436366e-05,-0.00013699965892257187,0.00010289954824573897
+0.5342117500109386,0.75,3.0,52.0,-5.5291432176152764e-05,4.4581863694404284e-05,-0.00010576871288660142,8.948407057083126e-05
+0.5342117500109386,0.81,3.0,38.0,-4.3992759126044504e-05,5.208962077938072e-05,-8.279681276204359e-05,0.00010170827404873106
+0.5342117500109386,0.87,3.0,24.0,-6.597256698366436e-05,6.952308649370305e-05,-0.00013197034158887394,0.00013441303035430642
+0.5342117500109386,0.93,3.0,39.0,-1.483103527165539e-05,1.2120331045999623e-05,-3.0511204043985534e-05,2.3593142004013186e-05
+0.5342117500109386,0.99,3.0,36.0,-1.2722843526394787e-05,6.741708803853166e-06,-3.146733001432177e-05,1.1313070898678325e-05
+0.6786916380543286,0.27,3.0,21.0,-0.0007836058627280135,0.0007607149227493964,-0.0015107898763840103,0.0014848892398107143
+0.6786916380543286,0.33,3.0,18.0,-0.0008076615391459606,0.0008473902764589284,-0.0015325096246628896,0.0017777808572240735
+0.6786916380543286,0.39,3.0,41.0,-0.00048100202149501883,0.0004452268767085439,-0.0009503199846887378,0.0008597525231387134
+0.6786916380543286,0.45,3.0,41.0,-0.0005061755546569822,0.00046018468093210165,-0.0010606072629232354,0.0008499455335430686
+0.6786916380543286,0.51,3.0,47.0,-0.00031397144632217043,0.0002743240410356137,-0.0006405558324611075,0.0005233344198229542
+0.6786916380543286,0.57,3.0,53.0,-0.0003771364852336363,0.0002854017318621383,-0.0007529144050910183,0.0005380311599594848
+0.6786916380543286,0.63,3.0,44.0,-0.00022917914865151274,0.0001788545402808416,-0.0004827169337549591,0.0003485786315826075
+0.6786916380543286,0.69,3.0,45.0,-0.00010751601082390698,8.483242698471589e-05,-0.00021687470059374874,0.0001589126319393748
+0.6786916380543286,0.75,3.0,52.0,-8.463945426911122e-05,6.90333358963539e-05,-0.00017945639635774248,0.000130427846149937
+0.6786916380543286,0.81,3.0,38.0,-5.9344200100473395e-05,6.722103361833603e-05,-0.00011581191734638559,0.00013263481363467102
+0.6786916380543286,0.87,3.0,23.0,-8.19417697767501e-05,8.863492559382772e-05,-0.00016346605339759914,0.00017125420566950082
+0.6786916380543286,0.93,3.0,40.0,-2.5326376470114066e-05,2.0952236959245305e-05,-5.209583789840342e-05,4.080656503196296e-05
+0.6786916380543286,0.99,3.0,36.0,-2.286298808539559e-05,1.2096936332992129e-05,-5.25421631574218e-05,2.117330870899791e-05
+0.8622467393414373,0.27,3.0,20.0,-0.0012136078163049976,0.0011793450109668982,-0.00232249678064042,0.002353040968879117
+0.8622467393414373,0.33,3.0,18.0,-0.0011834846214334109,0.0013069323084859779,-0.0023584932405703966,0.002690377905333965
+0.8622467393414373,0.39,3.0,41.0,-0.0007861064570466538,0.0006958140763972954,-0.0015606337450686503,0.001348945749100369
+0.8622467393414373,0.45,3.0,42.0,-0.0007726406489003472,0.0007445124781774893,-0.0015846138515384879,0.0014044539585003953
+0.8622467393414373,0.51,3.0,47.0,-0.0005243728959517855,0.00044434986002303773,-0.0010489599542359293,0.0008533121818581495
+0.8622467393414373,0.57,3.0,53.0,-0.0005865047226939832,0.00045257436148935204,-0.0012480749777962167,0.00086319262332473
+0.8622467393414373,0.63,3.0,44.0,-0.0003886073940607865,0.0002872699905610414,-0.0007692305579463941,0.0005711648383286376
+0.8622467393414373,0.69,3.0,45.0,-0.0001699723820544011,0.00014157290204642743,-0.00035893713212968185,0.00025929060720077075
+0.8622467393414373,0.75,3.0,53.0,-0.0001387076325383216,0.00010907721713225066,-0.00028323792576193205,0.00020534448837859163
+0.8622467393414373,0.81,3.0,36.0,-9.447696013559095e-05,9.524592194948151e-05,-0.00018237705787801676,0.00018314471331650487
+0.8622467393414373,0.87,3.0,24.0,-0.00010683959676819915,0.00010828855673763114,-0.00020126911265654838,0.00022045774019292667
+0.8622467393414373,0.93,3.0,39.0,-4.265617095191652e-05,3.666155166799631e-05,-9.543152185194305e-05,6.900086597017569e-05
+0.8622467393414373,0.99,3.0,37.0,-3.846507941545951e-05,2.2591454537669308e-05,-8.937911228252217e-05,4.058797110834019e-05
+1.0954451150103528,0.27,3.0,20.0,-0.0017697847480880582,0.0017273623827265825,-0.0035022662642911575,0.003316612291408912
+1.0954451150103528,0.33,3.0,18.0,-0.0017162327897888318,0.0019063832528427185,-0.00337719350632884,0.003744021409718877
+1.0954451150103528,0.39,3.0,41.0,-0.0011892045881799684,0.0010816095593638917,-0.002292821251284761,0.002197409361454886
+1.0954451150103528,0.45,3.0,42.0,-0.001235229838884526,0.0011621750028242427,-0.0025480789874871997,0.0021265160822589516
+1.0954451150103528,0.51,3.0,46.0,-0.0008786851065177637,0.0007367505512355021,-0.0017742314142789285,0.0014131402245491623
+1.0954451150103528,0.57,3.0,54.0,-0.0009287459492809578,0.0007428171798826146,-0.0019097770622430975,0.0013880738908588356
+1.0954451150103528,0.63,3.0,45.0,-0.0005758829083180824,0.0005128592009794914,-0.0012417034694048854,0.0009342057947794889
+1.0954451150103528,0.69,3.0,44.0,-0.0003020700496946843,0.0002289850457968904,-0.0006341640280922812,0.00042680244977440657
+1.0954451150103528,0.75,3.0,53.0,-0.00022494177046104735,0.00018924106781178422,-0.00046478194659342777,0.0003485630317953313
+1.0954451150103528,0.81,3.0,36.0,-0.00015588334546600278,0.00014617535126493363,-0.00030791739707393254,0.0002853072926541421
+1.0954451150103528,0.87,3.0,24.0,-0.00015173929489519932,0.0001493850512596948,-0.00029735834301667844,0.0002986782459256128
+1.0954451150103528,0.93,3.0,38.0,-7.600247867395401e-05,6.28332166611272e-05,-0.00015994722408835908,0.00011527097460575551
+1.0954451150103528,0.99,3.0,38.0,-5.883887590280601e-05,3.1343427026778516e-05,-0.00014726417900685573,5.5844870089261595e-05
+1.3917130042341792,0.27,3.0,19.0,-0.0022616703448857583,0.0023254201956155866,-0.004379220100519774,0.004462466937380675
+1.3917130042341792,0.33,3.0,20.0,-0.0022567742708187954,0.002227548216247546,-0.004323893334608837,0.004578048957371751
+1.3917130042341792,0.39,3.0,40.0,-0.0016569199715486434,0.0016492176074067734,-0.0034880857917484447,0.003077909271589549
+1.3917130042341792,0.45,3.0,42.0,-0.001687364372258921,0.001532715051291792,-0.0035909947152137586,0.0028655277795966716
+1.3917130042341792,0.51,3.0,47.0,-0.0017219151779296615,0.0013744868339740834,-0.00344928408149637,0.0026874453546052754
+1.3917130042341792,0.57,3.0,53.0,-0.0010152055561379672,0.0009077474753854413,-0.002027545824604539,0.00177073610442776
+1.3917130042341792,0.63,3.0,45.0,-0.0009040102049757297,0.0007762908506787165,-0.0018657069100019622,0.0014793100544597928
+1.3917130042341792,0.69,3.0,43.0,-0.00047323636682080293,0.00037758555319671847,-0.0009662350341461562,0.0007113363319884616
+1.3917130042341792,0.75,3.0,52.0,-0.0003743181239015736,0.0002908205583229373,-0.0007387468990739561,0.0005685436564819839
+1.3917130042341792,0.81,3.0,38.0,-0.00024914658200619677,0.0002151513535617793,-0.0005161654870008873,0.00041546869710729615
+1.3917130042341792,0.87,3.0,24.0,-0.00023210241785243636,0.0001932641354067749,-0.0004538449297148876,0.00038021797382727367
+1.3917130042341792,0.93,3.0,36.0,-0.00014326131189243844,0.00011027256084495472,-0.00029957709636045714,0.00020766359200829126
+1.3917130042341792,0.99,3.0,39.0,-9.795596625859268e-05,5.8842248589035556e-05,-0.00022315313034754227,0.00010463817074326539
+1.7681078308849854,0.27,3.0,18.0,-0.002146389463937258,0.0024665913676807736,-0.004329594367078629,0.004732198798295026
+1.7681078308849854,0.33,3.0,21.0,-0.0023143042711090836,0.0025403366698504093,-0.004507455094225137,0.005118337509434919
+1.7681078308849854,0.39,3.0,38.0,-0.0021641623040136626,0.00199385599418692,-0.004170284452074804,0.0040381654053323595
+1.7681078308849854,0.45,3.0,42.0,-0.0021463119905007553,0.0018494793382568364,-0.004388820063096129,0.0036172494620379247
+1.7681078308849854,0.51,3.0,48.0,-0.0020996938943611144,0.001906497563327405,-0.0042278885995503035,0.0036315113392856035
+1.7681078308849854,0.57,3.0,54.0,-0.0013717878763142603,0.0012954293806331457,-0.0028024971122257813,0.002408802082511532
+1.7681078308849854,0.63,3.0,44.0,-0.001154602580336964,0.001001803411491994,-0.0022166482031669437,0.0018590339700647923
+1.7681078308849854,0.69,3.0,43.0,-0.0006357181044671328,0.0005409121186773851,-0.0012873731672015931,0.0010013647646245393
+1.7681078308849854,0.75,3.0,51.0,-0.0005331674964194551,0.00044645636058188425,-0.001157394761598065,0.0008202659568188332
+1.7681078308849854,0.81,3.0,39.0,-0.00040799988344935077,0.0003329267029347926,-0.0008122394132162472,0.0006353694832458495
+1.7681078308849854,0.87,3.0,24.0,-0.00035878288972032544,0.0002924514652587098,-0.0007389343344694396,0.000552096015210303
+1.7681078308849854,0.93,3.0,36.0,-0.0002190268349082563,0.00016671632822034044,-0.0004586657098379745,0.0003114266115999429
+1.7681078308849854,0.99,3.0,37.0,-0.00016976478977185556,0.00010948171791158611,-0.000394823878582382,0.00019602879131893312
+2.2463002732068973,0.27,3.0,18.0,-0.001582619430610004,0.0018385560942095678,-0.0029050688883169844,0.0038558117368453497
+2.2463002732068973,0.33,3.0,20.0,-0.002477526218132104,0.0026253255018712524,-0.0047441993733089395,0.005333502716353085
+2.2463002732068973,0.39,3.0,38.0,-0.0021299829140501952,0.0018943550266243801,-0.004099454675186921,0.0038505463287500513
+2.2463002732068973,0.45,3.0,44.0,-0.0022013940474663375,0.0020951443678783694,-0.00445924253402147,0.004013472301190518
+2.2463002732068973,0.51,3.0,48.0,-0.002331645087479418,0.0021991750479302317,-0.004632138933530065,0.004150186641201812
+2.2463002732068973,0.57,3.0,51.0,-0.001609055904888891,0.0015005413934249278,-0.0031662219286555954,0.00295357532851392
+2.2463002732068973,0.63,3.0,42.0,-0.0015460614988949248,0.0014456401937099567,-0.003212545959218671,0.0027421742138538947
+2.2463002732068973,0.69,3.0,46.0,-0.0008081995305101265,0.0007390947716651323,-0.0016228554502561846,0.001437389249600147
+2.2463002732068973,0.75,3.0,49.0,-0.0007374018549654949,0.0005938201984271799,-0.0015094120544268555,0.0011246248099727534
+2.2463002732068973,0.81,3.0,44.0,-0.0004989341168340542,0.00045340782294298174,-0.001077505833051106,0.0008456432901720363
+2.2463002732068973,0.87,3.0,31.0,-0.0004511584156783047,0.00038652417801511666,-0.0009470081292536238,0.0007285012558052614
+2.2463002732068973,0.93,3.0,27.0,-0.0002864146557573076,0.00022829956751985078,-0.000631104209646696,0.0004097520732655731
+2.2463002732068973,0.99,3.0,35.0,-0.000271124481060114,0.00015497992831192692,-0.0006215603272525763,0.00028288671942250094
+2.2463002732068973,1.05,3.0,5.0,-8.876371093897717e-05,5.8066703827376103e-05,-0.00016949996239223886,0.00010164396361198592
+2.853821938497904,0.21,3.0,5.0,-0.002461385799940885,0.003889332445062843,-0.003775573388579434,0.008991388082920748
+2.853821938497904,0.27,3.0,15.0,-0.001624234726370593,0.0017154325606822621,-0.0030794623147012367,0.0034014058550206937
+2.853821938497904,0.33,3.0,21.0,-0.0017758961153665454,0.001963625953555346,-0.003587835113946826,0.003787928178650627
+2.853821938497904,0.39,3.0,37.0,-0.001682368162252259,0.0015712676794204183,-0.0033261043645570563,0.0031681117673352335
+2.853821938497904,0.45,3.0,46.0,-0.0018666911129982613,0.0019445667155720992,-0.0037524908024263864,0.003689520414784953
+2.853821938497904,0.51,3.0,42.0,-0.002157219752586434,0.0021519715820305656,-0.004460397819655638,0.003994495140310388
+2.853821938497904,0.57,3.0,51.0,-0.0016202076194782836,0.0016566098828406969,-0.0031963980249267803,0.0033102822903812636
+2.853821938497904,0.63,3.0,46.0,-0.0016426445788204382,0.0015225878029683654,-0.0032849633639407657,0.0029690149586895985
+2.853821938497904,0.69,3.0,46.0,-0.0010891359039593921,0.0009972452729829612,-0.002155920598825199,0.0020141934253306536
+2.853821938497904,0.75,3.0,48.0,-0.0007679801184375511,0.000725060222077442,-0.0016301223278567915,0.001358457452773725
+2.853821938497904,0.81,3.0,45.0,-0.0006832026870365816,0.0006505476886212837,-0.001456737380425074,0.0012450051865139577
+2.853821938497904,0.87,3.0,40.0,-0.000491646331573022,0.000356153450633656,-0.0010683147580253535,0.0006438669349386761
+2.853821938497904,0.93,3.0,18.0,-0.0008065153440635295,0.0005230433360516078,-0.0016222123613433767,0.0009620840090013907
+2.853821938497904,0.99,3.0,30.0,-0.00021210432429627014,0.0002038668308481769,-0.0004426448517817289,0.00037258671092307014
+2.853821938497904,1.05,3.0,10.0,-7.583634120945178e-05,9.671710343677571e-05,-0.0001453108253064328,0.00019237176851922557
+3.625650476828125,0.21,3.0,5.0,-0.002740917173701018,0.0031691201451697023,-0.005367186600481299,0.006252054070043167
+3.625650476828125,0.27,3.0,13.0,-0.0016852540916175143,0.0020333147939969633,-0.0031950357321520193,0.004247483866892715
+3.625650476828125,0.33,3.0,29.0,-0.0015198076121728471,0.001490015209254712,-0.002989950656660116,0.002882340073618016
+3.625650476828125,0.39,3.0,37.0,-0.0015235134138109486,0.0014250348142956935,-0.0027498977433999404,0.002937492662097351
+3.625650476828125,0.45,3.0,36.0,-0.0017231870175312158,0.001640530669554217,-0.0034013961174517047,0.0031932541041499196
+3.625650476828125,0.51,3.0,52.0,-0.0018550782139637944,0.001983343714806824,-0.0037883328107819847,0.0037021459850704124
+3.625650476828125,0.57,3.0,50.0,-0.0017762093473030645,0.001739501872129859,-0.0038042632315306063,0.0032544979563243624
+3.625650476828125,0.63,3.0,33.0,-0.002271964850489685,0.002123977093429366,-0.004570705134719193,0.0042425652016204
+3.625650476828125,0.69,3.0,47.0,-0.0016162666277009913,0.0015985194902998789,-0.003235016437709409,0.003170573228850588
+3.625650476828125,0.75,3.0,47.0,-0.001510219787258943,0.0014674639298036451,-0.0029701600723662782,0.002850832351734857
+3.625650476828125,0.81,3.0,55.0,-0.0010808733532754681,0.0010633272732278824,-0.0021534576208090865,0.0020660816760304213
+3.625650476828125,0.87,3.0,37.0,-0.0008624966047965984,0.0006446841238112238,-0.0017877812145075695,0.001176962170317133
+3.625650476828125,0.93,3.0,19.0,-0.0008675055349844759,0.0007321964046207828,-0.0018352915303387555,0.0013730603864272354
+3.625650476828125,0.99,3.0,26.0,-0.0004089095161217685,0.0003385701709685155,-0.0007748291350260383,0.0006749525870250795
+3.625650476828125,1.05,3.0,14.0,-0.00015037161998287447,0.00018834010802657987,-0.0002927266986919936,0.0003533399684254729
+4.606223395648529,0.21,3.0,6.0,-0.003017279956743076,0.0031317258640097636,-0.00558439991173985,0.006252468220743879
+4.606223395648529,0.27,3.0,12.0,-0.0016869145620318216,0.0023879827681254967,-0.0031927615338856272,0.004761403437074398
+4.606223395648529,0.33,3.0,33.0,-0.0015482063958485908,0.001370354909902161,-0.0029678759806224444,0.002743454056418552
+4.606223395648529,0.39,3.0,29.0,-0.0017193605370781524,0.0016955664612046042,-0.003251614205119705,0.003522640733597935
+4.606223395648529,0.45,3.0,50.0,-0.0013773803060106971,0.0013726998230401764,-0.002699092935096804,0.0027327187635438305
+4.606223395648529,0.51,3.0,39.0,-0.0023301595870115965,0.002075039156060528,-0.004366102173927913,0.004068647426166928
+4.606223395648529,0.57,3.0,45.0,-0.0020671014964369454,0.0018872187467012045,-0.0040147915555749595,0.003659349472342003
+4.606223395648529,0.63,3.0,39.0,-0.002473260227455844,0.0021547216940184903,-0.004975919850576733,0.004032939242712541
+4.606223395648529,0.69,3.0,50.0,-0.0020604090684638926,0.0022026676908299347,-0.004049594854158584,0.0043332324176548745
+4.606223395648529,0.75,3.0,44.0,-0.002088536685109983,0.0020843421249979073,-0.004217593968811828,0.004090291110230979
+4.606223395648529,0.81,3.0,57.0,-0.0016076704452141247,0.0015966616545443461,-0.0031391256055210786,0.003191607629345698
+4.606223395648529,0.87,3.0,37.0,-0.001545069730462124,0.001299147588781692,-0.0031515015844424837,0.002473081119808098
+4.606223395648529,0.93,3.0,18.0,-0.0012540635520090842,0.0011772389053433929,-0.0023999652562046725,0.0022290897745762925
+4.606223395648529,0.99,3.0,22.0,-0.0006743816079774696,0.0006297114906853638,-0.0014490078166808848,0.0011787528039616396
+4.606223395648529,1.05,3.0,19.0,-0.00040098288417844414,0.00033479647549076796,-0.0008261514750163705,0.0006560183411393345
+5.851996519306413,0.27,3.0,6.0,-0.0029484132725915435,0.0024544941057974934,-0.005806529455642065,0.004601772620809666
+5.851996519306413,0.33,3.0,28.0,-0.0012167485935924672,0.0012994880507125482,-0.0022987166963903062,0.002630055026879419
+5.851996519306413,0.39,3.0,30.0,-0.001145732872828859,0.0011033095043497016,-0.0022167724868632824,0.0022504907309448853
+5.851996519306413,0.45,3.0,36.0,-0.001565466953968295,0.0016289921584787454,-0.002972171069358451,0.003167978331246151
+5.851996519306413,0.51,3.0,59.0,-0.0012738003648929436,0.0013019286859325529,-0.002474516485337798,0.0025892413132533767
+5.851996519306413,0.57,3.0,47.0,-0.0017769636334278396,0.001601928375092924,-0.003482412892040534,0.0031725407458395153
+5.851996519306413,0.63,3.0,48.0,-0.0014378434164332003,0.001448965097228067,-0.0028006327027672463,0.0028374436598766813
+5.851996519306413,0.69,3.0,54.0,-0.0013812014953123349,0.0015531175499244212,-0.0028137518483334523,0.0029560922391139314
+5.851996519306413,0.75,3.0,50.0,-0.0012148004616668053,0.0011695325669005927,-0.002339902140585298,0.0023737606926761416
+5.851996519306413,0.81,3.0,43.0,-0.0011132055624340205,0.001104838122784803,-0.002232141938553198,0.0021666940152248113
+5.851996519306413,0.87,3.0,36.0,-0.001015173612307316,0.0010499164652870046,-0.001958935272203398,0.002026205289628539
+5.851996519306413,0.93,3.0,14.0,-0.001431105168689778,0.0013291206178081755,-0.0027383169845084545,0.0026913634261963608
+5.851996519306413,0.99,3.0,21.0,-0.001050989245163912,0.000796880466478151,-0.002184614467806494,0.001517200313842747
+5.851996519306413,1.05,3.0,27.0,-0.0006104474441592971,0.0005392072888242548,-0.0011533717751006582,0.0010548699675229328
+7.434694395049642,0.33,3.0,13.0,-0.0026642227427129315,0.002850924818704615,-0.005021045567960182,0.00587125488582683
+7.434694395049642,0.39,3.0,31.0,-0.002097622705106367,0.002157655159495191,-0.004097045682536547,0.004217781580440627
+7.434694395049642,0.45,3.0,42.0,-0.0014271781946801454,0.0014661409082016416,-0.002660920071639628,0.002991162649041567
+7.434694395049642,0.51,3.0,65.0,-0.0014683829893431134,0.0015342571101827893,-0.002900099014128315,0.002989414462969146
+7.434694395049642,0.57,3.0,48.0,-0.0016282558259154078,0.0018290719921519403,-0.0032331222649082635,0.0035885026997683044
+7.434694395049642,0.63,3.0,63.0,-0.0017776086765445565,0.0016090219862182266,-0.0034876309346093164,0.0030780118083407054
+7.434694395049642,0.69,3.0,57.0,-0.0017008237775588658,0.0017734460278702128,-0.0033914148515937874,0.0032928269992854517
+7.434694395049642,0.75,3.0,42.0,-0.0013780881807362157,0.0014111835189401275,-0.0027056587850906575,0.0027735622902940902
+7.434694395049642,0.81,3.0,35.0,-0.0019642375299500883,0.002050920727084842,-0.004002412452716785,0.0038735057212769893
+7.434694395049642,0.87,3.0,21.0,-0.0048914880763908115,0.003919367522363249,-0.009750185219118933,0.007352469193870337
+7.434694395049642,0.93,3.0,27.0,-0.0009997096876098904,0.0015416807311647602,-0.0018568856803825957,0.0033515380019471497
+7.434694395049642,0.99,3.0,20.0,-0.001821492662200865,0.0014512474144170874,-0.003524050837765766,0.002745225125946593
+7.434694395049642,1.05,3.0,34.0,-0.000763084866461452,0.0007744543649763893,-0.0015163726393494438,0.0015306018227937432
+9.445439785451777,0.27,3.0,8.0,-0.0017734515320502325,0.001400263660926715,-0.003550603347994722,0.0025627278945011783
+9.445439785451777,0.33,3.0,23.0,-0.0018646541701598726,0.0016360247023448817,-0.003658242885876083,0.0032183130384227814
+9.445439785451777,0.39,3.0,37.0,-0.0012093341175023861,0.0011039115124982799,-0.002325183534152388,0.002286531992777545
+9.445439785451777,0.45,3.0,38.0,-0.0010468046181680713,0.001234737162068423,-0.002033226099760466,0.0024414395132222127
+9.445439785451777,0.51,3.0,58.0,-0.001136512804789054,0.001211873473745666,-0.002295281230364189,0.002425541344495843
+9.445439785451777,0.57,3.0,51.0,-0.0016753426085733794,0.0015684103790008655,-0.003196895532581695,0.003139451439835135
+9.445439785451777,0.63,3.0,58.0,-0.001467033183061152,0.0015256194935308587,-0.0028472053818487755,0.0030884330502841985
+9.445439785451777,0.69,3.0,52.0,-0.0015501886784577287,0.001688625350650288,-0.003034370290097832,0.0032487467869443927
+9.445439785451777,0.75,3.0,30.0,-0.0018563886779168481,0.0016294191551180844,-0.0037793011763663964,0.0031538030784452956
+9.445439785451777,0.81,3.0,24.0,-0.004701077933220507,0.004068545960748149,-0.009161428886219623,0.007894623464116223
+9.445439785451777,0.87,3.0,30.0,-0.005411352895669255,0.0040943756026877035,-0.011038439394053932,0.007689844065216098
+9.445439785451777,0.93,3.0,23.0,-0.006253566539029847,0.00699452958073204,-0.011464275500678344,0.015265389216832601
+9.445439785451777,0.99,3.0,34.0,-0.0011198862655354784,0.001149478439970093,-0.002107168711021154,0.0022694514769174686
+9.445439785451777,1.05,3.0,34.0,-0.0009347057506317107,0.001073535993391803,-0.001929423645891344,0.0019919199466444924
+12.000000000000014,0.33,3.0,13.0,-0.0018355409102158984,0.0014992585140684387,-0.0036755859527439175,0.0027390186761134167
+12.000000000000014,0.39,3.0,24.0,-0.0017769296458488104,0.001764010396961907,-0.0033147792383984758,0.003550403357370258
+12.000000000000014,0.45,3.0,40.0,-0.0015588999178130268,0.0014494295293908087,-0.0030796726710740335,0.0027699755342849427
+12.000000000000014,0.51,3.0,61.0,-0.0013558568059656912,0.0012805494441514632,-0.00269080210835374,0.0024230902218344117
+12.000000000000014,0.57,3.0,62.0,-0.0017395748260810254,0.0015465885976028676,-0.003339690145111813,0.00319634419146178
+12.000000000000014,0.63,3.0,72.0,-0.0012973719551848581,0.0013286482448050217,-0.002633247451429168,0.0025100829093053847
+12.000000000000014,0.69,3.0,52.0,-0.0012528867228397244,0.001304890394557582,-0.002443054564591529,0.002627338408709368
+12.000000000000014,0.75,3.0,26.0,-0.0027343635881039883,0.0022150649870365637,-0.005664165700281237,0.00424721902052544
+12.000000000000014,0.81,3.0,26.0,-0.002022602337681744,0.0021390252637031176,-0.004384817014614516,0.0038951629779629617
+12.000000000000014,0.87,3.0,26.0,-0.01217164467259648,0.00957719521976066,-0.025460064218492996,0.016525885167328537
+12.000000000000014,0.93,3.0,12.0,-0.011803144708892918,0.01620001187338028,-0.014816769766887755,0.05197712876758723
+12.000000000000014,0.99,3.0,22.0,-0.002146480684674516,0.0019270040376234573,-0.0042886444610898454,0.003872231626649537
+12.000000000000014,1.05,3.0,43.0,-0.0021246406913715665,0.0018706593438794854,-0.004116847787325501,0.0037235140916633902
+12.000000000000014,1.11,3.0,19.0,-0.0014145461724545613,0.0010159143204884428,-0.0028190524877680827,0.00192548160288451
```

### Comparing `pyspk-1.3/pyspk.egg-info/PKG-INFO` & `pyspk-1.4/pyspk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.3
+Version: 1.4
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
                           _____ ____   ____   _ 
         ____  __  __     / ___// __ \_/_/ /__| |
        / __ \/ / / /_____\__ \/ /_/ / // //_// /
       / /_/ / /_/ /_____/__/ / ____/ // ,<  / / 
      / .___/\__, /     /____/_/   / //_/|_|/_/  
     /_/    /____/                 |_|    /_/    
 
-py-SP(k) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
+py-SP(k) [(Salcido et al. 2023)](https://academic.oup.com/mnras/article/523/2/2247/7165765) is a python package aimed at predicting the suppression of the total matter power spectrum due to baryonic physics as a function of the baryon fraction of haloes and redshift.
 
 ## Requirements
 
 The module requires the following:
 
 - numpy
 - scipy
@@ -129,21 +129,23 @@
 ## Acknowledging the code
 
 Please cite py-SP(k) using:
 
 ```
 @ARTICLE{SPK_Salcido_2023,
     author = {Salcido, Jaime and McCarthy, Ian G and Kwan, Juliana and Upadhye, Amol and Font, Andreea S},
-    title = "{SP(k) - A hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
+    title = "{SP(k) – a hydrodynamical simulation-based model for the impact of baryon physics on the non-linear matter power spectrum}",
     journal = {Monthly Notices of the Royal Astronomical Society},
+    volume = {523},
+    number = {2},
+    pages = {2247-2262},
     year = {2023},
     month = {05},
     issn = {0035-8711},
     doi = {10.1093/mnras/stad1474},
     url = {https://doi.org/10.1093/mnras/stad1474},
-    note = {stad1474},
-    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stad1474/50356057/stad1474.pdf},
+    eprint = {https://academic.oup.com/mnras/article-pdf/523/2/2247/50512773/stad1474.pdf},
 }
 ```
 For any questions and enquires please contact me via email at *j.salcidonegrete@ljmu.ac.uk*
```

### Comparing `pyspk-1.3/setup.py` & `pyspk-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.3,
+    version=1.4,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

