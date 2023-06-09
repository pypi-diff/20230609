# Comparing `tmp/scselpy-1.1.3.tar.gz` & `tmp/scselpy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scselpy-1.1.3.tar", last modified: Thu Apr  6 17:11:21 2023, max compression
+gzip compressed data, was "scselpy-1.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scselpy-1.1.3.tar` & `scselpy-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1747 2023-04-06 17:10:37.240881 scselpy-1.1.3/README.md
--rw-r--r--   0        0        0      915 2023-03-22 13:42:12.675245 scselpy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2075 2023-02-08 20:22:06.225149 scselpy-1.1.3/scselpy/AnndataTestObj/_CreateAnndataObj.py
--rw-r--r--   0        0        0       76 2021-10-04 13:18:11.988429 scselpy-1.1.3/scselpy/AnndataTestObj/__init__.py
--rw-r--r--   0        0        0      337 2022-07-02 12:22:31.203866 scselpy-1.1.3/scselpy/Rename_annotation/_GenerateDict.py
--rw-r--r--   0        0        0     1773 2022-07-05 15:22:34.862482 scselpy-1.1.3/scselpy/Rename_annotation/_RenameAnno.py
--rw-r--r--   0        0        0      202 2022-07-02 12:54:47.491839 scselpy-1.1.3/scselpy/Rename_annotation/__init__.py
--rw-r--r--   0        0        0      245 2023-03-15 10:26:31.448006 scselpy-1.1.3/scselpy/__init__.py
--rw-r--r--   0        0        0       75 2022-07-07 13:34:32.845258 scselpy-1.1.3/scselpy/__main__.py
--rw-r--r--   0        0        0      229 2022-07-07 13:50:29.973245 scselpy-1.1.3/scselpy/call_main.py
--rw-r--r--   0        0        0      390 2023-03-21 16:57:41.456285 scselpy-1.1.3/scselpy/config.py
--rw-r--r--   0        0        0     1308 2023-03-17 14:29:25.040972 scselpy-1.1.3/scselpy/plotting/__init__.py
--rw-r--r--   0        0        0    39156 2023-04-06 16:42:50.832875 scselpy-1.1.3/scselpy/plotting/_scselpy.py
--rw-r--r--   0        0        0     5386 2021-10-04 13:18:11.984429 scselpy-1.1.3/scselpy/tests/REMAP_val.txt
--rw-r--r--   0        0        0     5135 2021-10-12 17:42:07.877314 scselpy-1.1.3/scselpy/tests/REMAP_val2.txt
--rw-r--r--   0        0        0     5155 2021-10-12 18:18:37.977322 scselpy-1.1.3/scselpy/tests/REMAP_val3.txt
--rw-r--r--   0        0        0        0 2021-10-04 13:18:11.984429 scselpy-1.1.3/scselpy/tests/__init__.py
--rw-r--r--   0        0        0    21701 2023-03-17 14:11:30.529000 scselpy-1.1.3/scselpy/tests/scselpy_tests.py
--rw-r--r--   0        0        0      434 2021-10-04 13:18:11.984429 scselpy-1.1.3/scselpy/tests/utils.py
--rw-r--r--   0        0        0      144 2023-02-08 19:34:20.109189 scselpy-1.1.3/scselpy/tools/__init__.py
--rw-r--r--   0        0        0     2933 2023-02-08 20:13:16.033156 scselpy-1.1.3/scselpy/tools/_calculate_stats.py
--rw-r--r--   0        0        0       17 2023-04-06 17:10:53.456881 scselpy-1.1.3/scselpy/version.py
--rw-r--r--   0        0        0        5 2023-04-06 17:10:53.456881 scselpy-1.1.3/scselpy/version.txt
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 scselpy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1747 2023-04-06 17:10:37.240881 scselpy-1.1.7/README.md
+-rw-r--r--   0        0        0      915 2023-03-22 13:42:12.675245 scselpy-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2075 2023-02-08 20:22:06.225149 scselpy-1.1.7/scselpy/AnndataTestObj/_CreateAnndataObj.py
+-rw-r--r--   0        0        0       76 2021-10-04 13:18:11.988429 scselpy-1.1.7/scselpy/AnndataTestObj/__init__.py
+-rw-r--r--   0        0        0      337 2022-07-02 12:22:31.203866 scselpy-1.1.7/scselpy/Rename_annotation/_GenerateDict.py
+-rw-r--r--   0        0        0     1773 2022-07-05 15:22:34.862482 scselpy-1.1.7/scselpy/Rename_annotation/_RenameAnno.py
+-rw-r--r--   0        0        0      202 2022-07-02 12:54:47.491839 scselpy-1.1.7/scselpy/Rename_annotation/__init__.py
+-rw-r--r--   0        0        0      245 2023-03-15 10:26:31.448006 scselpy-1.1.7/scselpy/__init__.py
+-rw-r--r--   0        0        0       75 2022-07-07 13:34:32.845258 scselpy-1.1.7/scselpy/__main__.py
+-rw-r--r--   0        0        0      229 2022-07-07 13:50:29.973245 scselpy-1.1.7/scselpy/call_main.py
+-rw-r--r--   0        0        0      390 2023-03-21 16:57:41.456285 scselpy-1.1.7/scselpy/config.py
+-rw-r--r--   0        0        0     1308 2023-03-17 14:29:25.040972 scselpy-1.1.7/scselpy/plotting/__init__.py
+-rw-r--r--   0        0        0    39780 2023-06-09 20:00:35.187676 scselpy-1.1.7/scselpy/plotting/_scselpy.py
+-rw-r--r--   0        0        0     5386 2021-10-04 13:18:11.984429 scselpy-1.1.7/scselpy/tests/REMAP_val.txt
+-rw-r--r--   0        0        0     5135 2021-10-12 17:42:07.877314 scselpy-1.1.7/scselpy/tests/REMAP_val2.txt
+-rw-r--r--   0        0        0     5155 2021-10-12 18:18:37.977322 scselpy-1.1.7/scselpy/tests/REMAP_val3.txt
+-rw-r--r--   0        0        0        0 2021-10-04 13:18:11.984429 scselpy-1.1.7/scselpy/tests/__init__.py
+-rw-r--r--   0        0        0    21701 2023-03-17 14:11:30.529000 scselpy-1.1.7/scselpy/tests/scselpy_tests.py
+-rw-r--r--   0        0        0      434 2021-10-04 13:18:11.984429 scselpy-1.1.7/scselpy/tests/utils.py
+-rw-r--r--   0        0        0      144 2023-02-08 19:34:20.109189 scselpy-1.1.7/scselpy/tools/__init__.py
+-rw-r--r--   0        0        0     2933 2023-02-08 20:13:16.033156 scselpy-1.1.7/scselpy/tools/_calculate_stats.py
+-rw-r--r--   0        0        0       17 2023-06-09 20:08:48.355669 scselpy-1.1.7/scselpy/version.py
+-rw-r--r--   0        0        0        5 2023-06-09 20:08:48.359670 scselpy-1.1.7/scselpy/version.txt
+-rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 scselpy-1.1.7/PKG-INFO
```

### Comparing `scselpy-1.1.3/README.md` & `scselpy-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/pyproject.toml` & `scselpy-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/AnndataTestObj/_CreateAnndataObj.py` & `scselpy-1.1.7/scselpy/AnndataTestObj/_CreateAnndataObj.py`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/Rename_annotation/_RenameAnno.py` & `scselpy-1.1.7/scselpy/Rename_annotation/_RenameAnno.py`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/plotting/__init__.py` & `scselpy-1.1.7/scselpy/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/plotting/_scselpy.py` & `scselpy-1.1.7/scselpy/plotting/_scselpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -714,27 +714,38 @@
     
     
     
     kwargs_copy,VarDict = setup(adata,**kwargs) # Create VarDict to keep track of scSELpy native args.
     if remove_show_override == True:
         del kwargs_copy["show"]
     
