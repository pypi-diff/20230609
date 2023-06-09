# Comparing `tmp/easydags-0.0.6.tar.gz` & `tmp/easydags-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.6.tar", last modified: Wed Jun  7 19:36:53 2023, max compression
+gzip compressed data, was "easydags-0.0.7.tar", last modified: Fri Jun  9 14:30:28 2023, max compression
```

## Comparing `easydags-0.0.6.tar` & `easydags-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.906931 easydags-0.0.6/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.6/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    14949 2023-06-07 19:36:53.906738 easydags-0.0.6/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    14754 2023-06-07 19:26:58.000000 easydags-0.0.6/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.905883 easydags-0.0.6/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.6/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.6/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    20355 2023-06-07 19:17:32.000000 easydags-0.0.6/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.6/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.6/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.6/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-07 19:36:53.906576 easydags-0.0.6/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    14949 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-07 19:36:53.000000 easydags-0.0.6/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.6/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-07 19:36:53.906970 easydags-0.0.6/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-07 19:36:44.000000 easydags-0.0.6/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.705435 easydags-0.0.7/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.7/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    16755 2023-06-09 14:30:28.705155 easydags-0.0.7/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    16560 2023-06-09 14:28:29.000000 easydags-0.0.7/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.703967 easydags-0.0.7/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.7/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.7/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    22827 2023-06-09 14:25:30.000000 easydags-0.0.7/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.7/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.7/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.7/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.704879 easydags-0.0.7/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    16755 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.7/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-09 14:30:28.705492 easydags-0.0.7/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-09 14:29:32.000000 easydags-0.0.7/setup.py
```

### Comparing `easydags-0.0.6/LICENSE` & `easydags-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.6/PKG-INFO` & `easydags-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -315,14 +315,98 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
+
+```python
+#See draw_ensemble.py
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    print('beginning pre pro')
+    time.sleep(3)
+    print('end pre pro')
+    return 'df with cool features'
+
+
+
+nodes.append( ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) )  
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+nodes.append( ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model1'
+              ) )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 78373'
+
+nodes.append( ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model2'
+              ) )  
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+nodes.append( ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) )  
+
+
+
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+
+dag.only_draw(name = 'green dag')
+
+dag.only_draw(name = 'yellow dag', color = 'yellow')
+
+```
+
 
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
```

### Comparing `easydags-0.0.6/README.md` & `easydags-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -306,14 +306,98 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
+
+```python
+#See draw_ensemble.py
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    print('beginning pre pro')
+    time.sleep(3)
+    print('end pre pro')
+    return 'df with cool features'
+
+
+
+nodes.append( ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) )  
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+nodes.append( ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model1'
+              ) )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 78373'
+
+nodes.append( ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model2'
+              ) )  
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+nodes.append( ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) )  
+
+
+
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+
+dag.only_draw(name = 'green dag')
+
+dag.only_draw(name = 'yellow dag', color = 'yellow')
+
+```
+
 
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
```

### Comparing `easydags-0.0.6/easydags/dag.py` & `easydags-0.0.7/easydags/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,16 +287,116 @@
                     parent_node.compound_priority += leaf_node.compound_priority
 
                 # trim the graph from its leaf nodes
                 graph_ids.remove_node(leaf_id)
 
             # assign the new leaf nodes
             leaf_ids = graph_ids.leaf_nodes()
