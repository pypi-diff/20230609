# Comparing `tmp/picmistandard-0.24.0.tar.gz` & `tmp/picmistandard-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picmistandard-0.24.0.tar", last modified: Tue Apr  4 16:16:00 2023, max compression
+gzip compressed data, was "picmistandard-0.25.0.tar", last modified: Fri Jun  9 01:13:46 2023, max compression
```

## Comparing `picmistandard-0.24.0.tar` & `picmistandard-0.25.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-04 16:16:00.696556 picmistandard-0.24.0/
--rw-r--r--   0 rlehe      (501) staff       (20)       43 2023-04-04 16:13:57.000000 picmistandard-0.24.0/MANIFEST.in
--rw-r--r--   0 rlehe      (501) staff       (20)      198 2023-04-04 16:16:00.696228 picmistandard-0.24.0/PKG-INFO
--rw-r--r--   0 rlehe      (501) staff       (20)     3305 2023-04-04 16:13:57.000000 picmistandard-0.24.0/README.md
--rw-r--r--   0 rlehe      (501) staff       (20)      234 2023-04-04 16:13:57.000000 picmistandard-0.24.0/__init__.py
--rw-r--r--   0 rlehe      (501) staff       (20)     5685 2023-04-04 16:13:57.000000 picmistandard-0.24.0/applied_fields.py
--rw-r--r--   0 rlehe      (501) staff       (20)     7917 2023-04-04 16:13:57.000000 picmistandard-0.24.0/base.py
--rw-r--r--   0 rlehe      (501) staff       (20)    10356 2023-04-04 16:13:57.000000 picmistandard-0.24.0/diagnostics.py
--rw-r--r--   0 rlehe      (501) staff       (20)    54140 2023-04-04 16:13:57.000000 picmistandard-0.24.0/fields.py
--rw-r--r--   0 rlehe      (501) staff       (20)      828 2023-04-04 16:13:57.000000 picmistandard-0.24.0/interactions.py
--rw-r--r--   0 rlehe      (501) staff       (20)     7713 2023-04-04 16:13:57.000000 picmistandard-0.24.0/lasers.py
--rw-r--r--   0 rlehe      (501) staff       (20)    21519 2023-04-04 16:13:57.000000 picmistandard-0.24.0/particles.py
-drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2023-04-04 16:16:00.695736 picmistandard-0.24.0/picmistandard.egg-info/
--rw-r--r--   0 rlehe      (501) staff       (20)      198 2023-04-04 16:16:00.000000 picmistandard-0.24.0/picmistandard.egg-info/PKG-INFO
--rw-r--r--   0 rlehe      (501) staff       (20)      378 2023-04-04 16:16:00.000000 picmistandard-0.24.0/picmistandard.egg-info/SOURCES.txt
--rw-r--r--   0 rlehe      (501) staff       (20)        1 2023-04-04 16:16:00.000000 picmistandard-0.24.0/picmistandard.egg-info/dependency_links.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       23 2023-04-04 16:16:00.000000 picmistandard-0.24.0/picmistandard.egg-info/requires.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       14 2023-04-04 16:16:00.000000 picmistandard-0.24.0/picmistandard.egg-info/top_level.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       23 2023-04-04 16:13:57.000000 picmistandard-0.24.0/requirements.txt
--rw-r--r--   0 rlehe      (501) staff       (20)       38 2023-04-04 16:16:00.696746 picmistandard-0.24.0/setup.cfg
--rw-r--r--   0 rlehe      (501) staff       (20)      620 2023-04-04 16:13:57.000000 picmistandard-0.24.0/setup.py
--rw-r--r--   0 rlehe      (501) staff       (20)     8089 2023-04-04 16:13:57.000000 picmistandard-0.24.0/simulation.py
--rw-r--r--   0 rlehe      (501) staff       (20)       23 2023-04-04 16:14:22.000000 picmistandard-0.24.0/version.py
+drwx------   0 grote1    (5613)     5613        0 2023-06-09 01:13:46.578373 picmistandard-0.25.0/
+-rw-------   0 grote1    (5613)     5613       43 2022-08-31 01:00:06.000000 picmistandard-0.25.0/MANIFEST.in
+-rw-------   0 grote1    (5613)     5613      171 2023-06-09 01:13:46.577849 picmistandard-0.25.0/PKG-INFO
+-rw-------   0 grote1    (5613)     5613     3305 2023-04-19 20:15:44.000000 picmistandard-0.25.0/README.md
+-rw-------   0 grote1    (5613)     5613      234 2023-04-19 20:15:44.000000 picmistandard-0.25.0/__init__.py
+-rw-------   0 grote1    (5613)     5613     6467 2023-06-09 01:06:01.000000 picmistandard-0.25.0/applied_fields.py
+-rw-------   0 grote1    (5613)     5613     7917 2022-09-16 16:29:08.000000 picmistandard-0.25.0/base.py
+-rw-------   0 grote1    (5613)     5613    10356 2022-09-09 18:55:41.000000 picmistandard-0.25.0/diagnostics.py
+-rw-------   0 grote1    (5613)     5613    54140 2023-04-19 20:15:44.000000 picmistandard-0.25.0/fields.py
+-rw-------   0 grote1    (5613)     5613      828 2022-12-02 00:23:48.000000 picmistandard-0.25.0/interactions.py
+-rw-------   0 grote1    (5613)     5613     7713 2023-04-19 20:15:44.000000 picmistandard-0.25.0/lasers.py
+-rw-------   0 grote1    (5613)     5613    24153 2023-06-09 01:06:01.000000 picmistandard-0.25.0/particles.py
+drwx------   0 grote1    (5613)     5613        0 2023-06-09 01:13:46.577080 picmistandard-0.25.0/picmistandard.egg-info/
+-rw-------   0 grote1    (5613)     5613      171 2023-06-09 01:13:46.000000 picmistandard-0.25.0/picmistandard.egg-info/PKG-INFO
+-rw-------   0 grote1    (5613)     5613      378 2023-06-09 01:13:46.000000 picmistandard-0.25.0/picmistandard.egg-info/SOURCES.txt
+-rw-------   0 grote1    (5613)     5613        1 2023-06-09 01:13:46.000000 picmistandard-0.25.0/picmistandard.egg-info/dependency_links.txt
+-rw-------   0 grote1    (5613)     5613       23 2023-06-09 01:13:46.000000 picmistandard-0.25.0/picmistandard.egg-info/requires.txt
+-rw-------   0 grote1    (5613)     5613       14 2023-06-09 01:13:46.000000 picmistandard-0.25.0/picmistandard.egg-info/top_level.txt
+-rw-------   0 grote1    (5613)     5613       23 2022-08-31 01:00:06.000000 picmistandard-0.25.0/requirements.txt
+-rw-------   0 grote1    (5613)     5613       38 2023-06-09 01:13:46.578551 picmistandard-0.25.0/setup.cfg
+-rw-------   0 grote1    (5613)     5613      620 2023-04-19 20:15:44.000000 picmistandard-0.25.0/setup.py
+-rw-------   0 grote1    (5613)     5613     8089 2022-12-02 00:23:48.000000 picmistandard-0.25.0/simulation.py
+-rw-------   0 grote1    (5613)     5613       23 2023-06-09 01:08:46.000000 picmistandard-0.25.0/version.py
```

### Comparing `picmistandard-0.24.0/README.md` & `picmistandard-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/applied_fields.py` & `picmistandard-0.25.0/applied_fields.py`

 * *Files 11% similar despite different names*

```diff
@@ -163,7 +163,30 @@
         self.y_front_location = y_front_location
         self.z_front_location = z_front_location
         self.depth = depth
         self.number_of_cells = number_of_cells
 
         self.handle_init(kw)
 
