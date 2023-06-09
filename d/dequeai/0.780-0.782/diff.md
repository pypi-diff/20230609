# Comparing `tmp/dequeai-0.780.tar.gz` & `tmp/dequeai-0.782.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.780.tar", last modified: Fri May 12 17:14:50 2023, max compression
+gzip compressed data, was "dequeai-0.782.tar", last modified: Fri Jun  9 20:57:39 2023, max compression
```

## Comparing `dequeai-0.780.tar` & `dequeai-0.782.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:14:50.845109 dequeai-0.780/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-12 17:14:50.845109 dequeai-0.780/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:14:50.845109 dequeai-0.780/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.780/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.780/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.780/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.780/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.780/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    30266 2023-05-12 17:14:03.000000 dequeai-0.780/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.780/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.780/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.780/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.780/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:14:50.845109 dequeai-0.780/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-12 17:14:50.000000 dequeai-0.780/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 17:14:50.000000 dequeai-0.780/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 17:14:50.000000 dequeai-0.780/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 17:14:50.000000 dequeai-0.780/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 17:14:50.000000 dequeai-0.780/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 17:14:50.845109 dequeai-0.780/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-12 17:14:38.000000 dequeai-0.780/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 20:57:39.043174 dequeai-0.782/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.782/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14780 2023-06-09 20:56:38.000000 dequeai-0.782/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.782/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.782/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.782/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    30266 2023-05-12 17:14:03.000000 dequeai-0.782/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.782/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.782/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.782/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.782/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-09 20:57:39.000000 dequeai-0.782/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 20:57:39.043174 dequeai-0.782/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-09 20:57:25.000000 dequeai-0.782/setup.py
```

### Comparing `dequeai-0.780/dequeai/datatypes.py` & `dequeai-0.782/dequeai/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,95 @@
 from PIL import Image as PILImage
 import PIL
 import pickle
 import json
 import time
 import dequeai.util as util
 import numpy as np
-from dequeai.util import DEQUE_IMAGE,DEQUE_HISTOGRAM,DEQUE_AUDIO, DEQUE_TEXT, DEQUE_TABLE, DEQUE_VIDEO, DEQUE_BOUNDING_BOX, DEQUE_PLOT
+from dequeai.util import DEQUE_IMAGE, DEQUE_HISTOGRAM, DEQUE_AUDIO, DEQUE_TEXT, DEQUE_TABLE, DEQUE_VIDEO, \
+    DEQUE_BOUNDING_BOX, DEQUE_PLOT
 from dequeai.util import *
 #import altair
 
+
 class BoundingBox2D():
     _type = DEQUE_BOUNDING_BOX
+
     def __init__(self, coordinates, domain=None, scores=None, caption=None):
         self.coordinates = coordinates
         if domain is None:
             self.domain = "relative"
         else:
             self.domain = domain
         self.scores = scores
         self.caption = caption
 
-
     def _validate(self):
         pass
 
     def to_json(self):
-        return {"coordinates":self.coordinates,"domain":self.domain,"scores":self
-                .scores,"caption":self.caption}
+        return {"coordinates": self.coordinates, "domain": self.domain, "scores": self
+            .scores, "caption": self.caption}
 
 
 class Image:
     _type = DEQUE_IMAGE
 
     def __init__(self, data, box_data=None, mode=None):
         self._images = []
-        self._box_data = None
+        self._box_data = []
 
         if isinstance(data, list):
             if len(data) == 0:
                 raise ValueError("Empty list. The list must have one or more images of type numpy, tensor or pil")
 
             if box_data is not None:
