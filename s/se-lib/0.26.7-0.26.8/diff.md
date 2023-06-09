# Comparing `tmp/se_lib-0.26.7.tar.gz` & `tmp/se_lib-0.26.8.tar.gz`

## Comparing `se_lib-0.26.7.tar` & `se_lib-0.26.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.7/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.7/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.7/selib/.DS_Store
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 se_lib-0.26.7/selib/__init__.py
--rw-r--r--   0        0        0    78302 2020-02-02 00:00:00.000000 se_lib-0.26.7/selib/selib.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 se_lib-0.26.7/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.7/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 se_lib-0.26.7/pyproject.toml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 se_lib-0.26.7/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.8/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.8/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/.DS_Store
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/__init__.py
+-rw-r--r--   0        0        0    80457 2020-02-02 00:00:00.000000 se_lib-0.26.8/selib/selib.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 se_lib-0.26.8/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.8/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 se_lib-0.26.8/pyproject.toml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 se_lib-0.26.8/PKG-INFO
```

### Comparing `se_lib-0.26.7/.DS_Store` & `se_lib-0.26.8/.DS_Store`

 * *Files 16% similar despite different names*

```diff
@@ -252,21 +252,21 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 001d 0000 0004  ................
 00001010: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
-00001020: 0000 0000 0001 c6c7 0000 0004 002e 0067  ...............g
+00001020: 0000 0000 000b ef47 0000 0004 002e 0067  .......G.......g
 00001030: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
-00001040: 4aeb 5880 64f0 c441 0000 0004 002e 0067  J.X.d..A.......g
+00001040: dcdc f58c 520b c541 0000 0004 002e 0067  ....R..A.......g
 00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
