# Comparing `tmp/openvisuspy-1.0.8-py3-none-any.whl.zip` & `tmp/openvisuspy-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25340 bytes, number of entries: 15
+Zip file size: 25378 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      239 b- defN 23-May-08 21:22 openvisuspy/__init__.py
 -rw-r--r--  2.0 unx     3757 b- defN 23-May-08 21:22 openvisuspy/app.py
--rw-r--r--  2.0 unx     6056 b- defN 23-May-11 00:04 openvisuspy/backend.py
+-rw-r--r--  2.0 unx     6094 b- defN 23-Jun-07 21:42 openvisuspy/backend.py
 -rw-r--r--  2.0 unx     7093 b- defN 23-May-08 21:22 openvisuspy/backend_cpp.py
 -rw-r--r--  2.0 unx    11577 b- defN 23-May-08 21:22 openvisuspy/backend_py.py
 -rw-r--r--  2.0 unx     4417 b- defN 23-May-08 21:22 openvisuspy/canvas.py
 -rw-r--r--  2.0 unx     6690 b- defN 23-May-31 20:01 openvisuspy/slice.py
 -rw-r--r--  2.0 unx     1498 b- defN 23-May-08 21:22 openvisuspy/slices.py
 -rw-r--r--  2.0 unx     7249 b- defN 23-May-08 21:22 openvisuspy/utils.py
--rw-r--r--  2.0 unx    16756 b- defN 23-May-31 23:10 openvisuspy/widgets.py
--rwxrwxrwx  2.0 unx     1849 b- defN 23-Jun-01 00:08 openvisuspy-1.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2982 b- defN 23-Jun-01 00:08 openvisuspy-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 00:08 openvisuspy-1.0.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       12 b- defN 23-Jun-01 00:08 openvisuspy-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1195 b- defN 23-Jun-01 00:08 openvisuspy-1.0.8.dist-info/RECORD
-15 files, 71462 bytes uncompressed, 23384 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx    16712 b- defN 23-Jun-07 18:10 openvisuspy/widgets.py
+-rwxrwxrwx  2.0 unx     1849 b- defN 23-Jun-08 06:07 openvisuspy-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3099 b- defN 23-Jun-08 06:07 openvisuspy-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 06:07 openvisuspy-1.0.9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       12 b- defN 23-Jun-08 06:07 openvisuspy-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 23-Jun-08 06:07 openvisuspy-1.0.9.dist-info/RECORD
+15 files, 71573 bytes uncompressed, 23422 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openvisuspy/utils.py
 Comment: 
 
 Filename: openvisuspy/widgets.py
 Comment: 
 
-Filename: openvisuspy-1.0.8.dist-info/LICENSE
+Filename: openvisuspy-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: openvisuspy-1.0.8.dist-info/METADATA
+Filename: openvisuspy-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: openvisuspy-1.0.8.dist-info/WHEEL
+Filename: openvisuspy-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: openvisuspy-1.0.8.dist-info/top_level.txt
+Filename: openvisuspy-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: openvisuspy-1.0.8.dist-info/RECORD
+Filename: openvisuspy-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openvisuspy/backend.py

```diff
@@ -43,15 +43,16 @@
 	def createBoxQuery(self,
 		timestep=None, 
 		field=None, 
 		logic_box=None,
 		max_pixels=None, 
 		endh=None, 
 		num_refinements=1, 
-		aborted=None
+		aborted=None,
+		full_dim=False,
 	):
 
 		pdim=self.getPointDim()
 		assert pdim==2 or pdim==3 # todo other cases?
 
 		maxh=self.getMaxResolution()
 		bitmask=self.getBitmask()
@@ -84,15 +85,15 @@
 		
 		# crop logic box
 		if True:
 			p1,p2=list(logic_box[0]),list(logic_box[1])
 			slice_dir=None
 			for I in range(pdim):
 				# *************** is a slice? *******************
-				if pdim==3 and (p2[I]-p1[I])==1:
+				if not full_dim and  pdim==3 and (p2[I]-p1[I])==1:
 					assert slice_dir is None 
 					slice_dir=I
 					p1[I]=Clamp(p1[I],0,dims[I])
 					p2[I]=p1[I]+1
 				else:
 					p1[I]=Clamp(int(math.floor(p1[I])),     0,dims[I])
 					p2[I]=Clamp(int(math.ceil (p2[I])) ,p1[I],dims[I])
```

## openvisuspy/widgets.py

