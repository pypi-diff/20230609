# Comparing `tmp/MatAn-0.1.5.2.2-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21024 bytes, number of entries: 9
--rw-r--r--  2.0 unx    15734 b- defN 23-May-08 17:43 matan/__init__.py
+Zip file size: 21495 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    17356 b- defN 23-Jun-09 11:29 matan/__init__.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-May-08 17:43 matan/files.py
--rw-r--r--  2.0 unx      155 b- defN 23-May-06 21:05 misc/__init__.py
--rw-r--r--  2.0 unx     2771 b- defN 23-May-08 18:03 properties/__init__.py
--rw-r--r--  2.0 unx    34670 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3931 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      694 b- defN 23-May-09 15:15 MatAn-0.1.5.2.2.dist-info/RECORD
-9 files, 62872 bytes uncompressed, 19842 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx      155 b- defN 23-May-29 20:55 misc/__init__.py
+-rw-r--r--  2.0 unx     2659 b- defN 23-May-29 20:57 properties/__init__.py
+-rw-r--r--  2.0 unx    34670 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4161 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jun-09 11:29 MatAn-0.1.5.2.3.dist-info/RECORD
+9 files, 64612 bytes uncompressed, 20313 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: misc/__init__.py
 Comment: 
 
 Filename: properties/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.5.2.2.dist-info/LICENSE
+Filename: MatAn-0.1.5.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: MatAn-0.1.5.2.2.dist-info/METADATA
+Filename: MatAn-0.1.5.2.3.dist-info/METADATA
 Comment: 
 
-Filename: MatAn-0.1.5.2.2.dist-info/WHEEL
+Filename: MatAn-0.1.5.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: MatAn-0.1.5.2.2.dist-info/top_level.txt
+Filename: MatAn-0.1.5.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: MatAn-0.1.5.2.2.dist-info/RECORD
+Filename: MatAn-0.1.5.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matan/__init__.py