+        
+class PICMI_LoadGriddedField(_ClassWithInit):
+    """
+    The data read in is used to initialize the E and B fields on the grid at the start of the simulation. 
+    The expected format is the file is OpenPMD with axes (x,y,z) in Cartesian, or (r,z) in Cylindrical geometry. 
+
+    Parameters
+    ----------
+    read_fields_from_path: string
+        Path to file with field data
+
+    load_B: bool, default=True
+        If False, do not load magnetic field
+
+    load_E: bool, default=True
+        If False, do not load electric field
+    """
+    def __init__(self, read_fields_from_path, load_B=True, load_E=True, **kw):
+        self.load_B = load_B
+        self.load_E = load_E
+        self.read_fields_from_path = read_fields_from_path
+        
+        self.handle_init(kw)
```

### Comparing `picmistandard-0.24.0/base.py` & `picmistandard-0.25.0/base.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/diagnostics.py` & `picmistandard-0.25.0/diagnostics.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/fields.py` & `picmistandard-0.25.0/fields.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/interactions.py` & `picmistandard-0.25.0/interactions.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/lasers.py` & `picmistandard-0.25.0/lasers.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/particles.py` & `picmistandard-0.25.0/particles.py`

 * *Files 6% similar despite different names*

```diff
@@ -278,14 +278,88 @@
         self.rms_velocity = rms_velocity
         self.directed_velocity = directed_velocity
         self.fill_in = fill_in
 
         self.handle_init(kw)
 
 