-    #adata = CheckRaw(anndata,VarDict,**kwargs)
+
     VarDict = checks(adata,VarDict,**kwargs) # Perform some checks
     if override == False:
         scat_plot,plotattr = set_map_attr(adata,VarDict,**kwargs) #umap, tsne, pca or scatter.
     else:  #Not supported, but if a user would want to run anything outside of umap, tsne, pca or scatter, I give them the option to by running: 
         scat_plot = kwargs['scat_plot']
         plotattr = kwargs['plotattr']
         del kwargs_copy['plotattr']
         del kwargs_copy['scat_plot']
         
     unsError = "The replot_lines parameter should only be invoked with the name of an anndata.uns. e.g. in case of adata.uns[\"REMAP_1\"], run scSELpy.pl.umap(adata,replot_lines=\"REMAP_1\",kwargs**). Current input: "+str(VarDict['replot_lines']) 
 
-                
+        
+    #PRE-plotting before backend switch. To make sure all parameters are working.
+    if scat_plot == "scat":
+        returned = plotattr(adata,VarDict['x_scat'],VarDict['y_scat'], **kwargs_copy) 
+    elif scat_plot == "embedding":
+        returned = plotattr(adata,basis=VarDict['basis'], **kwargs_copy) #The "show" parameter will always be false, even if user puts it on True.
+
+    else:
+        returned = plotattr(adata, **kwargs_copy) # Here we plot. plotattr is e.g. sc.pl.umap. As we switched the back-end, this plot will be interactive.
+
+
+        
     if VarDict['replot_lines'] != None and VarDict['load'] == None: #In this case, we can skip the interactive part. Just replotting the already drawn.
         try:
             ShapeDict = adata.uns[VarDict['replot_lines']].copy()
         except:
             
             raise AttributeError(unsError)
 
