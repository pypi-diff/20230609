# Comparing `tmp/snake_opencv-0.1.3.tar.gz` & `tmp/snake_opencv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_opencv-0.1.3.tar", max compression
+gzip compressed data, was "snake_opencv-0.1.4.tar", max compression
```

## Comparing `snake_opencv-0.1.3.tar` & `snake_opencv-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.3/LICENSE
--rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.3/README.md
--rw-r--r--   0        0        0      686 2023-05-25 18:09:05.544570 snake_opencv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.3/snake_opencv/__init__.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.3/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.3/snake_opencv/core/binding.py
--rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.3/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.3/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.3/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.3/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.3/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.3/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.3/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.3/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.3/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.3/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.3/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    42748 2023-05-28 23:54:03.339666 snake_opencv-0.1.3/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.3/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.3/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.3/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.3/snake_opencv/photo/const.py
--rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.3/snake_opencv/py.typed
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.3/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.3/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.3/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.4/LICENSE
+-rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.4/README.md
+-rw-r--r--   0        0        0      686 2023-06-08 13:22:58.795154 snake_opencv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.4/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.4/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.4/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.4/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.4/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.4/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.4/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.4/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.4/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.4/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.4/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.4/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.4/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.4/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    43838 2023-06-08 13:21:35.366342 snake_opencv-0.1.4/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.4/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.4/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.4/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.4/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.4/snake_opencv/py.typed
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.4/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.4/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.4/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.4/PKG-INFO
```

### Comparing `snake_opencv-0.1.3/LICENSE` & `snake_opencv-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/pyproject.toml` & `snake_opencv-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.3"
+version = "0.1.4"
 repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
```

### Comparing `snake_opencv-0.1.3/snake_opencv/core/binding.py` & `snake_opencv-0.1.4/snake_opencv/core/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/core/const.py` & `snake_opencv-0.1.4/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/dnn/binding.py` & `snake_opencv-0.1.4/snake_opencv/dnn/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/dnn/const.py` & `snake_opencv-0.1.4/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/highgui/binding.py` & `snake_opencv-0.1.4/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/highgui/const.py` & `snake_opencv-0.1.4/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/imgcodecs/binding.py` & `snake_opencv-0.1.4/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/imgcodecs/const.py` & `snake_opencv-0.1.4/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/imgproc/binding.py` & `snake_opencv-0.1.4/snake_opencv/imgproc/binding.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     'match_template',
     'warp_affine',
     'get_affine_transform',
     'get_rotation_matrix_2d',
     'median_blur',
     'blur',
     'bilateral_filter',
+    'point_polygon_test',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
-
 Width = int
 Height = int
 
 
 def resize(
     src: np.ndarray,
     dsize: Optional[Tuple[Width, Height]] = None,
@@ -1188,7 +1188,35 @@
         src,
         d=d,
         sigmaColor=sigma_color,
         sigmaSpace=sigma_space,
         dst=dst,
         borderType=border_type,
     )
+
+
+def point_polygon_test(
+    contour: np.ndarray,
+    pt: Point2f,
+    measure_dist: bool,
+) -> float:
+    """Performs a point-in-contour test.
+
+    The function determines whether the point is inside a contour, outside, or
+    lies on an edge (or coincides with a vertex). It returns positive (inside),
+    negative (outside), or zero (on an edge) value, correspondingly. When
+    measureDist=false , the return value is +1, -1, and 0, respectively.
+    Otherwise, the return value is a signed distance between the point and the
+    nearest contour edge.
+
+    See below a sample output of the function where each image pixel is tested
+    against the contour:
+
+    Args:
+        contour: Input contour.
+        pt: Point tested against the contour.
+        measure_dist:
+            If true, the function estimates the signed distance from the point
+            to the nearest contour edge. Otherwise, the function only checks if
+            the point is inside a contour or not.
+    """
+    return cv2.pointPolygonTest(contour, pt, measure_dist)  # type: ignore
```

### Comparing `snake_opencv-0.1.3/snake_opencv/imgproc/const.py` & `snake_opencv-0.1.4/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/photo/binding.py` & `snake_opencv-0.1.4/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/photo/const.py` & `snake_opencv-0.1.4/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/videoio/binding.py` & `snake_opencv-0.1.4/snake_opencv/videoio/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/snake_opencv/videoio/const.py` & `snake_opencv-0.1.4/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.3/PKG-INFO` & `snake_opencv-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.3
+Version: 0.1.4
 Summary: Snake case opencv with type annotations
 Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