-                raise ValueError(
-                    "Bounding boxes cannot be set with data of array type. In order to use bounding box, "
-                    "please pass data of type pil image, tensor or numpy array")
-
-            for d in data:
-                if isinstance(data, PILImage.Image):
-                    self._images.append(d)
-                    # print("I am PIL image")
-                elif util.is_type_torch_tensor(util.get_full_typename(data)):
-                    torch_module = util.get_module(
-                        "torch", "torch is required to render images"
-                    )
-                    _image = self._tensor_to_pil_image(torch_module=torch_module, pic=d, mode=mode)
-                    self._images.append(_image)
-                    # print("I used to be tensor image")
-                else:
-                    if hasattr(d, "numpy"):  # TF data eager tensors
-                        d = d.numpy()
-                    if d.ndim > 2:
-                        d = d.squeeze()  # get rid of trivial dimensions as a convenience
-                    _image = PILImage.fromarray(
-                        self.to_uint8(d), mode=mode or self.guess_mode(d)
-                    )
-                    self._images.append(_image)
-                    # print("I used to be numpy image")
-
+                if not isinstance(box_data, list) or not all(isinstance(b, list) for b in box_data):
+                    raise ValueError(
+                        "Bounding boxes must be a list of list of BoundingBox2d objects, one list for each image")
+                if len(data) != len(box_data):
+                    raise ValueError("Number of images and bounding box lists must be the same")
+
+            for i, d in enumerate(data):
+                self._process_image(d, mode)
+
+                if box_data is not None:
+                    for b in box_data[i]:
+                        if not isinstance(b, BoundingBox2D):
+                            raise ValueError("All elements in box_data list must be BoundingBox2d objects")
+                    self._box_data.append(box_data[i])
         else:
-            if isinstance(data, PILImage.Image):
-                self._images.append(data)
-                # print("I am PIL image")
-            elif util.is_type_torch_tensor(util.get_full_typename(data)):
-                torch_module = util.get_module(
-                    "torch", "torch is required to render images"
-                )
-                self._images.append(self._tensor_to_pil_image(torch_module=torch_module, pic=data, mode=mode))
-                # print("I used to be tensor image")
-            else:
-                if hasattr(data, "numpy"):  # TF data eager tensors
-                    data = data.numpy()
-                if data.ndim > 2:
-                    data = data.squeeze()  # get rid of trivial dimensions as a convenience
-                self._images.append(PILImage.fromarray(
-                    self.to_uint8(data), mode=mode or self.guess_mode(data)
-                ))
-
-        if box_data is not None:
-            if not isinstance(box_data, list):
-                raise ValueError("box_data must be a list of BoundingBox2d objects")
-            for b in box_data:
-                if not isinstance(b, BoundingBox2D):
-                    raise ValueError("box_data array must have BoundingBox2d objects")
+            self._process_image(data, mode)
+
+            if box_data is not None:
+                if not isinstance(box_data, list):
+                    raise ValueError("box_data must be a list of BoundingBox2d objects")
+                for b in box_data:
+                    if not isinstance(b, BoundingBox2D):
+                        raise ValueError("All elements in box_data list must be BoundingBox2d objects")
+                self._box_data.append(box_data)
 
-        self._box_data = box_data
         self._validate_size()
 
+    def _process_image(self, d, mode):
+        if isinstance(d, PILImage.Image):
+            self._images.append(d)
+        elif util.is_type_torch_tensor(util.get_full_typename(d)):
+            torch_module = util.get_module(
+                "torch", "torch is required to render images"
+            )
+            self._images.append(self._tensor_to_pil_image(torch_module=torch_module, pic=d, mode=mode))
+        else:
+            if hasattr(d, "numpy"):  # TF data eager tensors
+                d = d.numpy()
+            if d.ndim > 2:
+                d = d.squeeze()  # get rid of trivial dimensions as a convenience
+            self._images.append(PILImage.fromarray(
+                self.to_uint8(d), mode=mode or self.guess_mode(d)
+            ))
 
     def _validate_size(self):
         pass
 
     def _tensor_to_pil_image(self, torch_module, pic, mode):
 
         if not (isinstance(pic, torch_module.Tensor) or isinstance(pic, np.ndarray)):