@@ -748,16 +759,16 @@
         returnVar = plotattr(adata,VarDict['x_scat'],VarDict['y_scat'], **kwargs_copy) #The "show" parameter will always be false, even if user puts it on True.
     elif scat_plot == "embedding":
         returnVar = plotattr(adata,basis=VarDict['basis'], **kwargs_copy) #The "show" parameter will always be false, even if user puts it on True.
 
     else:
         returnVar = plotattr(adata, **kwargs_copy) 
     
-    Backup_legend = plt.gca().legend_
 
+    
     if VarDict["use_log_scale"] == True:
         log_scale(VarDict,returnVar)
     
     
     #-------reploting the lines on the plot, so the plot can be printed and saved----------
     custom_lines = []
 
@@ -768,24 +779,28 @@
     
     if VarDict['line_labels'] != None:
 
         if len(ShapeDict) < len(VarDict['line_labels']):
             line_labels = VarDict['line_labels'][:len(ShapeDict)]
         else:
             line_labels = VarDict['line_labels']
-       
+
+        #handles.append(custom_lines)
+        #labels.append(line_labels)
         
-        plt.legend(custom_lines,line_labels,loc=VarDict['line_loc'],bbox_to_anchor=VarDict['line_bbox_to_anchor'],handlelength=VarDict['line_handlelength']) # Plotting the line legend. In getXY(), the labels are added.
-     
-    if Backup_legend != None:
         if type(returnVar) == list: #Multiple variables have been passed to the scanpy color argument.
-            returnVar[-1].add_artist(Backup_legend) #scSELpy is not made to support multiple plots in one go, so we just add the legend to the last plot.
-        else:
-            returnVar.add_artist(Backup_legend)
+            ax2 = returnVar[-1].twinx()
+            #scSELpy is not made to support multiple plots in one go, so we just add the legend to the last plot.
+        else:    
+            ax2 = returnVar.twinx() # We create a copy of the axes to add another legend. Using add_artist for adding legend is buggy.
+        ax2.legend(custom_lines,line_labels,loc=VarDict['line_loc'],bbox_to_anchor=VarDict['line_bbox_to_anchor'],handlelength=VarDict['line_handlelength']) # Plotting the line legend. In getXY(), the labels are added.
+        ax2.axis('off')
     
+
+        
     #--------- SAVING -----------------
     if VarDict['save'] != None: # We did not want the plots being saved while drawing. Now we can save it manually with the plt.savefig()
         Save(VarDict,scat_plot,returnVar) #Should automatically take the settings from scanpy.set_figure_params, as that function updated matplotlib.rcParams.
             
  
     #-----------Storing object with selected cells----------    
     # e.g. anndata.obs['Remap_1']
```

### Comparing `scselpy-1.1.3/scselpy/tests/REMAP_val.txt` & `scselpy-1.1.7/scselpy/tests/REMAP_val.txt`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/tests/REMAP_val2.txt` & `scselpy-1.1.7/scselpy/tests/REMAP_val2.txt`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/tests/REMAP_val3.txt` & `scselpy-1.1.7/scselpy/tests/REMAP_val3.txt`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/tests/scselpy_tests.py` & `scselpy-1.1.7/scselpy/tests/scselpy_tests.py`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/scselpy/tools/_calculate_stats.py` & `scselpy-1.1.7/scselpy/tools/_calculate_stats.py`

 * *Files identical despite different names*

### Comparing `scselpy-1.1.3/PKG-INFO` & `scselpy-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scselpy
-Version: 1.1.3
+Version: 1.1.7
 Summary: A tool to select cells on scanpy-based scRNA-seq analysis pipelines.
 Author: Mark Dedden
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
 Classifier: Natural Language :: English
```

