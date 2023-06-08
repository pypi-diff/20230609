# Comparing `tmp/tinybrain-1.3.3.tar.gz` & `tmp/tinybrain-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybrain-1.3.3.tar", last modified: Sat Jun  3 00:09:23 2023, max compression
+gzip compressed data, was "tinybrain-1.4.0.tar", last modified: Thu Jun  8 20:21:03 2023, max compression
```

## Comparing `tinybrain-1.3.3.tar` & `tinybrain-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.762244 tinybrain-1.3.3/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.752266 tinybrain-1.3.3/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.758597 tinybrain-1.3.3/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      947 2023-05-06 23:45:33.000000 tinybrain-1.3.3/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)      878 2022-08-26 19:08:36.000000 tinybrain-1.3.3/.github/workflows/run_tests.yml
--rw-r--r--   0 wms        (501) staff       (20)       97 2023-06-03 00:09:22.000000 tinybrain-1.3.3/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     4721 2023-06-03 00:09:22.000000 tinybrain-1.3.3/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.3.3/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-03 00:09:23.762505 tinybrain-1.3.3/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.3.3/README.md
--rw-r--r--   0 wms        (501) staff       (20)    21512 2022-08-26 19:05:33.000000 tinybrain-1.3.3/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.3.3/build_linux.sh
--rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.3.3/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.3.3/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.3.3/manylinux2014.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.3.3/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.3.3/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.3.3/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.3.3/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)      924 2023-06-03 00:09:23.763731 tinybrain-1.3.3/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     1141 2023-05-11 20:23:17.000000 tinybrain-1.3.3/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.760348 tinybrain-1.3.3/tinybrain/
--rw-r--r--   0 wms        (501) staff       (20)      183 2023-06-02 23:47:47.000000 tinybrain-1.3.3/tinybrain/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    25889 2023-06-02 23:52:33.000000 tinybrain-1.3.3/tinybrain/accelerated.hpp
--rw-r--r--   0 wms        (501) staff       (20)    26323 2022-03-05 06:53:04.000000 tinybrain-1.3.3/tinybrain/accelerated.pyx
--rw-r--r--   0 wms        (501) staff       (20)    15497 2023-06-01 19:36:31.000000 tinybrain-1.3.3/tinybrain/downsample.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.762006 tinybrain-1.3.3/tinybrain.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      616 2023-06-03 00:09:23.000000 tinybrain-1.3.3/tinybrain.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.3.3/tinybrain.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       10 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)      208 2023-05-11 20:22:50.000000 tinybrain-1.3.3/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-08 20:21:03.647532 tinybrain-1.4.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-08 20:21:03.639423 tinybrain-1.4.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-08 20:21:03.644981 tinybrain-1.4.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      947 2023-05-06 23:45:33.000000 tinybrain-1.4.0/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)      878 2022-08-26 19:08:36.000000 tinybrain-1.4.0/.github/workflows/run_tests.yml
+-rw-r--r--   0 wms        (501) staff       (20)       97 2023-06-08 20:21:02.000000 tinybrain-1.4.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     4881 2023-06-08 20:21:02.000000 tinybrain-1.4.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.4.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-08 20:21:03.647786 tinybrain-1.4.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.4.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    23095 2023-06-08 20:17:42.000000 tinybrain-1.4.0/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.4.0/build_linux.sh
+-rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.4.0/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.4.0/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.4.0/manylinux2014.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.4.0/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.4.0/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.4.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.4.0/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)      924 2023-06-08 20:21:03.649115 tinybrain-1.4.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     1141 2023-05-11 20:23:17.000000 tinybrain-1.4.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-08 20:21:03.645928 tinybrain-1.4.0/tinybrain/
+-rw-r--r--   0 wms        (501) staff       (20)      183 2023-06-08 20:20:18.000000 tinybrain-1.4.0/tinybrain/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    29621 2023-06-08 20:17:42.000000 tinybrain-1.4.0/tinybrain/accelerated.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    28263 2023-06-08 20:17:42.000000 tinybrain-1.4.0/tinybrain/accelerated.pyx
+-rw-r--r--   0 wms        (501) staff       (20)    15569 2023-06-08 20:17:42.000000 tinybrain-1.4.0/tinybrain/downsample.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-08 20:21:03.647368 tinybrain-1.4.0/tinybrain.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-08 20:21:02.000000 tinybrain-1.4.0/tinybrain.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      616 2023-06-08 20:21:03.000000 tinybrain-1.4.0/tinybrain.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-08 20:21:02.000000 tinybrain-1.4.0/tinybrain.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.4.0/tinybrain.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-08 20:21:02.000000 tinybrain-1.4.0/tinybrain.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-06-08 20:21:02.000000 tinybrain-1.4.0/tinybrain.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       10 2023-06-08 20:21:02.000000 tinybrain-1.4.0/tinybrain.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)      208 2023-05-11 20:22:50.000000 tinybrain-1.4.0/tox.ini
```

### Comparing `tinybrain-1.3.3/.github/workflows/build_wheel.yml` & `tinybrain-1.4.0/.github/workflows/build_wheel.yml`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/.github/workflows/run_tests.yml` & `tinybrain-1.4.0/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/ChangeLog` & `tinybrain-1.4.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+1.4.0
+-----
+
+* release(1.4.0): full support for 2x2x1 avg pooling
+* perf: 2x2x1 sparse avg pooling  (#20)
+* feat: numpy implementation of sparse for averaging
+
 1.3.3
 -----
 
 * release(1.3.3): fix sparse mode 2x2x2 seg ds and throw error
 * fix: throw error if sparse mode isn't supported
 * refactor: remove unused variable oyoff
 * fix: incorrect sparse check value in 2x2x2 mode downsampling
```

