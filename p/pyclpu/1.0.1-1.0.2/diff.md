# Comparing `tmp/pyclpu-1.0.1.tar.gz` & `tmp/pyclpu-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.0.1.tar", last modified: Tue Jun  6 23:26:26 2023, max compression
+gzip compressed data, was "pyclpu-1.0.2.tar", last modified: Fri Jun  9 10:22:21 2023, max compression
```

## Comparing `pyclpu-1.0.1.tar` & `pyclpu-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.914511 pyclpu-1.0.1/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7118 2023-06-06 23:26:26.914511 pyclpu-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6710 2023-06-06 23:24:20.000000 pyclpu-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.898608 pyclpu-1.0.1/pyclpu/
--rw-rw-rw-   0        0        0      629 2023-06-06 23:23:32.000000 pyclpu-1.0.1/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/formats.py
--rw-rw-rw-   0        0        0    20399 2023-06-06 22:44:46.000000 pyclpu-1.0.1/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 17:11:29.000000 pyclpu-1.0.1/pyclpu/main.py
--rw-rw-rw-   0        0        0    13273 2023-06-06 23:18:44.000000 pyclpu-1.0.1/pyclpu/manager.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/s33293804.py
-drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.914511 pyclpu-1.0.1/pyclpu.egg-info/
--rw-rw-rw-   0        0        0     7118 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-06-06 23:26:26.914511 pyclpu-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2295 2023-06-06 23:25:59.000000 pyclpu-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.369091 pyclpu-1.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-09 10:22:21.369091 pyclpu-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7615 2023-06-09 10:09:34.000000 pyclpu-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.356586 pyclpu-1.0.2/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-06-09 10:21:06.000000 pyclpu-1.0.2/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    20857 2023-06-09 10:12:34.000000 pyclpu-1.0.2/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.0.2/pyclpu/main.py
+-rw-rw-rw-   0        0        0    16301 2023-06-09 09:57:04.000000 pyclpu-1.0.2/pyclpu/manager.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.0.2/pyclpu/s33293804.py
+drwxrwxrwx   0        0        0        0 2023-06-09 10:22:21.367505 pyclpu-1.0.2/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 10:22:21.000000 pyclpu-1.0.2/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-06-09 10:22:21.369091 pyclpu-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2295 2023-06-06 23:27:35.000000 pyclpu-1.0.2/setup.py
```

### Comparing `pyclpu-1.0.1/LICENSE` & `pyclpu-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.1/PKG-INFO` & `pyclpu-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -14,47 +14,69 @@
 
 **This file describes the module of CLPU utilities and related aspects to users and maintainers.**
 
 # CLPU Utilities
 
 **Abstract:** This module bundels functions which are frequently used for applications at the Centro de Laseres Pulsados, Villamayor, Spain. Although we intend to deliver reliable software solutions, we can not guarantee that every implementation is flawless. We encourage the user to re-read the code and alert us if bugs are found.
 
-The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
+:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
 
 ## Installation
 
 Run `pip install pyclpu` when connected to the internet; or if not connected to the internet `pip install .` within the main folder of the project (where you find also files like `README.md`, `setup.py`, `LICENCE`).
 
 ## Use-cases
 
 The following use cases have occured and led to debugged implementations.
 
-### Catch Autosaved Images and apply Warp Transform
+### Rename Autosaved Images and Apply Warp Transform
+
+The following code sniffes in a directory `bin` for new files by means of `image.CatchAndRename` and performs a Warp Transform by means of `image.PerspectiveTransform`. Results are stored in `bin/output_warp` if such directory exists (else in the current working directory).
 
 ```
 import os
+import numpy as np
 
 from pyclpu import image
 from pyclpu import manager
 
 chase = manager.CatchAndRename()
 
 chase.directory = "C:\\bin"
 chase.prefix = "shot_"
 chase.number = 1
 
 warp_it = image.PerspectiveTransform()
+warp = []
 
 chase.loop = True
-while True:
-    
-    
-    image.imwrite(os.path.join(chase.directory,'output_warp',chase.name)
-    
+chase.leap = True
 
+while True:
+    if chase.flag_new:
+        chase.flag_new = False
+        warp_it.source = image.imread(os.path.join(chase.directory,chase.filename))
+    if warp_it.flag_new:
+        warp_it.flag_new = False
+        image.imwrite(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                chase.filename
+            ),
+            warp_it.warped
+        )
+        np.savetxt(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                manager.strip_extension(chase.filename)+".dat"
+            ),
+            warp_it.sourcecorners.point_list
+        )
 ```
 
 ### Rename Many Files ...
 
 #### ... changing only the extension
 
 ```
```

