# Comparing `tmp/hdlib-0.1.4.tar.gz` & `tmp/hdlib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.4.tar", last modified: Thu Jun  1 16:20:08 2023, max compression
+gzip compressed data, was "hdlib-0.1.5.tar", last modified: Fri Jun  9 04:36:59 2023, max compression
```

## Comparing `hdlib-0.1.4.tar` & `hdlib-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.356872 hdlib-0.1.4/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.4/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     9027 2023-06-01 16:20:08.355404 hdlib-0.1.4/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     8393 2023-06-01 16:15:34.000000 hdlib-0.1.4/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.157300 hdlib-0.1.4/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-01 13:34:35.000000 hdlib-0.1.4/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.4/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)     2241 2023-06-01 14:42:50.000000 hdlib-0.1.4/hdlib/parser.py
--rw-r--r--   0 fabio      (501) staff       (20)    20192 2023-06-01 15:29:21.000000 hdlib-0.1.4/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.309007 hdlib-0.1.4/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     9027 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      280 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       14 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-01 16:20:08.357214 hdlib-0.1.4/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.4/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.331489 hdlib-0.1.4/test/
--rw-r--r--   0 fabio      (501) staff       (20)     6578 2023-05-31 23:16:43.000000 hdlib-0.1.4/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.328309 hdlib-0.1.5/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.5/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     1713 2023-06-09 04:36:59.327566 hdlib-0.1.5/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     1079 2023-06-09 01:35:38.000000 hdlib-0.1.5/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.279552 hdlib-0.1.5/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      101 2023-06-07 18:33:03.000000 hdlib-0.1.5/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.5/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    14629 2023-06-09 01:49:03.000000 hdlib-0.1.5/hdlib/model.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.5/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.5/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.293772 hdlib-0.1.5/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     1713 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       14 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-09 04:36:59.328498 hdlib-0.1.5/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.5/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.325661 hdlib-0.1.5/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     6580 2023-06-08 21:35:23.000000 hdlib-0.1.5/test/test.py
```

### Comparing `hdlib-0.1.4/LICENSE` & `hdlib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.4/hdlib/arithmetic.py` & `hdlib-0.1.5/hdlib/arithmetic.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.4/hdlib/parser.py` & `hdlib-0.1.5/hdlib/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 """
 Utility to parse input files
 """
 
 import errno
 import os
+import random
 from typing import List, Tuple
 
 import numpy as np
 
 
 def load_dataset(
     filepath: os.path.abspath,
     sep: str="\t"
-) -> Tuple[List[str], List[List[float]], List[str], float, float]:
+) -> Tuple[List[str], List[List[float]], List[str]]:
     """
     Load the input dataset
 
     :param filepath:    Path to the input dataset
     :param sep:         Field separator
-    :return:            The list of sample IDs, the list of features, the content as list of lists, 
-                        and the list of classes, in addition to the minimum and maximum value
+    :return:            The list of sample IDs, the list of features, the content as list of lists, and the list of classes
     """
 
     if not os.path.isfile(filepath):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), filepath)
 
     samples = list()
     content = list()
     classes = list()
 
-    # Search for global minimum and maximum values
-    global_min = np.Inf
-    global_max = np.NINF
-
     with open(filepath) as infile:
         # Trip the first and last column out
         features = infile.readline().rstrip().split(sep)[1:-1]
 
         for line in infile:
             line = line.strip()
 
@@ -47,35 +43,48 @@
                 samples.append(line_split[0])
 
                 row_data = [float(value) for value in line_split[1:-1]]
 
                 # Add row
                 content.append(row_data)
 
-                local_min = min(row_data)
-
-                if local_min < global_min:
-                    global_min = local_min
-                
-                local_max = max(row_data)
-
-                if local_max > global_max:
-                    global_max = local_max
-
                 # Take track of the class
                 classes.append(line_split[-1])
 
-    return samples, features, content, classes, global_min, global_max
+    return samples, features, content, classes
 
 
-def split_dataset(points: int, folds: int) -> List[List[int]]:
+def kfolds_split(points: int, folds: int) -> List[List[int]]:
     """
     Given a number of data points and the number of folds, split a dataset into different folds
 
     :param points:  Number of data points
     :param folds:   Number of folds
-    :return:        List of lists with the indeces of data points
+    :return:        List of lists with the indices of data points
     """
 
+    if folds > points:
+        raise ValueError("The number of folds cannot exceed the number of data points")
+
     data_points = list(range(points))
 
     return [data_points[i::folds] for i in range(folds)]
+
+
+def percentage_split(points: int, percentage: float) -> List[int]:
+    """
+    Given a number of data points and a percentage number, split a dataset in two and report
+    the indices of the smallest set
+
+    :param points:      Number of data points
+    :param percentage:  Percentage split
+    :return:            List with indices of the smallest set after split
+    """
+
+    if percentage <= 0.0 or percentage > 100.0:
+        raise ValueError("Percentage must be greater than 0 and lower than or equal to 100")
+
+    select_points = percentage * points / 100.0
+
+    random.seed(0)
+
+    return random.sample(list(range(points)), int(select_points))
```

### Comparing `hdlib-0.1.4/hdlib/space.py` & `hdlib-0.1.5/hdlib/space.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 Implementation of hyperdimensional Vector and Space
 """
 
 import errno
 import os
 import pickle
 import uuid
+from typing import List, Optional, Set, Tuple, Union
 
 import numpy as np
-from typing import List, Optional, Set, Tuple, Union
 
 from hdlib import __version__
 
 
 class Vector(object):
     """
     Vector object
     """
 
     def __init__(
         self,
         name: Optional[str]=None,
         size: int=10000,
         vector: Optional[np.ndarray]=None,
-        vtype: Optional[str]="bipolar",
+        vtype: str="bipolar",
         tags: Optional[Set[Union[str, int, float]]]=None,
         seed: Optional[int]=None,
         warning: bool=False,
         from_file: Optional[os.path.abspath]=None,
     ) -> "Vector":
         """
         Initialize a Vector object