+class PICMI_FoilDistribution(_ClassWithInit):
+    """
+    Describes a foil with optional exponential pre- and post-plasma ramps along the propagation direction.
+
+    Parameters
+    ----------
+    density: float
+        Physical number density [m^-3]
+
+    front : float
+        postion of front surface of foil [m]
+
+    thickness: float >= 0
+        thickness of the foil [m]
+
+    exponential_pre_plasma_length: float > 0, optional
+        length scale of expoential decay of pre-foil plasma density [m]
+
+    exponential_pre_plasma_cutoff : float >= 0, optional
+        cutoff length for exponential decay of pre-foil density [m]
+
+    exponential_post_plasma_length: float > 0, optional
+        length scale of expoential decay of post-foil plasma density [m]
+
+    exponential_post_plasma_cutoff : float >= 0, optional
+        cutoff length for exponential decay of post-foil density [m]
+
+    lower_bound: vector of length 3 of floats, optional
+        Lower bound of the distribution [m]
+
+    upper_bound: vector of length 3 of floats, optional
+        Upper bound of the distribution [m]
+
+    rms_velocity: vector of length 3 of floats, default=[0.,0.,0.]
+        Thermal velocity spread [m/s]
+
+    directed_velocity: vector of length 3 of floats, default=[0.,0.,0.]
+        Directed, average, velocity [m/s]
+
+    fill_in: bool, optional
+        Flags whether to fill in the empty spaced opened up when the grid moves
+    """
+
+    def __init__(self,
+                 density,
+                 front,
+                 thickness,
+                 rms_velocity = [0., 0., 0.],
+                 directed_velocity = [0., 0., 0.],
+                 lower_bound = [None,None,None],
+                 upper_bound = [None,None,None],
+                 exponential_pre_plasma_length = None,
+                 exponential_pre_plasma_cutoff = None,
+                 exponential_post_plasma_length = None,
+                 exponential_post_plasma_cutoff = None,
+                 fill_in = None,
+                 **kw) :
+        self.density = density
+        self.lower_bound = lower_bound
+        self.upper_bound = upper_bound
+        self.rms_velocity = rms_velocity
+        self.directed_velocity = directed_velocity
+        self.fill_in = fill_in
+
+        self.front = front
+        self.thickness = thickness
+        self.exponential_pre_plasma_length = exponential_pre_plasma_length
+        self.exponential_pre_plasma_cutoff = exponential_pre_plasma_cutof
+        self.exponential_post_plasma_length = exponential_post_plasma_length
+        self.exponential_post_plasma_cutoff = exponential_post_plasma_cutoff
+
+        self.handle_init(kw)
+
+
 class PICMI_UniformFluxDistribution(_ClassWithInit):
     """
     Describes a flux of particles emitted from a plane
 
     Parameters
     ----------
     flux: float
```

### Comparing `picmistandard-0.24.0/setup.py` & `picmistandard-0.25.0/setup.py`

 * *Files identical despite different names*

### Comparing `picmistandard-0.24.0/simulation.py` & `picmistandard-0.25.0/simulation.py`

 * *Files identical despite different names*

