# Comparing `tmp/SimpleShape-1.4.1.tar.gz` & `tmp/SimpleShape-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleShape-1.4.1.tar", last modified: Thu Jun  8 14:49:45 2023, max compression
+gzip compressed data, was "SimpleShape-1.5.tar", last modified: Fri Jun  9 15:12:38 2023, max compression
```

## Comparing `SimpleShape-1.4.1.tar` & `SimpleShape-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:49:45.560494 SimpleShape-1.4.1/
--rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.4.1/License.txt
--rw-rw-rw-   0        0        0     5052 2023-06-08 14:49:45.560494 SimpleShape-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4646 2023-06-07 10:02:13.000000 SimpleShape-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 14:49:45.544880 SimpleShape-1.4.1/SimpleShape/
--rw-rw-rw-   0        0        0      879 2023-06-08 13:20:59.000000 SimpleShape-1.4.1/SimpleShape/Example.py
--rw-rw-rw-   0        0        0    15203 2023-06-08 12:58:25.000000 SimpleShape-1.4.1/SimpleShape/SimpleShape.py
--rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.4.1/SimpleShape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:49:45.560494 SimpleShape-1.4.1/SimpleShape.egg-info/
--rw-rw-rw-   0        0        0     5052 2023-06-08 14:49:45.000000 SimpleShape-1.4.1/SimpleShape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-08 14:49:45.000000 SimpleShape-1.4.1/SimpleShape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:49:45.000000 SimpleShape-1.4.1/SimpleShape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-08 14:49:45.000000 SimpleShape-1.4.1/SimpleShape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-08 14:49:45.560494 SimpleShape-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-06-07 17:54:37.000000 SimpleShape-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:12:38.826671 SimpleShape-1.5/
+-rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.5/License.txt
+-rw-rw-rw-   0        0        0     5055 2023-06-09 15:12:38.826671 SimpleShape-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-06-09 15:00:39.000000 SimpleShape-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 15:12:38.795428 SimpleShape-1.5/SimpleShape/
+-rw-rw-rw-   0        0        0      879 2023-06-09 14:09:36.000000 SimpleShape-1.5/SimpleShape/Example.py
+-rw-rw-rw-   0        0        0    15267 2023-06-09 15:08:07.000000 SimpleShape-1.5/SimpleShape/SimpleShape.py
+-rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.5/SimpleShape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:12:38.826671 SimpleShape-1.5/SimpleShape.egg-info/
+-rw-rw-rw-   0        0        0     5055 2023-06-09 15:12:38.000000 SimpleShape-1.5/SimpleShape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-09 15:12:38.000000 SimpleShape-1.5/SimpleShape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:12:38.000000 SimpleShape-1.5/SimpleShape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 15:12:38.000000 SimpleShape-1.5/SimpleShape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-09 15:12:38.826671 SimpleShape-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      972 2023-06-09 12:31:21.000000 SimpleShape-1.5/setup.py
```

### Comparing `SimpleShape-1.4.1/License.txt` & `SimpleShape-1.5/License.txt`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.4.1/PKG-INFO` & `SimpleShape-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.4.1
+Version: 1.5
 Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,12 +80,12 @@
 - **load\_shapes(filename):** Create JSON string from a .json file
 - **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
-- **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
+- **line_intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
-- **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
+- **line_intersect_circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
 **Note: Tangency also counts as intersection!**
```

### Comparing `SimpleShape-1.4.1/README.md` & `SimpleShape-1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,12 +67,12 @@
 - **load\_shapes(filename):** Create JSON string from a .json file
 - **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
-- **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
+- **line_intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
-- **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
+- **line_intersect_circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
 **Note: Tangency also counts as intersection!**