```diff
@@ -1,12 +1,14 @@
+import sys
+sys.path.append("..") # Adds higher directory to python modules path.
 import numpy as np
 import matplotlib.pyplot as plt
 from typing import Union
 
-from .. import properties
+from ..properties import  *
 
 
 
 """
 TODO:
 Create  abstract class for properties like tensile strength, tensile modulus, etc, with pass, so using diffrent norms and materials will be easier
 Move calculation of real values into method of engineering values
@@ -17,116 +19,164 @@
 https://professorkazarinoff.github.io/Engineering-Materials-Programming/07-Mechanical-Properties/mechanical-properties-from-stress-strain-curves.html
 
 
 """
 
 
 class sample:
-    """
-    Class to menage material, material properities, converting to engineerin stress etc.
-    """
+    """Initialization of sample class
+
+    That's class for each of your tested sample
+
+    Parameters
+        ----------
+        name : str
+        name of your sample etc. Neat PLA
+        thickness : float
+        thickness of your sample
+        width : float
+        width of your sample
+        elongation_array : Union[list, np.array]
+        elongation array from your tensile machine
+        force_array : Union[list, np.array]
+        forces obtained from your tensile machine
+        stress_array : Union[list, np.array]
+        calculated stresses
+        strain_array : Union[list, np.array]
+        calculated strains
+        manufactured_method : str
+        how your sample was made, etc. by FDM or injection method, just for description
+        comments : str
+        any comments describing your sample
+        force_units : str
+        force units of your force array
+        lenght_units : str
+        length units of your force array
+
+    Raises
+        ------
+        ValueError
+        Raises ValueError while stress/strains or width/thickness are not defined
+    
+    Examples
+        --------
+        elongation_array=df["elongation"]
+        force_array=df["force"]
+
+        # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
+        example=mt.sample(name="your sample name",
+        thickness = 5,
+        width= 5,
+        elongation_array=elongation_array,
+        force_array=force_array
+        )
+        """
+
     def __init__(self,name: str,
-                 thickness:float = None,
-                 width:float = None,
-                 elongation_array: Union[list, np.array] =None,
-                 force_array: Union[list, np.array] =None,
-                 stress_array: Union[list, np.array] =None,
-                 strain_array: Union[list, np.array] =None,
-                 manufactured_method=None,
-                 comments=None,
-                 force_units: str="N",
-                 lenght_units: str="mm"):
-
-        self.name=name
-        self.thickness, self.width= thickness,width
-        self.eng_values=engineering_values(name=name,
-                                           force_units=force_units,
-                                           lenght_units=lenght_units,
-                                           thickness=thickness,
-                                           width=width
-                                           )
-        self.force_units, self.lenght_units=force_units,lenght_units
-        if stress_array is None and strain_array is None:
-            if elongation_array is None and force_array is None:
-                raise ValueError("None of elongation/force or stress/strain arrays are defined!")
-            elif thickness is None:
-                raise ValueError("Thickness is not defined!")
-            elif width is None:
-                raise ValueError(" Width is not defined!")
-            else:
-                self.elongation_array=elongation_array
-                self.force_array=force_array
-                self.eng_values.calculate(thickness=self.thickness,
-                                          width=self.width,
-                                          elongation_array=elongation_array,
-                                          force_array=force_array)
+                     thickness:float = None,
+                     width:float = None,
+                     elongation_array: Union[list, np.array] =None,
+                     force_array: Union[list, np.array] =None,
+                     stress_array: Union[list, np.array] =None,
+                     strain_array: Union[list, np.array] =None,
+                     manufactured_method: str=None,
+                     comments: str=None,
+                     force_units: str="N",
+                     lenght_units: str="mm"):
+            
+        
 
-        else:
-            self.eng_values.set(stress_array, strain_array)
+
+            self.name=name
+            self.thickness, self.width= thickness,width
+            self.eng_values=engineering_values(name=name,
+                                               force_units=force_units,
+                                               lenght_units=lenght_units,
+                                               thickness=thickness,
+                                               width=width
+                                               )
+            self.force_units, self.lenght_units=force_units,lenght_units
+            if stress_array is None and strain_array is None:
+                if elongation_array is None and force_array is None:
+                    raise ValueError("None of elongation/force or stress/strain arrays are defined!")
+                elif thickness is None:
+                    raise ValueError("Thickness is not defined!")
+                elif width is None:
+                    raise ValueError(" Width is not defined!")
+                else:
+                    self.elongation_array=elongation_array
+                    self.force_array=force_array
+                    self.eng_values.calculate(thickness=self.thickness,
+                                              width=self.width,
+                                              elongation_array=elongation_array,
+                                              force_array=force_array)
+
+            else:
+                self.eng_values.set(stress_array, strain_array)
 
     def calculate_real_values(self):
         self.real_values=real_values_class(name=self.name,
                                            thickness=self.thickness,
                                            width=self.width,
                                            force_units=self.force_units,
-                                            lenght_units=self.lenght_units
-                                               )
+                                           lenght_units=self.lenght_units
+                                           )
         self.real_values.calculate(self.eng_values.stress,
-                                           self.eng_values.strain)            
+                                   self.eng_values.strain)            
     def plot(self, show=False):
-            """Method for plotting the results
+        """Method for plotting the results
 
             This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
             parameter show as True
 
             Parameters
             ----------
             show : bool
                 It it equal to matplotlib.pyplot function show
 
             Examples
             --------
             FIXME: Add docs.
 
             """
-            plt.plot(self.elongation_array,self.force_array, label=self.name)
-            plt.title(self.name)
-            plt.ylabel(f"Force [{self.force_units}]")
-            plt.xlabel(f"Strain [{self.lenght_units}]")
-            plt.legend()
-            if show:
+        plt.plot(self.elongation_array,self.force_array, label=self.name)
+        plt.title(self.name)
+        plt.ylabel(f"Force [{self.force_units}]")
+        plt.xlabel(f"Strain [{self.lenght_units}]")
+        plt.legend()
+        if show:
                 plt.show()        
 
 
                 
         
     def composition_from_name(delimiter: str, percent_sign="p"):
         """
         TODODO baby shark
         method to obtain material ingridiens from name, as I usually name files extracted from machine with code allowing me to get that information from filename
-    Finds the proportional range of a stress-strain curve by searching for a derivative.
-    
+        Finds the proportional range of a stress-strain curve by searching for a derivative.
+        
     Parameters:
         strain (array-like): An array of strain values.
         stress (array-like): An array of corresponding stress values.
         n: An count of chunks to divide stress/strain array
-    
+        
     Returns:n
             Sets start and end of proportional range points
-    """
+        """
         pass
     
 class engineering_values:
         def __init__(self,
                      thickness,
                      width,
                      name=None,
                      force_units="N",
-                      lenght_units="mm"
-            ):
+                     lenght_units="mm"
+                     ):
             """initializer of engineering values class
 
             This class is used to menage the properties of engineering values
 
             Parameters
             ----------
             name : str
@@ -242,20 +292,20 @@
             def __init__(self,stress, strain):
                 at_break=properties.at_break(stress, strain)
                 self.stress=at_break.stress
                 self.strain=at_break.strain
 
 
         def calculate_tensile_modulus(self,
-                                    plot=False,
-                                    r2=True,
-                                    output=True,
-                                    lower_limit=0.05,
-                                    upper_limit=0.25
-                                    ):
+                                      plot=False,
+                                      r2=True,
+                                      output=True,
+                                      lower_limit=0.05,
+                                      upper_limit=0.25
+                                      ):
             """            Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent according to DIN ISO 527-1
 
             Parameters
             ----------
             plot : bool
                 Put True for use pyplot on the tensile modulus part
             r2 : Put coeffitient 	of determination into pyplot label
@@ -270,25 +320,25 @@
             Examples
             --------
             FIXME: Add docs.
 
             """
 
             E=properties.tensile_modulus(self.stress,
-                                       self.strain,
-                                       percent_strain=self.percent_strain
-                                       )
+                                         self.strain,
+                                         percent_strain=self.percent_strain
+                                         )
             if plot:
                 label=rf"Young's modulus {int(E.tensile_modulus)} $\left[\frac{{{self.force_units}}}{{{self.lenght_units}^2}}\right]$"
                 if r2:
                     label+="\n"+rf"$R^{{{2}}}={E.r2}$"
-                plt.plot(E.module_strain,
-                         E.module_stress,
-                         label=label
-                         )
+                    plt.plot(E.module_strain,
+                             E.module_stress,
+                             label=label
+                             )
             if output:
                 print(f"Tensile modulus is equal to {int(E.tensile_modulus)} [{self.force_units}/{self.lenght_units}^2]")
                 return   E.tensile_modulus
 
                 
         def set(self,
                 engineering_stress: Union[list, np.array] =None,
@@ -310,17 +360,17 @@
             --------
             FIXME: Add docs.
 
             """
             
             self.stress, self.strain=engineering_stress, engineering_strain
             self.calculate(thickness=self.thickness,
-                                      width=self.width,
-                                      elongation_array=None,
-                                      force_array=None)
+                           width=self.width,
+                           elongation_array=None,
+                           force_array=None)
             
 
         def plot(self, show=False):
             """Method for plotting the results
 
             This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
             parameter show as True
@@ -372,20 +422,20 @@
                              )
 
         def calculate(self, stress, strain):
             """
                 Calculates the true stress and strain, from engineering values.
                 Read more there:
                         https://courses.ansys.com/index.php/courses/topics-in-metal-plasticity/lessons/how-to-define-a-multilinear-hardening-plasticity-model-lesson-1/
-    
+            
                 Parameters:
                         strain (array-like): An array of strain values.
                         stress (array-like): An array of corresponding stress values.
                         n: An count of chunks to divide stress/strain array
-    
+            
                 Returns:
                     A tuple (start_strain, end_strain) representing the proportional range of the stress-strain curve.
             """
             self.stress=[stress_val*(1+strain_val) for stress_val, strain_val in zip(stress, strain)]
             self.strain=[np.log(1+strain_val) for strain_val in strain]
 
             self.strength=self.calculate_strength(self.stress,
```