### Comparing `pyclpu-1.0.1/README.md` & `pyclpu-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 **This file describes the module of CLPU utilities and related aspects to users and maintainers.**
 
 # CLPU Utilities
 
 **Abstract:** This module bundels functions which are frequently used for applications at the Centro de Laseres Pulsados, Villamayor, Spain. Although we intend to deliver reliable software solutions, we can not guarantee that every implementation is flawless. We encourage the user to re-read the code and alert us if bugs are found.
 
-The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
+:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
 
 ## Installation
 
 Run `pip install pyclpu` when connected to the internet; or if not connected to the internet `pip install .` within the main folder of the project (where you find also files like `README.md`, `setup.py`, `LICENCE`).
 
 ## Use-cases
 
 The following use cases have occured and led to debugged implementations.
 
-### Catch Autosaved Images and apply Warp Transform
+### Rename Autosaved Images and Apply Warp Transform
+
+The following code sniffes in a directory `bin` for new files by means of `image.CatchAndRename` and performs a Warp Transform by means of `image.PerspectiveTransform`. Results are stored in `bin/output_warp` if such directory exists (else in the current working directory).
 
 ```
 import os
+import numpy as np
 
 from pyclpu import image
 from pyclpu import manager
 
 chase = manager.CatchAndRename()
 
 chase.directory = "C:\\bin"
 chase.prefix = "shot_"
 chase.number = 1
 
 warp_it = image.PerspectiveTransform()
+warp = []
 
 chase.loop = True
-while True:
-    
-    
-    image.imwrite(os.path.join(chase.directory,'output_warp',chase.name)
-    
+chase.leap = True
 
+while True:
+    if chase.flag_new:
+        chase.flag_new = False
+        warp_it.source = image.imread(os.path.join(chase.directory,chase.filename))
+    if warp_it.flag_new:
+        warp_it.flag_new = False
+        image.imwrite(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                chase.filename
+            ),
+            warp_it.warped
+        )
+        np.savetxt(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                manager.strip_extension(chase.filename)+".dat"
+            ),
+            warp_it.sourcecorners.point_list
+        )
 ```
 
 ### Rename Many Files ...
 
 #### ... changing only the extension
 
 ```
```

### Comparing `pyclpu-1.0.1/pyclpu/__init__.py` & `pyclpu-1.0.2/pyclpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.0.1/pyclpu/constants.py` & `pyclpu-1.0.2/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.1/pyclpu/formats.py` & `pyclpu-1.0.2/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.1/pyclpu/image.py` & `pyclpu-1.0.2/pyclpu/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -400,14 +400,17 @@
     Args:
         source  (:obj: ``numpy.array``,optional) : Source image.
         sourcecorners (:obj: ``PointPicker``,optional) : Object of type `PointPicker`, i.e. `sourcecorners.point_list` is a list of shape `(4,2)` which describe the source's corner coordinates in the original image matrix;`sourcecorners.n` equals 4; and `sourcecorners.status` should return True.
     
     Attributes:
         status (bool) : True if processing was successfull, else False.
             Initializes to False.
+        flag_new (bool) : True if processing was successfull, else False.
+            Initializes to False.
+            Intended to be modified from outside in use cases where this routine delivers output for another process.
     
     Returns:
         warped  (:obj: ``numpy.array``) : Warped image.
         
     Note:
         The source image is not part of the object in its final form.
     
@@ -434,14 +437,15 @@
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
         self.status = False
+        self.flag_new = False
         # INTEGRITY
         if not hasattr(self, 'source'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `source` as `source=IMG`.")
         if not hasattr(self, 'sourcecorners'):
             warning(self.__class__.__name__,"Found no corners (x,y) of target rectangle, optional key `sourcecorners` as `sourcecorners=np.array((4,2),dtype='int')`.")
         # IN PLACE
         if hasattr(self, 'source'):
@@ -449,14 +453,15 @@
         return None
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
         if name == "source":
             self.__run__()
         return None
     def __run__(self):
+        self.status = False
         # METHODS
         def order_points(pts):
             """
             Orders automatically a list of coordinates of (rectangular) image corners as follows: top-left, top-right, bottom-right, bottom-left.
             """
             rect = np.zeros((4, 2), dtype = "float32")
             s = pts.sum(axis = 1)
@@ -488,26 +493,31 @@
                 [0, maxHeight - 1]], dtype = "float32")
             # compute perspective transform matrix and apply it
             M = cv2.getPerspectiveTransform(rect, dst)
             warped = cv2.warpPerspective(image, M, (maxWidth, maxHeight))
             # return the warped image
             return warped    
         # MAIN
+        first_warp = False
         if not hasattr(self,'sourcecorners'):
+            first_warp = True
             warning(self.__class__.__name__,"Found no corners of target rectangle, open interactive dialogue to pick them.")
             self.sourcecorners = PointPicker(image=self.source,n=4)
         self.warped = four_point_transform(self.source, self.sourcecorners.point_list)