+    
+    def only_draw(self, name = None, color = 'green') -> None:
+        """
+        Draws the Networkx directed graph.
+        Args:
+            k: parameter for the layout of the graph, the higher, the further the nodes apart
+            display: display the layout created
+            t: time to display in seconds
+        """
+
+        if name is None:
+            name = self.name
+
+
+        for layer, nodes in enumerate(nx.topological_generations(self.graph_ids)):
+            # `multipartite_layout` expects the layer as a node attribute, so add the
+            # numeric layer value as a node attribute
+            for node in nodes:
+                self.graph_ids.nodes[node]["layer"] = layer
+
+        # Compute the multipartite_layout using the "layer" node attribute
+        pos = nx.multipartite_layout(self.graph_ids, subset_key="layer")
+        
+
+        from pyvis.network import Network
+
+        
+
+        head_title = f"{self.name} structure"
+
+        g = Network(layout=True,directed =True,heading=head_title)
+
+
+        titles = []
+        color_map = [] 
+        
+        for f in  list(pos.keys()):
+            title = f'''id: {f}'''
+            titles.append(title)
+            color_map.append(color)
+
+
+
+        aux = [x[0]   for x in pos.values()]
+
+        pos_holder = list(set(aux))
+
+        pos_holder.sort()
+
+        
+
+        level = [pos_holder.index(i) for i in aux]
+
 
-    def _draw(self,name='Graph', k: float = 0.8, display: bool = True, t: int = 3) -> None:
+        for i in range(len(pos.keys())):
+            g.add_node(list(pos.keys())[i],
+                         label= list(pos.keys())[i],
+                         level = level[i],
+                         title = titles[i],
+                         color= color_map[i])
+            
+
+        #g = Network('500px', '500px')
+
+
+
+
+        for e in self.graph_ids.edges :
+            
+            g.add_edge(e[0],e[1])
+            
+
+        g.set_options('''
+        var options = {
+            "layout": {
+                "hierarchical": {
+                    "enabled": true,
+                    "direction": "LR",  
+                    "sortMethod": "directed"
+                }
+            },
+            "physics": {
+                "enabled": false
+            }
+        }
+        ''')
+
+
+        
+
+        html_file_name = f'{name}_structure.html'
+        g.show( html_file_name)
+        
+
+        import re 
+        html_str = re.sub(r'<center>.+?<\/h1>\s+<\/center>', '', g.html, 1, re.DOTALL)
+        h = open( html_file_name,'w')
+        h.write(html_str)
+        h.close()
+        
+
+    def _draw(self) -> None:
         """
         Draws the Networkx directed graph.
         Args:
             k: parameter for the layout of the graph, the higher, the further the nodes apart
             display: display the layout created
             t: time to display in seconds
         """
@@ -399,21 +499,21 @@
             },
             "physics": {
                 "enabled": false
             }
         }
         ''')
 
-
-        #g.show('nx.html')
+        html_file_name = f'{self.name}_states_run.html'
+        g.show( html_file_name)
         
 
         import re 
         html_str = re.sub(r'<center>.+?<\/h1>\s+<\/center>', '', g.html, 1, re.DOTALL)
-        h = open(f'{self.name}_states_run.html','w')
+        h = open( html_file_name,'w')
         h.write(html_str)
         h.close()
 
         
 
     def execute(
         self, leaves_ids: Optional[List[Union[Hashable, ExecNode]]] = None
```

### Comparing `easydags-0.0.6/easydags/node.py` & `easydags-0.0.7/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.6/easydags/ops.py` & `easydags-0.0.7/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.6/easydags.egg-info/PKG-INFO` & `easydags-0.0.7/easydags.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -315,14 +315,98 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
+
+```python
+#See draw_ensemble.py
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    print('beginning pre pro')
+    time.sleep(3)
+    print('end pre pro')
+    return 'df with cool features'
+
+
+
+nodes.append( ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) )  
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+nodes.append( ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model1'
+              ) )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 78373'
+
+nodes.append( ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
+              output_name = 'model2'
+              ) )  
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+nodes.append( ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) )  
+
+
+
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+
+dag.only_draw(name = 'green dag')
+
+dag.only_draw(name = 'yellow dag', color = 'yellow')
+
+```
+
 
 ![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
 
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
```

### Comparing `easydags-0.0.6/setup.py` & `easydags-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.0.6',      # Start with a small number and increase it with every change you make
+  version = '0.0.7',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