@@ -54,15 +54,15 @@
                 name = str(name)
 
             self.name = name
 
         except:
             raise TypeError("Vector name must be instance of a primitive")
 
-        # Register random seed for reproducibility 
+        # Register random seed for reproducibility
         self.seed = seed
 
         # Take track of the hdlib version
         self.version = __version__
 
         if tags and not isinstance(tags, set):
             raise TypeError("Tags must be a set")
@@ -122,20 +122,20 @@
                 raise TypeError("Vector size must be an integer number")
 
             if size < 10000:
                 raise ValueError("Vector size must be greater than or equal to 10000")
 
             self.size = size
 
-            # Add vector type
-            self.vtype = vtype.lower()
-
             if vtype not in ("bipolar", "binary"):
                 raise ValueError("Vector type can be binary or bipolar only")
 
+            # Add vector type
+            self.vtype = vtype.lower()
+
             if seed is None:
                 rand = np.random
 
             else:
                 # Conditions on random seed for reproducibility
                 # numpy allows integers as random seeds
                 if not isinstance(seed, int):
@@ -223,14 +223,74 @@
         if self.vtype not in ("bipolar", "binary"):
             raise Exception("Vector type is not supported")
 
         self.vector[self.vector > 0] = 1
 
         self.vector[self.vector <= 0] = 0 if self.vtype == "binary" else -1
 
+    def bind(self, vector: "Vector") -> None:
+        """
+        Bind vectors inplace
+        Refer to hdlib.arithmetic.bind
+
+        :param vector:  Vector object
+        """
+
+        # Import arithmetic.bind here to avoid circular imports
+        from hdlib.arithmetic import bind as bind_operator
+
+        self.__override_object(bind_operator(self, vector))
+
+    def bundle(self, vector: "Vector") -> None:
+        """
+        Bundle vectors inplace
+        Refer to hdlib.arithmetic.bundle
+
+        :param vector:  Vector object
+        """
+
+        # Import arithmetic.bundle here to avoid circular imports
+        from hdlib.arithmetic import bundle as bundle_operator
+
+        self.__override_object(bundle_operator(self, vector))
+    
+    def permute(self, rotate_by: int=1) -> None:
+        """
+        Permute vector inplace
+        Refer to hdlib.arithmetic.permute
+
+        :param rotate_by:   How many rotations
+        """
+
+        # Import arithmetic.permute here to avoid circular imports
+        from hdlib.arithmetic import permute as permute_operator
+
+        self.__override_object(permute_operator(self, rotate_by=rotate_by))
+
+    def __override_object(self, vector: "Vector") -> None:
+        """
+        Override the Vector object with another Vector object
+        This is a private method
+
+        :param vector:  Vector object
+        """
+
+        self.name = vector.name
+        self.size = vector.size
+        self.seed = vector.seed
+        self.tags = vector.tags
+
+        self.parent = vector.parent
+        self.children = vector.children
+
+        self.vtype = vector.vtype
+        self.vector = vector.vector
+
+        self.version = vector.version
+
     def dump(self, to_file: Optional[os.path.abspath]=None) -> None:
         """
         Dump the hyperdimensional vector to a pickle file
 
         :param to_file:     Path to the output pickle file
         """
 
@@ -246,15 +306,15 @@
 
 
 class Space(object):
     """
     Vectors space
     """
 
-    def __init__(self, size: int=10000, vtype: Optional[str]="bipolar", from_file: Optional[os.path.abspath]=None) -> "Space":
+    def __init__(self, size: int=10000, vtype: str="bipolar", from_file: Optional[os.path.abspath]=None) -> "Space":
         """
         Initialize the vectors space as a dictionary of Vector objects
 
         :param size:        Size of vectors in the space
         :param vtype:       Vector type: bipolar or binary
         :param from_file:   Load a space from pickle file
         :return:            A Space object
```

### Comparing `hdlib-0.1.4/setup.py` & `hdlib-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.4/test/test.py` & `hdlib-0.1.5/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Unit tests for hdlib/space.py:Space class
         """
 
         # Create a Space object
         space = Space(vtype="bipolar")
 
         # Add 1000 vectors
-        space.bulkInsert(list(range(1000)))
+        space.bulk_insert(list(range(1000)))
 
         # Retrieve vector 0 and 1
         # Vector names are automatically converted to strings
         vectors = space.get(names=[0, 1])
 
         with self.subTest():
             # Test the vector type: both vectors must be bipolar here
@@ -151,15 +151,15 @@
             "NAM", "CAP", "MON", # Features
             "USA", "WDC", "DOL", # United States of America
             "MEX", "MXC", "PES"  # Mexico
         ]
 
         # Build a random bipolar vector for each feature and country information
         # Add vectors to the space
-        space.bulkInsert(names)
+        space.bulk_insert(names)
 
         # Encode USA information in a single vector
         # USTATES = [(NAM * USA) + (CAP * WDC) + (MON * DOL)]
         ustates_nam = bind(space.get(names=["NAM"])[0], space.get(names=["USA"])[0]) # Bind NAM with USA
         ustates_cap = bind(space.get(names=["CAP"])[0], space.get(names=["WDC"])[0]) # Bind CAP with WDC
         ustates_mon = bind(space.get(names=["MON"])[0], space.get(names=["DOL"])[0]) # Bind MON with DOL
         ustates = bundle(bundle(ustates_nam, ustates_cap), ustates_mon) # Bundle ustates_nam, ustates_cap, and ustates_mon
```