-        message(self.__class__.__name__,"PRESS ANY KEY TO CLOSE IMAGE AND PROCEED",headline="DISPLAY WARP")
-        cv2.namedWindow(self.__class__.__name__)
-        cv2.imshow(self.__class__.__name__, self.warped)
-        cv2.waitKey(0)
+        if first_warp == True:
+            first_warp = False
+            message(self.__class__.__name__,"PRESS ANY KEY TO CLOSE IMAGE AND PROCEED",headline="DISPLAY WARP")
+            cv2.namedWindow(self.__class__.__name__)
+            cv2.imshow(self.__class__.__name__, self.warped)
+            cv2.waitKey(0)
         # housekeeping
         cv2.destroyAllWindows()
         del self.source
         self.status = True
+        self.flag_new = True
         return None
         
     
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
```

### Comparing `pyclpu-1.0.1/pyclpu/main.py` & `pyclpu-1.0.2/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.1/pyclpu/manager.py` & `pyclpu-1.0.2/pyclpu/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -138,14 +138,24 @@
     Function returns extension of a filename as string or `None`.
     """
     try:
         extension = filename.rsplit(".",1)[1]
     except:
         extension = None
     return extension
+    
+def strip_extension(filename):
+    """
+    Function returns a filename without extension as string or `None`.
+    """
+    try:
+        noextension = filename[0:-(len(give_extension(filename))+1)]
+    except:
+        noextension = None
+    return noextension
 
     
 # =============================================================================
 # CLASSES
 # =============================================================================
 # INTEGRATION AND TESTING
 class Main:
@@ -183,17 +193,29 @@
     
     Args:
         directory (str) : Path to directory where new files are expected.
         prefix (str, optional) : Prefix of renamed filename. Defaults to `""`.
         number (int, optional) : Suffix of renamed filename. Defaults to `0`.
         extension (str, optional) : Extension of renamed files. Defaults to the old extension.
         loop (bool, optional) : Activity status of the catcher. Inactive if `False`, active if `True`.
+        leap (bool) : Leaps over existing files if set True. Defaults to False. 
+            With leap = False, routine will not overwrite exisiting files and exists if an attempt is made.
+            With leap = True, routine will not overwrite exisiting files but use the next possible number, counting up.
         
     Attributes:
-        ignored (list) : List of files which is ignored 
+        filename (str) : Name of last file which was written. Initializes as empty string.
+        flag_new (bool) : True if processing was successfull, else False.
+            Initializes to False.
+            Intended to be modified from outside in use cases where this routine delivers output for another process.
+        status (bool) : True if processing was successfull, else False.
+            Initializes to False.
+        
+    Returns:
+        ident (int) : Identity of thread. If more than one thread is started, a list is created that contains the identities in chronologic order, with the newest one last.
+        ignored (list) : List of files which is ignored.
     
     Notes:
         Rename freshly arriving files to `str(prefix+number+"."+extension)` when loop is activated by setting the input parameter `loop = True`. If elements from the list `inored` are purged during `loop = True`, then corresponding files will be renamed as they are recognized as new.
         
     Examples:
         The class can be used in a functional way
         ```
@@ -222,14 +244,19 @@
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         # INPUT
         self.__dict__.update(kwargs)
         # VARIABLES
         #self.cwd = os.getcwd()
         self.timeout = 2
+        self.filename = ""
+        self.flag_new = False
+        self.status = False
+        self.leap = False
+        self.ident = None
         # INTEGRITY
         if not hasattr(self, 'loop'):
             warning(self.__class__.__name__,"Find no loop request status, expect key `loop` as boolean and start if `loop = True`.")
         # IN PLACE
         if hasattr(self, 'loop') and self.loop == True:
             self.__run__()
         return None
@@ -254,14 +281,15 @@
             self.extension = ""
         if not hasattr(self, 'prefix'):
             warning(self.__class__.__name__,"No prefix defined, expect key `prefix` as `prefix=any_string`. Set `prefix = ''`.")
             self.prefix = ""
         # METHODS
         #@classmethod
         def _worker(event):
+            self.ident = threading.get_ident()
             self.ignored = os.listdir(self.directory)
             while not self._event.is_set():
                 time.sleep(self.timeout)
                 file_list = os.listdir(self.directory)
                 for file in file_list:
                     if file in self.ignored:
                         continue
@@ -283,35 +311,64 @@
                         else:
                             new_file = self.prefix+str(self.number).zfill(3)+'.'+new_extension
                             self.number = self.number + 1
                         self.ignored.append(new_file)
                         old_name = os.path.join(self.directory,file)
                         new_name = os.path.join(self.directory,new_file)
                         if os.path.isfile(new_name):
-                            warning(self.__class__.__name__,"FILE ALREADY EXISTS: DO NOTHING FOR "+old_name)
-                            break
-                        else:
-                            message(self.__class__.__name__,"CREATE  "+new_name)
-                            os.rename(old_name, new_name)
+                            message(self.__class__.__name__,"FILE ALREADY EXISTS: "+new_name)
+                            find_next_free_number_for_pattern = self.number
+                            while True:
+                                find_next_free_number_for_pattern = find_next_free_number_for_pattern + 1
+                                test_file = self.prefix+str(find_next_free_number_for_pattern).zfill(3)+'.'+new_extension
+                                if os.path.isfile(os.path.join(self.directory,test_file)):
+                                    continue
+                                else:
+                                    break
+                            new_file = test_file
+                            new_name = os.path.join(self.directory,new_file)
+                            message(self.__class__.__name__,"FIND NEXT POSSIBLE: "+new_name)
+                            if self.leap == True:
+                                pass
+                            else:
+                                warning(self.__class__.__name__,"FILE ALREADY EXISTS: DO NOTHING FOR "+old_name)
+                                message(self.__class__.__name__,"EXIT LOOP: loop = False")
+                                self.status = False
+                                self.loop = False
+                                #break
+                        message(self.__class__.__name__,"CREATE  "+new_name)
+                        os.rename(old_name, new_name)
+                        self.filename = new_file
+                        self.flag_new = True
+                        self.status = True
         # MAIN
-        self._event = threading.Event()
-        self._process = threading.Thread(target=_worker, args=(self._event,))
+        if not hasattr(self,"_event"):
+            self._event = threading.Event()
+            self._process = threading.Thread(target=_worker, args=(self._event,))
         self.start()
     
     def start(self):
         # START
-        self._process.start()
+        if hasattr(self,"_process"):
+            self._process.start()
+        else:
+            warning(self.__class__.__name__,"THREAD ALREADY STARTED: DO NOTHING")
     
     def stop(self):
         self._event.set()
         self._process.join()
         # integrity of results
         # ..
         # housekeeping
-        # ..
+        try:
+            del self.ident
+            del self._event
+            del self._process
+        except:
+            pass
         return None
     
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
 if globals()["__name__"] == '__main__':
```

### Comparing `pyclpu-1.0.1/pyclpu/s33293804.py` & `pyclpu-1.0.2/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.0.1/pyclpu.egg-info/PKG-INFO` & `pyclpu-1.0.2/pyclpu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -14,47 +14,69 @@
 
 **This file describes the module of CLPU utilities and related aspects to users and maintainers.**
 
 # CLPU Utilities
 
 **Abstract:** This module bundels functions which are frequently used for applications at the Centro de Laseres Pulsados, Villamayor, Spain. Although we intend to deliver reliable software solutions, we can not guarantee that every implementation is flawless. We encourage the user to re-read the code and alert us if bugs are found.
 
-The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
+:paperclip: The documentation is available in both [`html`](./html/pyclpu/index.html) and [`markdown`](./md/pyclpu/index.md) format.
 
 ## Installation
 
 Run `pip install pyclpu` when connected to the internet; or if not connected to the internet `pip install .` within the main folder of the project (where you find also files like `README.md`, `setup.py`, `LICENCE`).
 
 ## Use-cases
 
 The following use cases have occured and led to debugged implementations.
 
-### Catch Autosaved Images and apply Warp Transform
+### Rename Autosaved Images and Apply Warp Transform
+
+The following code sniffes in a directory `bin` for new files by means of `image.CatchAndRename` and performs a Warp Transform by means of `image.PerspectiveTransform`. Results are stored in `bin/output_warp` if such directory exists (else in the current working directory).
 
 ```
 import os
+import numpy as np
 
 from pyclpu import image
 from pyclpu import manager
 
 chase = manager.CatchAndRename()
 
 chase.directory = "C:\\bin"
 chase.prefix = "shot_"
 chase.number = 1
 
 warp_it = image.PerspectiveTransform()
+warp = []
 
 chase.loop = True
-while True:
-    
-    
-    image.imwrite(os.path.join(chase.directory,'output_warp',chase.name)
-    
+chase.leap = True
 
+while True:
+    if chase.flag_new:
+        chase.flag_new = False
+        warp_it.source = image.imread(os.path.join(chase.directory,chase.filename))
+    if warp_it.flag_new:
+        warp_it.flag_new = False
+        image.imwrite(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                chase.filename
+            ),
+            warp_it.warped
+        )
+        np.savetxt(
+            os.path.join(
+                chase.directory,
+                'output_warp',
+                manager.strip_extension(chase.filename)+".dat"
+            ),
+            warp_it.sourcecorners.point_list
+        )
 ```
 
 ### Rename Many Files ...
 
 #### ... changing only the extension
 
 ```
```

### Comparing `pyclpu-1.0.1/setup.py` & `pyclpu-1.0.2/setup.py`

 * *Files identical despite different names*