### Comparing `tinybrain-1.3.3/LICENSE` & `tinybrain-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/PKG-INFO` & `tinybrain-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.3.3
+Version: 1.4.0
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)
```

### Comparing `tinybrain-1.3.3/README.md` & `tinybrain-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/automated_test.py` & `tinybrain-1.4.0/automated_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,35 +122,78 @@
     ],
   ])
 
   assert np.array_equal(oddimg, ans3x3x3)
   assert np.array_equal(oddimgf, ans3x3x3)
 
 @pytest.mark.parametrize("dtype", (np.uint8, np.uint16, np.float32, np.float64))
-def test_accelerated_vs_numpy_avg_pooling_2x2(dtype):
-  image = np.random.randint(0,255, size=(512, 512, 6), dtype=np.uint8).astype(dtype)
+@pytest.mark.parametrize("sparse", [False, True])
+def test_accelerated_vs_numpy_avg_pooling_2x2x1(dtype, sparse):
+  image = np.random.randint(0,255, size=(512, 512, 6), dtype=np.uint8).astype(dtype, copy=False)
   imagef = np.asfortranarray(image)
 
-  accimg = tinybrain.accelerated.average_pooling_2x2(imagef) 
-  npimg = tinybrain.downsample.downsample_with_averaging_numpy(imagef, (2,2,1))
+  accimg = tinybrain.accelerated.average_pooling_2x2(imagef, sparse=sparse) 
+  npimg = tinybrain.downsample.downsample_with_averaging_numpy(imagef, (2,2,1), sparse=sparse)
   assert np.all(accimg == npimg)
 
   # There are slight differences in how the accelerated version and 
   # the numpy version handle the edge so we only compare a nice 
   # even power of two where there's no edge. We also can't do iterated
   # downsamples of the (naked) numpy version because it will result in
   # integer truncation. We can't compare above mip 4 because the accelerated
   # version will exhibit integer truncation.
 
-  mips = tinybrain.downsample_with_averaging(imagef, (2,2,1), num_mips=4)
-  npimg = tinybrain.downsample.downsample_with_averaging_numpy(imagef, (16,16,1))
-  
+  mips = tinybrain.downsample_with_averaging(imagef, (2,2,1), num_mips=4, sparse=sparse)
+  npimg = tinybrain.downsample.downsample_with_averaging_numpy(imagef, (16,16,1), sparse=sparse)
+
   assert np.all(mips[-1] == npimg)
 
 @pytest.mark.parametrize("dtype", (np.uint8, np.uint16, np.float32, np.float64))
+def test_accelerated_vs_numpy_avg_pooling_2x2x1_simple_sparse(dtype):
+  for x in [0,1]:
+    for y in [0,1]:
+      image = np.zeros((2,2,1,3), order="F", dtype=dtype)
+      image[x,y,0,0] = 1
+      image[x,y,0,1] = 2
+      image[x,y,0,2] = 3
+      res = tinybrain.accelerated.average_pooling_2x2(image, num_mips=1, sparse=True) 
+      
+      ans = np.zeros((1,1,1,3), order="F", dtype=dtype)
+      ans[0,0,0,0] = 1
+      ans[0,0,0,1] = 2
+      ans[0,0,0,2] = 3
+      assert np.all(res == ans)
+
+  for x in [0,1]:
+    for y in [0,1]:
+      image = np.zeros((4,4,1,3), order="F", dtype=dtype)
+      image[x,y,0,0] = 1
+      image[x,y,0,1] = 2
+      image[x,y,0,2] = 3
+      res = tinybrain.accelerated.average_pooling_2x2(image, num_mips=2, sparse=True) 
+      res = res[1]
+
+      ans = np.zeros((1,1,1,3), order="F", dtype=dtype)
+      ans[0,0,0,0] = 1
+      ans[0,0,0,1] = 2
+      ans[0,0,0,2] = 3
+      assert np.all(res == ans)
+
+  image = np.zeros((2,2,1,3), order="F", dtype=dtype)
+  ans = np.zeros((1,1,1,3), order="F", dtype=dtype)
+  res = tinybrain.accelerated.average_pooling_2x2(image, num_mips=1, sparse=True) 
+  assert np.all(res[0] == ans)
+
+  image = np.zeros((4,4,1,3), order="F", dtype=dtype)
+  ans = np.zeros((1,1,1,3), order="F", dtype=dtype)
+  res = tinybrain.accelerated.average_pooling_2x2(image, num_mips=2, sparse=True) 
+  assert np.all(res[1] == ans)
+
+
+@pytest.mark.parametrize("dtype", (np.uint8, np.uint16, np.float32, np.float64))
 @pytest.mark.parametrize("sx", (6,7,1024,1025))
 @pytest.mark.parametrize("sy", (6,7,1024,1025))
 @pytest.mark.parametrize("sz", (4,5,32,33))
 def test_accelerated_vs_numpy_avg_pooling_2x2x2(dtype, sx, sy, sz):
   image = np.random.randint(0,255, size=(sx, sy, sz), dtype=np.uint8).astype(dtype)
   imagef = np.asfortranarray(image)