## properties/__init__.py

```diff
@@ -56,19 +56,17 @@
 
 class yield_strenght:
     def __init__(self,stress, strain):
         self.value=misc.round_sig(stress[self.find_idx(stress,strain)], sig=3)
         self.strain=misc.round_sig(strain[self.find_idx(stress,strain)])
     def find_idx(self, stress,strain):
         for i in range(1, len(strain)):
-            print(i, stress[i] , 'huju')
             if strain[i] > strain[i-1] and stress[i] <= stress[i-1]:
                 if stress[i]>1:
-                    print(stress[i])
                     return i
                 else:
-                    print("kurwo", i , stress[i], len(stress))
                     continue
                     # exit()
+        return len(strain)-1
```

## Comparing `MatAn-0.1.5.2.2.dist-info/LICENSE` & `MatAn-0.1.5.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MatAn-0.1.5.2.2.dist-info/METADATA` & `MatAn-0.1.5.2.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MatAn
-Version: 0.1.5.2.2
+Version: 0.1.5.2.3
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
 Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 3 - Alpha
@@ -35,30 +35,34 @@
 
 Moreover, the package would need a graphical user interface, which could make it even simpler to use and, more importantly, allow users to upload their obtained results into OpenAccess databases and export plastic strains, tensile modulus, and other properties needed to perform FEM and other numerical analysis. That could make FEM methods even more accessible, which would lead to a decrease in the use of unnecessary materials and, due to this, less CO2 pollution.
 
 
 # How to use it?
 
 Just simply put elongation and force arrays into sample
+
+Be aware that sometimes csv files can have diffrent extension depends on machine manufacturer. To be sure just check it using simples notepad, or try to read it by pandas.
+
 ```python
 import matan as mt
 import pandas as pd
 
 path_to_your_CSV = r"path/to/your/CSV"
 
 
 '''
 Be aware that somethimes some software machines uses diffrent encoding! Check the documentation of pandas.read_csv for more
 '''
 test_data_frame = pd.read_csv(path_to_your_CSV)
 
 elongation_array=df["elongation"]
-elongation_array=df["force"]
+force_array=df["force"]
 
 # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
+# by default force units are Newtons and lenght units are mm
 example=mt.sample(name="your sample name",
 thickness = 5,
 width= 5,
 elongation_array=elongation_array,
 force_array=force_array
 )
```