```

### Comparing `SimpleShape-1.4.1/SimpleShape/Example.py` & `SimpleShape-1.5/SimpleShape/Example.py`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.4.1/SimpleShape/SimpleShape.py` & `SimpleShape-1.5/SimpleShape/SimpleShape.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         for element in self.coordinates:
             if len(element) != 2:
                 raise Warning("Provide 2 coordinates for each point")
     
     def __str__(self) -> str:
         """A string representation of the object"""
-        return ("The coordinates of the " + self.__class__.__name__
+        return ("The coordinates of the " + self.type
                 + " are " + str(self.coordinates))
 
     def perimeter(self) -> float:
         """Perimeter (circumference) of the object"""
         L = 0
         for i in range(len(self.coordinates)):
             L += sqrt((self.coordinates[i][0] - self.coordinates[i-1][0])**2
@@ -45,57 +45,56 @@
             s += (self.coordinates[i-1][0] * self.coordinates[i][1]
                   - self.coordinates[i][0] * self.coordinates[i-1][1])
         return abs(s/2)
             
     
     def intersect(self, other) -> bool:
         """Check if there is an intersection. This includes tangency"""
-        if self.__class__.__name__ in ('Triangle', 'Rectangle', 'Polygon'):
-            if other.__class__.__name__ in ('Triangle', 'Rectangle', 'Polygon'):
+        if self.type in ('Triangle', 'Rectangle', 'Polygon'):
+            if other.type in ('Triangle', 'Rectangle', 'Polygon'):
                 for i in range(len(self.coordinates)):
                     for j in range(len(other.coordinates)):
-                        if intersect(self.coordinates[i-1], self.coordinates[i],
+                        if line_intersect(self.coordinates[i-1], 
+                                          self.coordinates[i],
                             other.coordinates[j-1], other.coordinates[j]):
                             return True
                 return False
-            elif isinstance(other, Circle):
+            elif other.type == "Circle":
                 for i in range(len(self.coordinates)):
-                    if Line_Intersect_Circle(self.coordinates[i-1],
+                    if line_intersect_circle(self.coordinates[i-1],
                         self.coordinates[i], other.center, other.r):
                         return True
                 return False
             
-            elif isinstance(other, Ellipse):
+            elif other.type == "Ellipse":
                 return "This feature has yet to be implemented"
             else:
                 raise Warning("Invalid shape type for intersection check")
             
-        
        
-        elif self.__class__.__name__ == 'Circle':
-            if isinstance(other, Circle):
+        elif self.type == "Circle":
+            if other.type == "Circle":
                 distance = sqrt((self.center[0] - other.center[0])**2
                                 + (self.center[1] - other.center[1])**2)
                 if distance > abs(self.r - other.r): 
                     return distance <= (self.r + other.r)
                 return False
-            elif other.__class__.__name__ in ('Triangle',
-                                              'Rectangle', 'Polygon'):
+            elif other.type in ('Triangle', 'Rectangle', 'Polygon'):
                 for i in range(len(other.coordinates)):
-                    if Line_Intersect_Circle(other.coordinates[i-1],
+                    if line_intersect_circle(other.coordinates[i-1],
                         other.coordinates[i], self.center, self.r):
                         return True
                 return False
-            elif isinstance(other, Ellipse):
+            elif other.type == "Ellipse":
                 return "This feature has yet to be implemented"
             else:
                 raise Warning("Invalid shape type for intersection check")
 
     
-        elif self.__class__.__name__ == 'Ellipse':
+        elif self.type == 'Ellipse':
             return "This feature has yet to be implemented"
         else:
             raise Warning("Invalid shape type for intersection check")
             
     
     def visualize(self) -> None:
         """Visualize the object using Matplotlib module"""
@@ -119,16 +118,14 @@
 
         if (len(self.coordinates) != 3):
             raise Warning("Provide a 3x2 array or tuple")
         if parallel(a,b,b,c):
             raise Warning("Not a triangle. Try again") 
         if (a in (b, c) or b == c):
             raise Warning("Not a triangle. Try again")
-
-    
     
 class Rectangle(Geometry):
     """Insert points in clockwise or counter-clockwise direction"""
     def __init__(self, coordinates):
         super().__init__(coordinates)
         
         a = self.coordinates[0]
@@ -141,14 +138,15 @@
         cd = (c[0] - d[0], c[1] - d[1])
         da = (d[0] - a[0], d[1] - a[1])
         
         ac = sqrt((a[0] - c[0])**2 + (a[1] - c[1])**2)
         bd = sqrt((b[0] - d[0])**2 + (b[1] - d[1])**2)
 
         eps = 1e-10
+        
         if (len(self.coordinates) != 4):
             raise Warning("Provide a 4x2 array or tuple")
         if (abs(ab[0] + cd[0]) > eps or
             abs(bc[0] + da[0]) > eps or abs(ac - bd) > eps):
             raise Warning('Not a rectangle. Try again')
         if (abs(ab[1] + cd[1]) > eps or abs(bc[1] + da[1]) > eps):
             raise Warning('Not a rectangle. Try again')
@@ -158,25 +156,27 @@
 class Polygon(Geometry):
     """Insert points in specific order"""
     def __init__(self, coordinates):
         super().__init__(coordinates)
 
         if len(self.coordinates) < 3:
             raise Warning("Provide a nx2 array or tuple, where n > 2")
+        
         # Check for parallelism
         for i in range(len(self.coordinates)):
             if parallel(self.coordinates[i-1], self.coordinates[i],
                          self.coordinates[i-2], self.coordinates[i-1]):
                 raise Warning("One of the edges in polygon is 180°. Try again")
-        # Check if polygon is self intersectiong
+            
+        # Check if polygon is self intersecting
         self.is_intersected = 0
         for i in range(1, len(self.coordinates)):
             if self.is_intersected == 1: break
             for j in range(i-1):  # To not consider neighbours
-                if intersect(self.coordinates[i-1], self.coordinates[i],
+                if line_intersect(self.coordinates[i-1], self.coordinates[i],
                              self.coordinates[j-1], self.coordinates[j]):
                     if i - j != len(self.coordinates) - 1:  # No neighbours
                         self.is_intersected = 1
                         print("This polygon is not a simple polygon. The result of area() method will presumably be incorrect")
                         break
 
        
@@ -342,15 +342,15 @@
     y = sin(f) * (P1[0] - P2[0]) + cos(f) * (P1[1] - P2[1]) + P2[1]
     return [x,y]
 
 
 
 # From: https://www.geeksforgeeks.org/check-if-two-given-line-segments-intersect/
 
-def intersect(A, B, C, D):
+def line_intersect(A, B, C, D):
     
     def onSegment(p, q, r):
         if ( (q[0] <= max(p[0], r[0])) and (q[0] >= min(p[0], r[0])) and 
                (q[1] <= max(p[1], r[1])) and (q[1] >= min(p[1], r[1]))):
             return True
         return False
       
@@ -388,23 +388,30 @@
   
     return False
 
 
     
 
 def parallel(A, B, C, D):
-    if B[0] == A[0]: return (True if C[0] == D[0] else False)
-    if C[0] == D[0]: return (True if A[0] == B[0] else False)
+    
+    if A[0] == B[0]:
+        if A[1] == B[1]: return True
+        else: return (True if C[0] == D[0] else False)
+        
+    if C[0] == D[0]: 
+        if C[1] == D[1]: return True
+        else: return (True if A[0] == B[0] else False)
+        
     return (B[1] - A[1])/(B[0] - A[0]) == (D[1] - C[1])/(D[0] - C[0])
 
 # From: https://stackoverflow.com/questions/1073336/circle-line-segment-collision-detection-algorithm
 # (bobobobo answer)
 
 
-def Line_Intersect_Circle(A, B, C, r):
+def line_intersect_circle(A, B, C, r):
     d = (B[0] - A[0], B[1] - A[1])
     f = (A[0] - C[0], A[1] - C[1])
 
     a = d[0] * d[0] + d[1] * d[1]
     b = 2 * (f[0] * d[0] + f[1] * d[1])
     c = f[0] * f[0] + f[1] * f[1] - r * r
     discriminant = b * b - 4 * a * c
```

### Comparing `SimpleShape-1.4.1/SimpleShape.egg-info/PKG-INFO` & `SimpleShape-1.5/SimpleShape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.4.1
+Version: 1.5
 Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,12 +80,12 @@
 - **load\_shapes(filename):** Create JSON string from a .json file
 - **from\_json(json\_data):** Create a list of objects from a JSON string
 
 ##### Other functions:
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
-- **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
+- **line_intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
-- **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
+- **line_intersect_circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
 **Note: Tangency also counts as intersection!**
```

### Comparing `SimpleShape-1.4.1/setup.py` & `SimpleShape-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
     setup(
         
     name="SimpleShape",
-    version="1.4.1",
+    version="1.5",
     author="Tilen Žel",
     author_email="tilen.zel@gmail.com",
  
     #Small Description about module
     description="""A simple package for creating geometric objects""",
  
     # Specifying that we are using markdown file for description
```