-00001060: 4aeb 5880 64f0 c441 0000 0004 002e 0067  J.X.d..A.......g
+00001060: dcdc f58c 520b c541 0000 0004 002e 0067  ....R..A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
-00001080: 0004 e000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
+00001080: 0015 6000 0000 0004 0064 0069 0073 0074  ..`......d.i.s.t
 00001090: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
 000010a0: 0000 002e ffff ffff ffff 0000 0000 0004  ................
 000010b0: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
 000010c0: 0000 00bd 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000010d0: 0405 0607 0709 070b 075d 5368 6f77 5374  .........]ShowSt
 000010e0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 000010f0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
@@ -276,21 +276,21 @@
 00001130: 0908 095f 101d 7b7b 2d31 3430 342c 202d  ..._..{{-1404, -
 00001140: 3434 387d 2c20 7b31 3430 342c 2031 3931  448}, {1404, 191
 00001150: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
 00001160: 8f00 0000 0000 0001 0100 0000 0000 0000  ................
 00001170: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 9000 0000 0400 6400 6900 7300 7464 7363  ......d.i.s.tdsc
 00001190: 6c62 6f6f 6c01 0000 0004 0064 0069 0073  lbool......d.i.s
-000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0000  .tlg1Scomp......
-000011b0: a5e7 0000 0004 0064 0069 0073 0074 6d6f  .......d.i.s.tmo
-000011c0: 4444 626c 6f62 0000 0008 213b e5ed 61f2  DDblob....!;..a.
-000011d0: c441 0000 0004 0064 0069 0073 0074 6d6f  .A.....d.i.s.tmo
-000011e0: 6444 626c 6f62 0000 0008 213b e5ed 61f2  dDblob....!;..a.
-000011f0: c441 0000 0004 0064 0069 0073 0074 7068  .A.....d.i.s.tph
-00001200: 3153 636f 6d70 0000 0000 0000 c000 0000  1Scomp..........
+000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0004  .tlg1Scomp......
+000011b0: 8ae7 0000 0004 0064 0069 0073 0074 6d6f  .......d.i.s.tmo
+000011c0: 4444 626c 6f62 0000 0008 9bc6 2bee d804  DDblob......+...
+000011d0: c541 0000 0004 0064 0069 0073 0074 6d6f  .A.....d.i.s.tmo
+000011e0: 6444 626c 6f62 0000 0008 9bc6 2bee d804  dDblob......+...
+000011f0: c541 0000 0004 0064 0069 0073 0074 7068  .A.....d.i.s.tph
+00001200: 3153 636f 6d70 0000 0000 0005 1000 0000  1Scomp..........
 00001210: 0004 0064 0069 0073 0074 7653 726e 6c6f  ...d.i.s.tvSrnlo
 00001220: 6e67 0000 0001 0000 0007 004c 0049 0043  ng.........L.I.C
 00001230: 0045 004e 0053 0045 496c 6f63 626c 6f62  .E.N.S.EIlocblob
 00001240: 0000 0010 0000 00af 0000 002e ffff ffff  ................
 00001250: ffff 0000 0000 000e 0070 0079 0070 0072  .........p.y.p.r
 00001260: 006f 006a 0065 0063 0074 002e 0074 006f  .o.j.e.c.t...t.o
 00001270: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
@@ -313,21 +313,21 @@
 00001380: 202d 3133 387d 2c20 7b31 3430 342c 2031   -138}, {1404, 1
 00001390: 3931 367d 7d09 0815 232f 3b52 5f6b 6c6d  916}}...#/;R_klm
 000013a0: 6e6f 8f00 0000 0000 0001 0100 0000 0000  no..............
 000013b0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
 000013c0: 0000 9000 0000 0500 7300 6500 6c00 6900  ........s.e.l.i.
 000013d0: 6264 7363 6c62 6f6f 6c01 0000 0005 0073  bdsclbool......s
 000013e0: 0065 006c 0069 0062 6c67 3153 636f 6d70  .e.l.i.blg1Scomp
-000013f0: 0000 0000 0000 f955 0000 0005 0073 0065  .......U.....s.e
+000013f0: 0000 0000 0001 4cbf 0000 0005 0073 0065  ......L......s.e
 00001400: 006c 0069 0062 6d6f 4444 626c 6f62 0000  .l.i.bmoDDblob..
-00001410: 0008 e7af bd52 62f0 c441 0000 0005 0073  .....Rb..A.....s
+00001410: 0008 e850 f58c 520b c541 0000 0005 0073  ...P..R..A.....s
 00001420: 0065 006c 0069 0062 6d6f 6444 626c 6f62  .e.l.i.bmodDblob
-00001430: 0000 0008 e7af bd52 62f0 c441 0000 0005  .......Rb..A....
+00001430: 0000 0008 e850 f58c 520b c541 0000 0005  .....P..R..A....
 00001440: 0073 0065 006c 0069 0062 7068 3153 636f  .s.e.l.i.bph1Sco
-00001450: 6d70 0000 0000 0001 2000 0000 0005 0073  mp...... ......s
+00001450: 6d70 0000 0000 0001 8000 0000 0005 0073  mp.............s
 00001460: 0065 006c 0069 0062 7653 726e 6c6f 6e67  .e.l.i.bvSrnlong
 00001470: 0000 0001 0000 0005 0074 0065 0073 0074  .........t.e.s.t
 00001480: 0073 496c 6f63 626c 6f62 0000 0010 0000  .sIlocblob......
 00001490: 02d5 0000 002e ffff ffff ffff 0000 0000  ................
 000014a0: 0005 0074 0065 0073 0074 0073 6473 636c  ...t.e.s.t.sdscl
 000014b0: 626f 6f6c 0100 0000 0500 7400 6500 7300  bool......t.e.s.
 000014c0: 7400 736c 6731 5363 6f6d 7000 0000 0000  t.slg1Scomp.....
```