```diff
@@ -7,20 +7,20 @@
 
 from bokeh.models import Select,LinearColorMapper,ColorBar,Button,Slider,TextInput,Row,Column,Div
 
 logger = logging.getLogger(__name__)
 
 PALETTES=[
 	"Greys256", 
-    "Inferno256", 
-    "Magma256", 
-    "Plasma256", 
-    "Viridis256", 
-    "Cividis256", 
-    "Turbo256"
+	"Inferno256", 
+	"Magma256", 
+	"Plasma256", 
+	"Viridis256", 
+	"Cividis256", 
+	"Turbo256"
 	] + [
 		it  for it in [
 		'colorcet.blueternary', 
 		'colorcet.coolwarm', 
 		'colorcet.cyclicgrey', 
 		'colorcet.depth', 
 		'colorcet.divbjy', 
@@ -329,19 +329,19 @@
 		logger.info(f"Widgets[{self.id}]::setTimesteps start={value[0]} end={value[-1]}")
 		self.widgets.timestep.start =  value[0]
 		self.widgets.timestep.end   =  value[-1]
 		self.widgets.timestep.step  = 1
 
 	# speedFromOption
 	def speedFromOption (self,option):
-                return (int(option[:-1]))
+				return (int(option[:-1]))
 
 	# optionFromSpeed
 	def optionFromSpeed (self,speed):
-                return (str(speed)+"x")
+		return (str(speed)+"x")
 
 	# getTimestepDelta
 	def getTimestepDelta(self):
 		return self.speedFromOption(self.widgets.timestep_delta.value)
 
 	# setTimestepDelta
 	def setTimestepDelta(self,value):
```

## Comparing `openvisuspy-1.0.8.dist-info/LICENSE` & `openvisuspy-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openvisuspy-1.0.8.dist-info/METADATA` & `openvisuspy-1.0.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvisuspy
-Version: 1.0.8
+Version: 1.0.9
 Summary: openvisuspy
 Author: OpenVisus developers
 Project-URL: Homepage, https://github.com/sci-visus/openvisuspy
 Project-URL: Bug Tracker, https://github.com/sci-visus/openvisuspy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -46,17 +46,20 @@
 
 ```
 python3 -m pip install --upgrade OpenVisus
 python3 -m OpenVisus configure 
 python3 -m pip install --upgrade openvisuspy 
 ```
 
-if you are in debugging mode you may want to reference your local packages:
+if you are in **debugging mode** you may want to reference your local packages:
 
 ```
+python3 -m pip uninstall OpenVisusNoGui
+python3 -m pip uninstall OpenVisus
+python3 -m pip uninstall openvisuspy 
 export PYTHONPATH=./src;/projects/OpenVisus/build/RelWithDebInfo
 ```
 
 # Examples
 
 ## Bokeh Dashboards
```

## Comparing `openvisuspy-1.0.8.dist-info/RECORD` & `openvisuspy-1.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 openvisuspy/__init__.py,sha256=XJQQQgf-N1nzohZPP5BHW2yFZB0ApRqELJMpioa6sow,239
 openvisuspy/app.py,sha256=L3qnxJhL6D3xCFdUjgUzZ-Blk9Ag4x-sz7HSjaGZefM,3757
-openvisuspy/backend.py,sha256=inp3MJswK7QcDFV4__zdGcJ-diWJsrOXiWp8DBkpqL4,6056
+openvisuspy/backend.py,sha256=dgb1U5zdpMZIQ0hd9eapZJMD2angChfNyjuQXYpzw6o,6094
 openvisuspy/backend_cpp.py,sha256=ZukezVcj3DikB823ZvinWDb2Tlefke5CjRoSLCDjNTw,7093
 openvisuspy/backend_py.py,sha256=B-ns-tcnhhrE9AedVS6nrVICxZjkkYkqr_oa9mBd2uk,11577
 openvisuspy/canvas.py,sha256=oa42eKl7mQSRnagJ9Kz0uG8duJV0eKaaeG8fFLE6N3A,4417
 openvisuspy/slice.py,sha256=RmemDqmuuZb8hsbt7WkrMXh2iWgx9KDqmTewaKqmcuA,6690
 openvisuspy/slices.py,sha256=ijF00q4UpLMsYC1poXVjr2ZvZM2nl5OZnLh94scjWEM,1498
 openvisuspy/utils.py,sha256=DGfo09rGiKQdB6SHJiEWmOYeMTJnxRJFNUNWPUTxmVQ,7249
-openvisuspy/widgets.py,sha256=OADksn13PktE8giInU-IVH9Ti8skz_S6mdLrVMkzWeQ,16756
-openvisuspy-1.0.8.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
-openvisuspy-1.0.8.dist-info/METADATA,sha256=IGXVfvC4isivgOjuWObCdRzO6XUo0QhyKtmPt5rFh4s,2982
-openvisuspy-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openvisuspy-1.0.8.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
-openvisuspy-1.0.8.dist-info/RECORD,,
+openvisuspy/widgets.py,sha256=bFvO7kSW7EPvAGuNf5kkA1BFqMTy-5EpO7MfMYLonfo,16712
+openvisuspy-1.0.9.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
+openvisuspy-1.0.9.dist-info/METADATA,sha256=7VeIcLVYcYTAlLA74ymDH5EG2IsuHzz86DuNMJKyBNE,3099
+openvisuspy-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openvisuspy-1.0.9.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
+openvisuspy-1.0.9.dist-info/RECORD,,
```