```

### Comparing `tinybrain-1.3.3/build_linux.sh` & `tinybrain-1.4.0/build_linux.sh`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/manylinux1.Dockerfile` & `tinybrain-1.4.0/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/manylinux2010.Dockerfile` & `tinybrain-1.4.0/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/manylinux2014.Dockerfile` & `tinybrain-1.4.0/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/perf.py` & `tinybrain-1.4.0/perf.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/setup.cfg` & `tinybrain-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/setup.py` & `tinybrain-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.3/tinybrain/accelerated.hpp` & `tinybrain-1.4.0/tinybrain/accelerated.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 // lower memory version for a single mip level
 
 template <typename T>
 T* _average_pooling_2x2_single_mip(
   const T* channel, 
   const size_t sx, const size_t sy, 
   const size_t sz, const size_t sw = 1,
-  T* out = NULL
+  T* out = NULL, const bool sparse = false
 ) {
   using T2 = typename PromotedType<T>::type; // e.g. uint8_t -> uint16_t
 
   const size_t sxy = sx * sy;
 
   const size_t osx = (sx + 1) >> 1;
   const size_t osy = (sy + 1) >> 1;
@@ -334,47 +334,105 @@
   size_t zoff, ozoff;
 
   for (size_t w = 0; w < sw; w++) {
     for (size_t z = 0; z < sz; z++) {
       zoff = sxy * (z + sz * w);
       ozoff = osxy * (z + sz * w);
 
-      for (y = 0, oy = 0; y < sy - odd_y; y += 2, oy++) {
-        for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
-          out[ox + osx * oy + ozoff] = static_cast<T>(
-            (
-                static_cast<T2>(channel[x + sx * y + zoff]) 
-              + static_cast<T2>(channel[(x+1) + sx * y + zoff])
-              + static_cast<T2>(channel[x + sx * (y+1) + zoff]) 
-              + static_cast<T2>(channel[(x+1) + sx * (y+1) + zoff])
-            ) / 4
-          );
-        }
-
-        if (odd_x) {
-          out[(ox - 1) + osx * oy + ozoff] = static_cast<T>(
-            (
-                static_cast<T2>(channel[x + sx * y + zoff])
-              + static_cast<T2>(channel[x + sx * (y+1) + zoff])
-            ) / 2
-          );
-        }
+      if (sparse) {
+        for (y = 0, oy = 0; y < sy - odd_y; y += 2, oy++) {
+          for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
+            T a = channel[x + sx * y + zoff];
+            T b = channel[(x+1) + sx * y + zoff];
+            T c = channel[x + sx * (y+1) + zoff];
+            T d = channel[(x+1) + sx * (y+1) + zoff];
+
+            out[ox + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(a) 
+                + static_cast<T2>(b)
+                + static_cast<T2>(c) 
+                + static_cast<T2>(d)
+              ) / static_cast<T2>(
+                  std::max(
+                    static_cast<T>((a > 0) + (b > 0) + (c > 0) + (d > 0)),
+                    static_cast<T>(1)
+                  )
+                )
+              );
+          }
+
+          if (odd_x) {
+            T a = channel[x + sx * y + zoff];
+            T b = channel[x + sx * (y+1) + zoff];
+            out[(ox - 1) + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(a)
+                + static_cast<T2>(b)
+              ) / static_cast<T2>(
+                std::max(
+                  static_cast<T>((a > 0) + (b > 0)),
+                  static_cast<T>(1)
+              )
+            ));
+          }
+        }
+      }
+      else {
+        for (y = 0, oy = 0; y < sy - odd_y; y += 2, oy++) {
+          for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
+            out[ox + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(channel[x + sx * y + zoff]) 
+                + static_cast<T2>(channel[(x+1) + sx * y + zoff])
+                + static_cast<T2>(channel[x + sx * (y+1) + zoff]) 
+                + static_cast<T2>(channel[(x+1) + sx * (y+1) + zoff])
+              ) / 4
+            );
+          }
+
+          if (odd_x) {
+            out[(ox - 1) + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(channel[x + sx * y + zoff])
+                + static_cast<T2>(channel[x + sx * (y+1) + zoff])
+              ) / 2
+            );
+          }
+        }        
       }
 
       if (odd_y) {
         y = sy - 1;
         oy = osy - 1;
 
-        for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
-          out[ox + osx * oy + ozoff] = static_cast<T>(
-            (
-                static_cast<T2>(channel[x + sx * y + zoff]) 
-              + static_cast<T2>(channel[(x+1) + sx * y + zoff])
-            ) / 2
-          );
+        if (sparse) {
+          for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
+            out[ox + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(channel[x + sx * y + zoff]) 
+                + static_cast<T2>(channel[(x+1) + sx * y + zoff])
+              ) / 2
+            );
+          }
+        }
+        else {
+          T a = channel[x + sx * y + zoff];
+          T b = channel[(x+1) + sx * y + zoff];
+          for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
+            out[ox + osx * oy + ozoff] = static_cast<T>(
+              (
+                  static_cast<T2>(a) 
+                + static_cast<T2>(b)
+              ) / static_cast<T2>(std::max(
+                  static_cast<T>((a > 0) + (b > 0)),
+                  static_cast<T>(1)
+              ))
+            );
+          }          
         }
 
         if (odd_x) {
           out[(ox - 1) + osx * oy + ozoff] = channel[x + sx * y + zoff]; // corner
         }
       }
     }
@@ -663,14 +721,84 @@
     // to avoid darkening during render
     denom[(osx - 1) + o_offset] += static_cast<U>(channel[(sx - 1) + offset] != 0);
   }
 }
 
 // used for sparse=True only
 template <typename T, typename U>
+U* denominator_2x2(
+    T* channel, 
+    const size_t sx, const size_t sy, 
+    const size_t sz, const size_t sw = 1
+  ) {
+
+  const size_t sxy = sx * sy;
+
+  const size_t osx = (sx + 1) >> 1;
+  const size_t osy = (sy + 1) >> 1;
+  const size_t osz = sz;
+  const size_t osxy = osx * osy;
+  const size_t ovoxels = osxy * osz * sw;
+
+  const bool odd_y = (sy & 0x01);
+
+  U* denom = new U[ovoxels]();
+
+  size_t y, oy;
+  size_t zoff, ozoff, oyoff;
+
+  for (size_t w = 0; w < sw; w++) {
+    for (size_t z = 0; z < sz; z++) {
+      zoff = sxy * (z + sz * w);
+      ozoff = osxy * (z + sz * w);
+      
+      for (y = 0, oy = 0; y < sy - (size_t)odd_y; y++, oy++) {
+        denominator_x_pass<T, U>(
+          channel, denom, 
+          sx, osx,
+          (sx * y + zoff), (osx * oy + ozoff)
+        );
+
+        y++;
+
+        denominator_x_pass<T, U>(
+          channel, denom, 
+          sx, osx,
+          (sx * y + zoff), (osx * oy + ozoff)
+        );
+      }
+
+      if (odd_y) {
+        y = sy - 1;
+        oy = osy - 1;
+        oyoff = (osx * oy + ozoff);
+        denominator_x_pass<T, U>(
+          channel, denom, 
+          sx, osx,
+          (sx * y + zoff), oyoff
+        );
+      }
+    }
+
+    if (odd_y) {
+      y = sy - 1;
+      oy = osy - 1;
+      oyoff = (osx * oy + ozoff);
+      // double values to prevent darkening 
+      for (size_t x = 0; x < osx; x++) {
+        denom[x + oyoff] *= 2;
+      }
+    }
+  }
+
+  return denom;
+}
+
+// used for sparse=True only
+template <typename T, typename U>
 U* denominator_2x2x2(
     T* channel, 
     const size_t sx, const size_t sy, 
     const size_t sz, const size_t sw = 1
   ) {
 
   const size_t sxy = sx * sy;
@@ -808,14 +936,26 @@
 inline void render_image_floating(T* accum, T* oimg, const T divisor, const size_t ovoxels) {
   for (size_t i = 0; i < ovoxels; i++) {
     oimg[i] = accum[i] / divisor;
   }
 }
 
 template <typename T>
+inline void render_image_floating_sparse(T* accum, T* denominator, T* oimg, const size_t ovoxels) {
+  for (size_t i = 0; i < ovoxels; i++) {
+    if (denominator[i] == 0) {
+      oimg[i] = 0;
+    }
+    else {
+      oimg[i] = accum[i] / denominator[i];
+    }
+  }
+}
+
+template <typename T>
 inline void shift_right(T* accum, const size_t ovoxels, const size_t bits) {
   for (size_t i = 0; i < ovoxels; i++) {
     accum[i] >>= bits;
   }
 }
 
 template <typename T>
```