### Comparing `se_lib-0.26.7/selib/.DS_Store` & `se_lib-0.26.8/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.7/selib/__init__.py` & `se_lib-0.26.8/selib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-from .selib import context_diagram, activity_diagram, use_case_diagram, sequence_diagram, design_structure_matrix, design_structure_matrix, tree, fault_tree_diagram, read_fault_tree_excel, critical_path_diagram, draw_fault_tree_diagram_quantitative, fault_tree_cutsets, init_sd_model, build_model, add_stock, add_auxiliary, add_flow, plot_graph, save_graph, run_model, set_logical_run_time, get_logical_end_time, draw_sd_model, draw_model_diagram, init_de_model, add_source, add_server, add_delay, add_terminate, run_de_model, draw_discrete_model_diagram, plot_histogram
+from .selib import context_diagram, activity_diagram, use_case_diagram, sequence_diagram, design_structure_matrix, design_structure_matrix, tree, fault_tree_diagram, read_fault_tree_excel, critical_path_diagram, draw_fault_tree_diagram_quantitative, fault_tree_cutsets, init_sd_model, build_model, add_stock, add_auxiliary, add_flow, plot_graph, save_graph, run_model, set_logical_run_time, get_logical_end_time, draw_sd_model, draw_model_diagram, init_de_model, add_source, add_server, add_delay, add_terminate, run_de_model, draw_discrete_model_diagram, plot_histogram, requirements_diagram, causal_diagram
```

### Comparing `se_lib-0.26.7/selib/selib.py` & `se_lib-0.26.8/selib/selib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .26.7
+se-lib Version .26.8
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -102,15 +102,15 @@
 
 def context_diagram(system, external_systems, filename=None, format='svg', engine='neato'):
     """
     Returns a context diagram.
 
     Parameters
     ----------
-    system_name : string
+    system : string
         The name of the system to label the diagram.
     external_systems : list of strings
         Names of the external systems that interact with the system in a list.
     filename : string, optional
         A filename for the output not including a filename extension. The extension will specified by the format parameter.
     format : string, optional
         The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
@@ -438,14 +438,49 @@
 
     if filename != None:
         activity.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
     return activity
 
 
+# textwrap and graphviz are required for requirements_diagram(), but are called earlier in the library. They are
+# commented out here, but should be included if the function is pulled out separately.
+# import textwrap
+# import graphviz 
+
+wrap_width = 40
+def wrap(text): return textwrap.fill(
+    text, width=wrap_width, break_long_words=False)
+
+online = False
+
+def requirements_diagram(element_dependencies, filename="tree", format='dot', rankdir='TB'):
+    global svg
+    node_attr = {'color': 'black', 'fontsize': '11',
+                 'shape': 'box'}  # 'fontname': 'arial',
+    edge_attr = {'arrowsize': '.5', 'fontname': 'arial', 'fontsize': '11', }
+    activity = graphviz.Digraph('G', filename=filename, node_attr=node_attr,
+                                edge_attr=edge_attr, engine="dot", format='svg')
+    activity.attr(rankdir=rankdir, splines='ortho')  # rankdir='LR'
+    for edge_pair in element_dependencies:
+        if type(edge_pair[1]) != tuple: activity.edge(wrap(edge_pair[0]+'\l'), wrap(edge_pair[1]+'\l'))
+        if type(edge_pair[1]) == tuple:
+            for num, tail in enumerate(edge_pair[1]):
+                activity.edge(wrap(edge_pair[0]+'\l'), wrap(edge_pair[1][num]+'\l'))
+
+    if filename != None:
+        activity.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
+        #os.remove(filename) also doesn't work on windows "permission denied"
+    #return u
+    if online:
+        svg = return_svg_from_dot(str(activity), "dot")
+        print(str(svg))      
+        print(svg)
+    else:
+        return activity
 
 
 def fault_tree_diagram(ft, filename=None, format='svg'):
     """ Returns a fault tree diagram.
 
     Parameters
     ----------
@@ -1388,14 +1423,30 @@
                 css.remove(b)
             except BaseException:
                 continue
     if verbose: print(f'***{css=}') # rm
     ft = copy
     return(css)
 
+def causal_diagram(relationships):
+    dot_text= """
+    digraph G {
+  	node [color=black fontsize=11 shape=plain style=rounded]
+  	edge [arrowsize=.5 fontname=arial fontsize=11]
+  	  	splines=curved
+    """
+    
+    for relation in relationships:
+        dot_text += f""" "{relation[0]}" -> "{relation[1]}" [headlabel = "{relation[2]}"] """
+    
+    dot_text += "}"
+    src = graphviz.Source(dot_text, engine="neato", filename="atc_cld", format='svg')
+    src.render()
+    return(src)
+
 # system dynamics simulation functions
 
 def init_sd_model(start, stop, dt):
   """
   Instantiates a system dynamics model for simulation
   """
   global xmile_header, model, model_specs, model_dict, model_type
@@ -1963,8 +2014,8 @@
     fig, ax = plt.subplots(figsize=(5, 3))
     ax.hist(data, **kwargs)
     ax.set(xlabel=xlabel, ylabel='Frequency')
     ax.xaxis.labelmargin = -50
     ax.yaxis.labelmargin = 30
     plt.subplots_adjust(bottom=0.15,)
     if filename is not None: plt.savefig(filename)
-    return fig
+    return fig
```

### Comparing `se_lib-0.26.7/LICENSE` & `se_lib-0.26.8/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.7/README.md` & `se_lib-0.26.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-Version .26.7
+Version .26.8
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.7/pyproject.toml` & `se_lib-0.26.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26.7"
+version = "0.26.8"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26.7/PKG-INFO` & `se_lib-0.26.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26.7
+Version: 0.26.8
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Requires-Dist: simpy
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26.7
+Version .26.8
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

