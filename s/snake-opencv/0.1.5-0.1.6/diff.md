# Comparing `tmp/snake_opencv-0.1.5.tar.gz` & `tmp/snake_opencv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_opencv-0.1.5.tar", max compression
+gzip compressed data, was "snake_opencv-0.1.6.tar", max compression
```

## Comparing `snake_opencv-0.1.5.tar` & `snake_opencv-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.5/LICENSE
--rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.5/README.md
--rw-r--r--   0        0        0      686 2023-06-09 12:42:10.287324 snake_opencv-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.5/snake_opencv/__init__.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.5/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.5/snake_opencv/core/binding.py
--rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.5/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.5/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.5/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.5/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.5/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.5/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.5/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.5/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.5/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.5/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.5/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    44941 2023-06-09 12:34:52.430848 snake_opencv-0.1.5/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.5/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.5/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.5/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.5/snake_opencv/photo/const.py
--rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.5/snake_opencv/py.typed
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.5/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.5/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.5/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.6/LICENSE
+-rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.6/README.md
+-rw-r--r--   0        0        0      686 2023-06-09 16:58:51.083870 snake_opencv-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.6/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.6/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.6/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.6/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.6/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.6/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.6/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.6/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.6/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.6/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.6/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.6/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.6/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.6/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    46800 2023-06-09 16:55:09.639974 snake_opencv-0.1.6/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.6/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.6/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.6/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.6/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.6/snake_opencv/py.typed
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.6/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.6/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.6/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.6/PKG-INFO
```

### Comparing `snake_opencv-0.1.5/LICENSE` & `snake_opencv-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/pyproject.toml` & `snake_opencv-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.5"
+version = "0.1.6"
 repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
```

### Comparing `snake_opencv-0.1.5/snake_opencv/core/binding.py` & `snake_opencv-0.1.6/snake_opencv/core/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/core/const.py` & `snake_opencv-0.1.6/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/dnn/binding.py` & `snake_opencv-0.1.6/snake_opencv/dnn/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/dnn/const.py` & `snake_opencv-0.1.6/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/highgui/binding.py` & `snake_opencv-0.1.6/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/highgui/const.py` & `snake_opencv-0.1.6/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/imgcodecs/binding.py` & `snake_opencv-0.1.6/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/imgcodecs/const.py` & `snake_opencv-0.1.6/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/imgproc/binding.py` & `snake_opencv-0.1.6/snake_opencv/imgproc/binding.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     'get_affine_transform',
     'get_rotation_matrix_2d',
     'median_blur',
     'blur',
     'bilateral_filter',
     'point_polygon_test',
     'contour_area',
+    'convex_hull',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
 Width = int
 Height = int
@@ -416,15 +417,15 @@
             they should be analyzed in the whole image context.
     """
     return cv2.findContours(image, mode=mode, method=method, offset=offset)  # type: ignore
 
 
 def draw_contours(
     image: np.ndarray,
-    contours: Contours,
+    contours: Union[Contours, List[np.ndarray]],
     contour_idx: int,
     color: Scalar,
     thickness: int = 1,
     line_type: LineType = 8,
     hierarchy: Optional[Hierarchy] = None,
     max_level: Optional[int] = None,
     offset: Optional[Tuple[X, Y]] = None,
@@ -1241,7 +1242,47 @@
             area value, depending on the contour orientation (clockwise or
             counter-clockwise). Using this feature you can determine
             orientation of a contour by taking the sign of an area. By default,
             the parameter is false, which means that the absolute value is
             returned.
     """
     return cv2.contourArea(contour, oriented)  # type: ignore
+
+
+def convex_hull(
+    points: np.ndarray,
+    hull: Optional[np.ndarray] = None,
+    clockwise: bool = False,
+    return_points: bool = True,
+) -> np.ndarray:
+    """Finds the convex hull of a point set.
+
+    The function cv::convexHull finds the convex hull of a 2D point set using
+    the Sklansky's algorithm [226] that has O(N logN) complexity in the current
+    implementation.
+
+    Args:
+        points: Input 2D point set, stored in std::vector or Mat.
+        hull:
+            Output convex hull. It is either an integer vector of indices or
+            vector of points. In the first case, the hull elements are 0-based
+            indices of the convex hull points in the original array (since the
+            set of convex hull points is a subset of the original point set).
+            In the second case, hull elements are the convex hull points
+            themselves.
+        clockwise:
+            Orientation flag. If it is true, the output convex hull is oriented
+            clockwise. Otherwise, it is oriented counter-clockwise. The assumed
+            coordinate system has its X axis pointing to the right, and its Y
+            axis pointing upwards.
+        return_points:
+            Operation flag. In case of a matrix, when the flag is true, the
+            function returns convex hull points. Otherwise, it returns indices
+            of the convex hull points. When the output array is std::vector,
+            the flag is ignored, and the output depends on the type of the
+            vector: std::vector<int> implies returnPoints=false,
+            std::vector<Point> implies returnPoints=true.
+
+    Note: points and hull should be different arrays, inplace processing isn't
+    supported.
+    """
+    return cv2.convexHull(points, hull, clockwise, return_points)  # type: ignore
```

### Comparing `snake_opencv-0.1.5/snake_opencv/imgproc/const.py` & `snake_opencv-0.1.6/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/photo/binding.py` & `snake_opencv-0.1.6/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/photo/const.py` & `snake_opencv-0.1.6/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/videoio/binding.py` & `snake_opencv-0.1.6/snake_opencv/videoio/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/snake_opencv/videoio/const.py` & `snake_opencv-0.1.6/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.5/PKG-INFO` & `snake_opencv-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.5
+Version: 0.1.6
 Summary: Snake case opencv with type annotations
 Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