### Comparing `tinybrain-1.3.3/tinybrain/accelerated.pyx` & `tinybrain-1.4.0/tinybrain/accelerated.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+# cython: language_level=3
 """
 Cython accelerated routines for common downsampling operations.
 
 Author: William Silversmith
 Affiliation: Seung Lab, Princeton Neuroscience Institute
 Date: March 2019
 """
 cimport cython
 from cython cimport floating
-from cpython cimport PyObject, Py_INCREF
 from libc.stdint cimport (
   int8_t, int16_t, int32_t, int64_t,
   uint8_t, uint16_t, uint32_t, uint64_t,
 )
 import ctypes
 
 from libc.stdlib cimport malloc, free
 from cpython.mem cimport PyMem_Malloc, PyMem_Free
 
 cimport numpy as np
 import numpy as np
 np.import_array()
 
 cdef extern from "accelerated.hpp" namespace "accelerated":
-  cdef T* _average_pooling_2x2_single_mip[T](T* arr, size_t sx, size_t sy, size_t sz, size_t sw, T* out)
+  cdef T* _average_pooling_2x2_single_mip[T](T* arr, size_t sx, size_t sy, size_t sz, size_t sw, T* out, uint8_t sparse)
   cdef U* accumulate_2x2[T, U](T* arr, size_t sx, size_t sy, size_t sz, size_t sw)
   cdef T* accumulate_2x2f[T](T* arr, size_t sx, size_t sy, size_t sz, size_t sw)