@@ -242,20 +232,20 @@
         histogram: ([int]) number of elements falling in each bin
     """
 
     MAX_LENGTH: int = 512
     _type = DEQUE_HISTOGRAM
 
     def __init__(
-        self,
+            self,
 
-        np_histogram=None,
+            np_histogram=None,
 
     ):
-       if np_histogram:
+        if np_histogram:
             if len(np_histogram) == 2:
                 self._histogram = (
                     np_histogram[0].tolist()
                     if hasattr(np_histogram[0], "tolist")
                     else np_histogram[0]
                 )
                 self._bins = (
@@ -264,194 +254,191 @@
                     else np_histogram[1]
                 )
             else:
                 raise ValueError(
                     "Expected np_histogram to be a tuple of (values, bin_edges) or sequence to be specified"
                 )
 
-       if len(self._histogram) > self.MAX_LENGTH:
+        if len(self._histogram) > self.MAX_LENGTH:
             raise ValueError(
                 "The maximum length of a histogram is %i" % self.MAX_LENGTH
             )
-       if len(self._histogram) + 1 != len(self._bins):
+        if len(self._histogram) + 1 != len(self._bins):
             raise ValueError("len(bins) must be len(histogram) + 1")
 
-
-
     @classmethod
     def from_sequence(cls, sequence, num_bins):
         np = util.get_module(
             "numpy", required="Auto creation of histograms requires numpy"
         )
 
         np_histogram = np.histogram(sequence, bins=num_bins)
 
-        #histogram = np_histogram.tolist()
-
+        # histogram = np_histogram.tolist()
 
-        #if len(histogram) > cls.MAX_LENGTH:
-            #raise ValueError(
-               #"The maximum length of a histogram is %i" % cls.MAX_LENGTH
-            #)
-        #if len(histogram) + 1 != len(bins):
-            #raise ValueError("len(bins) must be len(histogram) + 1")
+        # if len(histogram) > cls.MAX_LENGTH:
+        # raise ValueError(
+        # "The maximum length of a histogram is %i" % cls.MAX_LENGTH
+        # )
+        # if len(histogram) + 1 != len(bins):
+        # raise ValueError("len(bins) must be len(histogram) + 1")
 
         return cls(np_histogram=np_histogram)
 
+
 class Audio:
     _type = DEQUE_AUDIO
+
     def __init__(self, data, sample_rate=None, caption=None):
         """Accepts a path to an audio file or a numpy array of audio data."""
 
         self._duration = None
         self._sample_rate = sample_rate
         self._caption = caption
 
-
         if sample_rate is None:
-                raise ValueError(
-                    'Argument "sample_rate" is required when instantiating deque.Audio with raw data.'
-                )
-
+            raise ValueError(
+                'Argument "sample_rate" is required when instantiating deque.Audio with raw data.'
+            )
 
         self._validate_size()
         self._data = data
 
     def _validate_size(self):
         pass
+
+
 class Video:
     _type = DEQUE_VIDEO
 
+
 class Text:
     _type = DEQUE_TEXT
 
 
-
 class Table:
     _type = DEQUE_TABLE
 
     '''
     'col1': [1, 2], 'col2': [3, 4]}
     >>> df = pd.DataFrame(data=d)
     >>> df
        col1  col2
     0     1     3
     1     2     4
 
-    
-    '''
 
+    '''
 
     '''
-    
+
     df2 = pd.DataFrame(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
     ...                    columns=['a', 'b', 'c'])
     >>> df2
        a  b  c
     0  1  2  3
     1  4  5  6
     2  7  8  9
     '''
 
     '''
-    
+
     Constructing DataFrame from a numpy ndarray that has labeled columns:
     >>> data = np.array([(1, 2, 3), (4, 5, 6), (7, 8, 9)],
     ...                 dtype=[("a", "i4"), ("b", "i4"), ("c", "i4")])
     >>> df3 = pd.DataFrame(data, columns=['c', 'a'])
     ...
     >>> df3
        c  a
     0  3  1
     1  6  4
     2  9  7
-    
-    
+
+
     '''
 
     def __init__(self, data, columns=None):
         self._data = data
-        self._columns=columns
+        self._columns = columns
         self._validate_data(data)
         self._validate_columns(columns)
 
     def _validate_data(self, data):
 
         if not isinstance(data, list):
             raise TypeError("data argument must be a list (rows) of list (column values)")
 
         for row in data:
             if not isinstance(row, list):
                 raise TypeError("data argument must be a list (rows) of list (column values)")
 
             for column_val in row:
-                if not isinstance(column_val,(Image,Audio,Video,Text,Histogram)) and not column_val.__class__.__module__ == 'builtins':
+                if not isinstance(column_val, (
+                Image, Audio, Video, Text, Histogram)) and not column_val.__class__.__module__ == 'builtins':
                     print("checking whether it is builtin datatype")
                     print(column_val.__class__.__module__)
                     print("checking whether it is deque datatype")
-                    print(isinstance(column_val,(Image,Audio,Video,Text,Histogram)))
+                    print(isinstance(column_val, (Image, Audio, Video, Text, Histogram)))
                     raise TypeError("Each column value must be a deque datatype or a builtin python type")
 
-
     def _validate_columns(self, columns):
         pass
-'''
+
+
 class Plot:
     _type = DEQUE_PLOT
 
-    def __init__(self, data: Table=None, altair_chart=None,plot_type=BAR, plot_attributes=None):
+    def __init__(self, data: Table = None, altair_chart=None, plot_type=BAR, plot_attributes=None):
 
-        self._data=data
+        self._data = data
         self._altair_chart = altair_chart
 
-        self._plot_type=plot_type
+        self._plot_type = plot_type
         self._plot_attributes = plot_attributes
         self._validate_plot()
         if self._altair_chart is not None:
             self._vega_json = self._read_vega_json()
         else:
             self._vega_json = None
 
-
     def _validate_plot(self):
         if self._altair_chart is None and self._data is None:
             raise ValueError("Plot needs either a Deque Table or an Altair chart to initialize")
 
     def _read_vega_json(self):
 
-        js_rep = self._altair_chart.properties(background="#61537B").to_json()
+        js_rep = self._altair_chart.to_json()
         return js_rep
 
     def to_vega_json(self):
         return self._vega_json
 
     def to_json(self):
         return {"data":self._data,"plot_type":self._plot_type,"plot_attributes":self._plot_attributes,"vega_json":self._vega_json,"datatype":Plot._type}
-'''
 
 if __name__ == "__main__":
-    #bins = [0,1, 2, 3]
-    #h = np.histogram([1,2,1], bins=bins)
+    # bins = [0,1, 2, 3]
+    # h = np.histogram([1,2,1], bins=bins)
     import matplotlib.pyplot as plt
 
-    #plt.hist(h)
-    #plt.hist(h, bins=bins)
-    #plt.show()
-    #dh = Histogram(np_histogram=h)
-    #dh=Histogram.from_sequence(sequence=[0,2,1], num_bins=[0,1,2,3])
-    import altair as alt
+    # plt.hist(h)
+    # plt.hist(h, bins=bins)
+    # plt.show()
+    # dh = Histogram(np_histogram=h)
+    # dh=Histogram.from_sequence(sequence=[0,2,1], num_bins=[0,1,2,3])
+    #import altair as alt
     import pandas as pd
 
     source = pd.DataFrame({
         'a': ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I'],
         'b': [28, 55, 43, 91, 81, 53, 19, 87, 52]
     })
 
-    chart = alt.Chart(source).mark_bar().encode(
-        x='a',
-        y='b'
-    )
+    #chart = alt.Chart(source).mark_bar().encode(
+     #   x='a',
+     #   y='b'
+    #)
 
-    #pl =Plot(altair_chart=chart)
+    #pl = Plot(altair_chart=chart)
     #print(pl.to_vega_json())
```

### Comparing `dequeai-0.780/dequeai/dequeai.py` & `dequeai-0.782/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.780/dequeai/dequeai_run.py` & `dequeai-0.782/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.780/dequeai/parsing_service.py` & `dequeai-0.782/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.780/dequeai/rest_connect.py` & `dequeai-0.782/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.780/dequeai/util.py` & `dequeai-0.782/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.780/setup.py` & `dequeai-0.782/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000780',
+    version='0.00000782',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