+  cdef U* denominator_2x2[T, U](T* arr, size_t sx, size_t sy, size_t sz, size_t sw)
   cdef T* _average_pooling_2x2x2_single_mip[T](T* arr, size_t sx, size_t sy, size_t sz, size_t sw, T* out)
   cdef U* accumulate_2x2x2[T, U](T* arr, size_t sx, size_t sy, size_t sz, size_t sw)
   cdef U* denominator_2x2x2[T, U](T* arr, size_t sx, size_t sy, size_t sz, size_t sw)
   cdef void render_image[T, U](T* arr, U* oimg, uint32_t bitshift, size_t ovoxels)
   cdef void render_image_sparse[T, U](T* numerator, T* denominator, U* oimg, size_t ovoxels)
   cdef void render_image_floating[T](T* arr, T* oimg, T divisor, size_t ovoxels)
+  cdef void render_image_floating_sparse[T](T* accum, T* denominator, T* oimg, size_t ovoxels)
   cdef T* shift_right[T](T* arr, size_t ovoxels, size_t bits)
   cdef void _mode_pooling_2x2[T](
     T* img, T* oimg, 
     size_t sx, size_t sy, 
     size_t sz, size_t sw,
     size_t stride_x, size_t stride_y,
     size_t stride_z, size_t stride_w
@@ -72,44 +74,44 @@
 ctypedef fused NUMBER:
   INTEGER
   float
   double
 
 ### AVERAGE POOLING 2x2 ####
 
-def average_pooling_2x2(channel, size_t num_mips=1):
+def average_pooling_2x2(channel, size_t num_mips=1, sparse=False):
   ndim = channel.ndim
   channel = expand_dims(channel, 4)
 
   cdef size_t sx = channel.shape[0]
   cdef size_t sy = channel.shape[1]
 
   if min(sx, sy) < <size_t>(2 ** num_mips):
     raise ValueError("Can't downsample smaller than the smallest XY plane dimension.")
 
   results = []
   if num_mips == 1:
-    results = _average_pooling_2x2_single_mip_py(channel)
+    results = _average_pooling_2x2_single_mip_py(channel, sparse)
   elif channel.dtype == np.uint8:
-    results = _average_pooling_2x2_uint8(channel, num_mips)
+    results = _average_pooling_2x2_uint8(channel, num_mips, sparse)
   elif channel.dtype == np.uint16:
-    results = _average_pooling_2x2_uint16(channel, num_mips)
+    results = _average_pooling_2x2_uint16(channel, num_mips, sparse)
   elif channel.dtype == np.float32:
-    results = _average_pooling_2x2_float(channel, num_mips)
+    results = _average_pooling_2x2_float(channel, num_mips, sparse)
   elif channel.dtype == np.float64:
-    results = _average_pooling_2x2_double(channel, num_mips)
+    results = _average_pooling_2x2_double(channel, num_mips, sparse)
   else:
     raise TypeError("Unsupported data type: ", channel.dtype)
 
   for i, img in enumerate(results):
     results[i] = squeeze_dims(img, ndim)
 
   return results
 
-def _average_pooling_2x2_single_mip_py(np.ndarray[NUMBER, ndim=4] channel):
+def _average_pooling_2x2_single_mip_py(np.ndarray[NUMBER, ndim=4] channel, sparse):
   cdef uint8_t[:,:,:,:] arr_memview8u
   cdef uint16_t[:,:,:,:] arr_memview16u
   cdef uint32_t[:,:,:,:] arr_memview32u
   cdef uint64_t[:,:,:,:] arr_memview64u
   cdef float[:,:,:,:] arr_memviewf
   cdef double[:,:,:,:] arr_memviewd
 
@@ -128,41 +130,41 @@
   shape = ( (sx+1)//2, (sy+1)//2, sz, sw )
 
   cdef np.ndarray[NUMBER, ndim=4] out = np.zeros(shape, dtype=channel.dtype, order="F")
 
   if channel.dtype == np.uint8:
     arr_memview8u = channel
     out_memview8u = out
-    _average_pooling_2x2_single_mip[uint8_t](&arr_memview8u[0,0,0,0], sx, sy, sz, sw, &out_memview8u[0,0,0,0])
+    _average_pooling_2x2_single_mip[uint8_t](&arr_memview8u[0,0,0,0], sx, sy, sz, sw, &out_memview8u[0,0,0,0], bool(sparse))
   elif channel.dtype == np.uint16:
     arr_memview16u = channel
     out_memview16u = out
-    _average_pooling_2x2_single_mip[uint16_t](&arr_memview16u[0,0,0,0], sx, sy, sz, sw, &out_memview16u[0,0,0,0])
+    _average_pooling_2x2_single_mip[uint16_t](&arr_memview16u[0,0,0,0], sx, sy, sz, sw, &out_memview16u[0,0,0,0], bool(sparse))
   elif channel.dtype == np.uint32:
     arr_memview32u = channel
     out_memview32u = out
-    _average_pooling_2x2_single_mip[uint32_t](&arr_memview32u[0,0,0,0], sx, sy, sz, sw, &out_memview32u[0,0,0,0])
+    _average_pooling_2x2_single_mip[uint32_t](&arr_memview32u[0,0,0,0], sx, sy, sz, sw, &out_memview32u[0,0,0,0], bool(sparse))
   elif channel.dtype == np.uint64:
     arr_memview64u = channel
     out_memview64u = out
-    _average_pooling_2x2_single_mip[uint64_t](&arr_memview64u[0,0,0,0], sx, sy, sz, sw, &out_memview64u[0,0,0,0])
+    _average_pooling_2x2_single_mip[uint64_t](&arr_memview64u[0,0,0,0], sx, sy, sz, sw, &out_memview64u[0,0,0,0], bool(sparse))
   elif channel.dtype == np.float32:
     arr_memviewf = channel
     out_memviewf = out
-    _average_pooling_2x2_single_mip[float](&arr_memviewf[0,0,0,0], sx, sy, sz, sw, &out_memviewf[0,0,0,0])
+    _average_pooling_2x2_single_mip[float](&arr_memviewf[0,0,0,0], sx, sy, sz, sw, &out_memviewf[0,0,0,0], bool(sparse))
   elif channel.dtype == np.float64:
     arr_memviewd = channel
     out_memviewd = out
-    _average_pooling_2x2_single_mip[double](&arr_memviewd[0,0,0,0], sx, sy, sz, sw, &out_memviewd[0,0,0,0])
+    _average_pooling_2x2_single_mip[double](&arr_memviewd[0,0,0,0], sx, sy, sz, sw, &out_memviewd[0,0,0,0], bool(sparse))
   else:
     raise TypeError("Unsupported data type. " + str(channel.dtype))
 
   return [ out ]
 
-def _average_pooling_2x2_uint8(np.ndarray[uint8_t, ndim=4] channel, uint32_t num_mips):
+def _average_pooling_2x2_uint8(np.ndarray[uint8_t, ndim=4] channel, uint32_t num_mips, sparse):
   cdef size_t sx = channel.shape[0]
   cdef size_t sy = channel.shape[1]
   cdef size_t sz = channel.shape[2]
   cdef size_t sw = channel.shape[3]
   cdef size_t sxy = sx * sy
 
   cdef size_t osx = (sx + 1) // 2
@@ -172,22 +174,30 @@
 
   cdef uint8_t[:,:,:,:] channelview = channel
   cdef uint16_t* accum = accumulate_2x2[uint8_t, uint16_t](&channelview[0,0,0,0], sx, sy, sz, sw)
   cdef uint16_t[:] accumview = <uint16_t[:ovoxels]>accum
   cdef uint16_t* tmp
   cdef uint32_t mip, bitshift
 
+  cdef uint16_t* denominator
+  if sparse:
+    denominator = denominator_2x2[uint8_t, uint16_t](&channelview[0,0,0,0], sx, sy, sz, sw)
+
   cdef uint8_t[:] oimgview
 
   results = []
   for mip in range(num_mips):
     bitshift = 2 * ((mip % 4) + 1) # integer truncation every 4 mip levels
     oimg = np.zeros( (ovoxels,), dtype=np.uint8, order='F')
     oimgview = oimg
-    render_image[uint16_t, uint8_t](&accumview[0], &oimgview[0], bitshift, ovoxels)
+
+    if sparse:
+      render_image_sparse[uint16_t, uint8_t](&accumview[0], denominator, &oimgview[0], ovoxels)
+    else:
+      render_image[uint16_t, uint8_t](&accumview[0], &oimgview[0], bitshift, ovoxels)
 
     results.append(
       oimg.reshape( (osx, osy, sz, sw), order='F' )
     )
 
     if mip == num_mips - 1:
       break
@@ -204,19 +214,24 @@
     ovoxels = osxy * sz * sw
 
     tmp = accum 
     accum = accumulate_2x2[uint16_t, uint16_t](accum, sx, sy, sz, sw)
     accumview = <uint16_t[:ovoxels]>accum
     PyMem_Free(tmp)
 
+    if sparse:
+      tmp = denominator
+      denominator = accumulate_2x2[uint16_t, uint16_t](denominator, sx, sy, sz, sw)
+      PyMem_Free(tmp)
+
   PyMem_Free(accum)
 
   return results
 
-def _average_pooling_2x2_uint16(np.ndarray[uint16_t, ndim=4] channel, uint32_t num_mips):
+def _average_pooling_2x2_uint16(np.ndarray[uint16_t, ndim=4] channel, uint32_t num_mips, sparse):
   cdef size_t sx = channel.shape[0]
   cdef size_t sy = channel.shape[1]
   cdef size_t sz = channel.shape[2]
   cdef size_t sw = channel.shape[3]
   cdef size_t sxy = sx * sy
 
   cdef size_t osx = (sx + 1) // 2
@@ -226,22 +241,30 @@
 
   cdef uint16_t[:,:,:,:] channelview = channel
   cdef uint32_t* accum = accumulate_2x2[uint16_t, uint32_t](&channelview[0,0,0,0], sx, sy, sz, sw)
   cdef uint32_t[:] accumview = <uint32_t[:ovoxels]>accum
   cdef uint32_t* tmp
   cdef uint32_t mip, bitshift
 
+  cdef uint32_t* denominator
+  if sparse:
+    denominator = denominator_2x2[uint16_t, uint32_t](&channelview[0,0,0,0], sx, sy, sz, sw)
+
   cdef uint16_t[:] oimgview
 
   results = []
   for mip in range(num_mips):
     bitshift = 2 * ((mip % 4) + 1) # integer truncation every 4 mip levels
     oimg = np.zeros( (ovoxels,), dtype=np.uint16, order='F')
     oimgview = oimg
-    render_image[uint32_t, uint16_t](&accumview[0], &oimgview[0], bitshift, ovoxels)
+
+    if sparse:
+      render_image_sparse[uint32_t, uint16_t](&accumview[0], denominator, &oimgview[0], ovoxels)
+    else:
+      render_image[uint32_t, uint16_t](&accumview[0], &oimgview[0], bitshift, ovoxels)
 
     results.append(
       oimg.reshape( (osx, osy, sz, sw), order='F' )
     )
 
     if mip == num_mips - 1:
       break
@@ -258,19 +281,24 @@
     ovoxels = osxy * sz * sw
 
     tmp = accum 
     accum = accumulate_2x2[uint32_t, uint32_t](accum, sx, sy, sz, sw)
     accumview = <uint32_t[:ovoxels]>accum
     PyMem_Free(tmp)
 
+    if sparse:
+      tmp = denominator
+      denominator = accumulate_2x2[uint32_t, uint32_t](denominator, sx, sy, sz, sw)
+      PyMem_Free(tmp)
+
   PyMem_Free(accum)
 
   return results
 
-def _average_pooling_2x2_float(np.ndarray[float, ndim=4] channel, uint32_t num_mips):
+def _average_pooling_2x2_float(np.ndarray[float, ndim=4] channel, uint32_t num_mips, sparse):
   cdef size_t sx = channel.shape[0]
   cdef size_t sy = channel.shape[1]
   cdef size_t sz = channel.shape[2]
   cdef size_t sw = channel.shape[3]
   cdef size_t sxy = sx * sy
 
   cdef size_t osx = (sx + 1) // 2
@@ -280,23 +308,31 @@
 
   cdef float[:,:,:,:] channelview = channel
   cdef float* accum = accumulate_2x2f[float](&channelview[0,0,0,0], sx, sy, sz, sw)
   cdef float[:] accumview = <float[:ovoxels]>accum
   cdef float* tmp
   cdef uint32_t mip
 
+  cdef float* denominator
+  if sparse:
+    denominator = denominator_2x2[float, float](&channelview[0,0,0,0], sx, sy, sz, sw)
+
   cdef float divisor = 1.0
   cdef float[:] oimgview
 
   results = []
   for mip in range(num_mips):
     divisor = 4.0 ** (mip+1)
     oimg = np.zeros( (ovoxels,), dtype=np.float32, order='F')
     oimgview = oimg
-    render_image_floating[float](&accumview[0], &oimgview[0], divisor, ovoxels)
+
+    if sparse:
+      render_image_floating_sparse[float](&accumview[0], denominator, &oimgview[0], ovoxels)
+    else:
+      render_image_floating[float](&accumview[0], &oimgview[0], divisor, ovoxels)
 
     results.append(
       oimg.reshape( (osx, osy, sz, sw), order='F' )
     )
 
     if mip == num_mips - 1:
       break
@@ -310,19 +346,24 @@
     ovoxels = osxy * sz * sw
 
     tmp = accum 
     accum = accumulate_2x2f[float](accum, sx, sy, sz, sw)
     accumview = <float[:ovoxels]>accum
     PyMem_Free(tmp)
 
+    if sparse:
+      tmp = denominator
+      denominator = accumulate_2x2f[float](denominator, sx, sy, sz, sw)
+      PyMem_Free(tmp)
+
   PyMem_Free(accum)
 
   return results
 
-def _average_pooling_2x2_double(np.ndarray[double, ndim=4] channel, uint32_t num_mips):
+def _average_pooling_2x2_double(np.ndarray[double, ndim=4] channel, uint32_t num_mips, sparse):
   cdef size_t sx = channel.shape[0]
   cdef size_t sy = channel.shape[1]
   cdef size_t sz = channel.shape[2]
   cdef size_t sw = channel.shape[3]
   cdef size_t sxy = sx * sy
 
   cdef size_t osx = (sx + 1) // 2
@@ -335,20 +376,28 @@
   cdef double[:] accumview = <double[:ovoxels]>accum
   cdef double* tmp
   cdef uint32_t mip
 
   cdef double divisor = 1.0
   cdef double[:] oimgview
 
+  cdef double* denominator
+  if sparse:
+    denominator = denominator_2x2[double, double](&channelview[0,0,0,0], sx, sy, sz, sw)
+
   results = []
   for mip in range(num_mips):
     divisor = 4.0 ** (mip+1)
     oimg = np.zeros( (ovoxels,), dtype=np.float64, order='F')
     oimgview = oimg
-    render_image_floating[double](&accumview[0], &oimgview[0], divisor, ovoxels)
+
+    if sparse:
+      render_image_floating_sparse[double](&accumview[0], denominator, &oimgview[0], ovoxels)
+    else:
+      render_image_floating[double](&accumview[0], &oimgview[0], divisor, ovoxels)
 
     results.append(
       oimg.reshape( (osx, osy, sz, sw), order='F' )
     )
 
     if mip == num_mips - 1:
       break
@@ -362,14 +411,19 @@
     ovoxels = osxy * sz * sw
 
     tmp = accum 
     accum = accumulate_2x2f[double](accum, sx, sy, sz, sw)
     accumview = <double[:ovoxels]>accum
     PyMem_Free(tmp)
 
+    if sparse:
+      tmp = denominator
+      denominator = accumulate_2x2f[double](denominator, sx, sy, sz, sw)
+      PyMem_Free(tmp)
+
   PyMem_Free(accum)
 
   return results
 
 ### AVERAGE POOLING 2x2x2 ###
 
 def average_pooling_2x2x2(channel, size_t num_mips=1, sparse=False):
```

### Comparing `tinybrain-1.3.3/tinybrain/downsample.py` & `tinybrain-1.4.0/tinybrain/downsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,30 +46,28 @@
   """
   if (
     img.dtype in (np.uint8, np.uint16, np.float32, np.float64)
     or num_mips == 1 # _average_pooling_2x2_single_mip_py supports all primative types
   ):
     img = np.asfortranarray(img)
     if (tuple(factor) in ( (2,2), (2,2,1), (2,2,1,1) )):
-      if sparse:
-        raise ValueError("sparse mode is not implemented for 2x2.")
-      return tinybrain.accelerated.average_pooling_2x2(img, num_mips)
+      return tinybrain.accelerated.average_pooling_2x2(img, num_mips, sparse)
     elif (tuple(factor) in ( (2,2,2), (2,2,2,1) )):
       return tinybrain.accelerated.average_pooling_2x2x2(img, num_mips, sparse)
 
   results = []
   if np.dtype(img.dtype).itemsize < 4:
     dtype = img.dtype
     img = img.astype(np.float32)
     for mip in range(num_mips):
-      img = downsample_with_averaging_numpy(img, factor)
+      img = downsample_with_averaging_numpy(img, factor, sparse)
       results.append(img.astype(dtype))
   else:
     for mip in range(num_mips):
-      img = downsample_with_averaging_numpy(img, factor)
+      img = downsample_with_averaging_numpy(img, factor, sparse)
       results.append(img)
 
   return results
 
 def validate_factor(array, factor):
   factor = np.array(factor, dtype=np.int32)
   if np.any(factor <= 0):
@@ -113,15 +111,15 @@
   newimg[-1,-1,:] = image[-1,-1,:]
   newimg[:sx-ox,-1,:] = image[:,-1,:]
   newimg[-1,:sy-oy,:] = image[-1,:,:]
   newimg[:sx-ox,:sy-oy] = image
   
   return newimg
 
-def downsample_with_averaging_numpy(array, factor):
+def downsample_with_averaging_numpy(array, factor, sparse=False):
   """
   Downsample x by factor using averaging.
 
   If factor has fewer parameters than data.shape, the remainder
   are assumed to be 1.
 
   @return: The downsampled array, of the same type as x.
@@ -133,15 +131,21 @@
   output_shape = tuple(int(math.ceil(s / f)) for s, f in zip(array.shape, factor))
   temp = np.zeros(output_shape, dtype=np.float32)
   counts = np.zeros(output_shape, int)
   for offset in np.ndindex(factor):
     part = array[tuple(np.s_[o::f] for o, f in zip(offset, factor))]
     indexing_expr = tuple(np.s_[:s] for s in part.shape)
     temp[indexing_expr] += part
-    counts[indexing_expr] += 1
+    if sparse:
+      counts[indexing_expr] += part > 0
+    else:
+      counts[indexing_expr] += 1
+
+  if sparse:
+    np.maximum(counts, 1, out=counts)
   return np.cast[array.dtype](temp / counts)
 
 def downsample_with_max_pooling(array, factor, num_mips=1):
   """
   Downsample by picking the maximum value within a
   cuboid specified by factor. That is, a reduction factor
   of 2x2 works by summarizing many 2x2 cuboids. If factor's
```

### Comparing `tinybrain-1.3.3/tinybrain.egg-info/PKG-INFO` & `tinybrain-1.4.0/tinybrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.3.3
+Version: 1.4.0
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)
```

### Comparing `tinybrain-1.3.3/tinybrain.egg-info/SOURCES.txt` & `tinybrain-1.4.0/tinybrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

