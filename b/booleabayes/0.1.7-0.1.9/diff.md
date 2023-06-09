# Comparing `tmp/booleabayes-0.1.7.tar.gz` & `tmp/booleabayes-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/smgroves/Documents/GitHub/BooleaBayes/dist/tmprxcjxfc_/booleabayes-0.1.7.tar", last modified: Thu Nov 10 15:44:32 2022, max compression
+gzip compressed data, was "/Users/smgroves/Documents/GitHub/BooleaBayes/dist/.tmp-ost8bm5r/booleabayes-0.1.9.tar", last modified: Thu Dec 22 22:28:39 2022, max compression
```

## Comparing `booleabayes-0.1.7.tar` & `booleabayes-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-11-10 15:44:32.000000 booleabayes-0.1.7/
--rw-r--r--   0 smgroves   (501) staff       (20)     1065 2022-06-30 16:32:09.000000 booleabayes-0.1.7/LICENSE
--rw-r--r--   0 smgroves   (501) staff       (20)     1862 2022-11-10 15:44:32.000000 booleabayes-0.1.7/PKG-INFO
--rw-r--r--   0 smgroves   (501) staff       (20)     1240 2022-09-23 03:13:28.000000 booleabayes-0.1.7/README.rst
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes/
--rw-r--r--   0 smgroves   (501) staff       (20)      192 2022-09-23 02:41:13.000000 booleabayes-0.1.7/booleabayes/__init__.py
--rw-r--r--   0 smgroves   (501) staff       (20)    11152 2020-04-16 16:10:22.000000 booleabayes-0.1.7/booleabayes/enrichr.py
--rw-r--r--   0 smgroves   (501) staff       (20)     9788 2022-11-10 06:01:18.000000 booleabayes-0.1.7/booleabayes/load.py
--rw-r--r--   0 smgroves   (501) staff       (20)     6912 2022-10-19 17:23:58.000000 booleabayes-0.1.7/booleabayes/make_tf_network.py
--rw-r--r--   0 smgroves   (501) staff       (20)    47610 2022-11-10 15:43:10.000000 booleabayes-0.1.7/booleabayes/plot.py
--rw-r--r--   0 smgroves   (501) staff       (20)     3766 2022-09-23 02:39:34.000000 booleabayes-0.1.7/booleabayes/proc.py
--rw-r--r--   0 smgroves   (501) staff       (20)    23817 2022-11-10 15:22:00.000000 booleabayes-0.1.7/booleabayes/rw.py
--rw-r--r--   0 smgroves   (501) staff       (20)    34895 2022-11-10 15:43:11.000000 booleabayes-0.1.7/booleabayes/tl.py
--rw-r--r--   0 smgroves   (501) staff       (20)    24708 2022-11-10 15:42:35.000000 booleabayes-0.1.7/booleabayes/utils.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/
--rw-r--r--   0 smgroves   (501) staff       (20)     1862 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/PKG-INFO
--rw-r--r--   0 smgroves   (501) staff       (20)      429 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/SOURCES.txt
--rw-r--r--   0 smgroves   (501) staff       (20)        1 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/dependency_links.txt
--rw-r--r--   0 smgroves   (501) staff       (20)      172 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/requires.txt
--rw-r--r--   0 smgroves   (501) staff       (20)       18 2022-11-10 15:44:32.000000 booleabayes-0.1.7/booleabayes.egg-info/top_level.txt
--rw-r--r--   0 smgroves   (501) staff       (20)       80 2022-09-22 23:20:35.000000 booleabayes-0.1.7/pyproject.toml
--rw-r--r--   0 smgroves   (501) staff       (20)       38 2022-11-10 15:44:32.000000 booleabayes-0.1.7/setup.cfg
--rw-r--r--   0 smgroves   (501) staff       (20)     1446 2022-11-10 15:43:47.000000 booleabayes-0.1.7/setup.py
-drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-11-10 15:44:32.000000 booleabayes-0.1.7/tests/
--rw-r--r--   0 smgroves   (501) staff       (20)        0 2022-11-04 21:47:16.000000 booleabayes-0.1.7/tests/__init__.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-12-22 22:28:39.000000 booleabayes-0.1.9/
+-rw-r--r--   0 smgroves   (501) staff       (20)     1065 2022-06-30 16:32:09.000000 booleabayes-0.1.9/LICENSE
+-rw-r--r--   0 smgroves   (501) staff       (20)     1863 2022-12-22 22:28:39.000000 booleabayes-0.1.9/PKG-INFO
+-rw-r--r--   0 smgroves   (501) staff       (20)     1242 2022-12-22 22:27:49.000000 booleabayes-0.1.9/README.rst
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes/
+-rw-r--r--   0 smgroves   (501) staff       (20)      192 2022-09-23 02:41:13.000000 booleabayes-0.1.9/booleabayes/__init__.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    11152 2020-04-16 16:10:22.000000 booleabayes-0.1.9/booleabayes/enrichr.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     9788 2022-11-10 06:01:18.000000 booleabayes-0.1.9/booleabayes/load.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     6948 2022-12-22 22:21:57.000000 booleabayes-0.1.9/booleabayes/make_tf_network.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    50434 2022-11-11 00:09:05.000000 booleabayes-0.1.9/booleabayes/plot.py
+-rw-r--r--   0 smgroves   (501) staff       (20)     3766 2022-09-23 02:39:34.000000 booleabayes-0.1.9/booleabayes/proc.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    23807 2022-11-10 16:09:36.000000 booleabayes-0.1.9/booleabayes/rw.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    37608 2022-11-10 23:04:58.000000 booleabayes-0.1.9/booleabayes/tl.py
+-rw-r--r--   0 smgroves   (501) staff       (20)    28009 2022-12-22 20:51:02.000000 booleabayes-0.1.9/booleabayes/utils.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/
+-rw-r--r--   0 smgroves   (501) staff       (20)     1863 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/PKG-INFO
+-rw-r--r--   0 smgroves   (501) staff       (20)      429 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/SOURCES.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)        1 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/dependency_links.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)      172 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/requires.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)       18 2022-12-22 22:28:39.000000 booleabayes-0.1.9/booleabayes.egg-info/top_level.txt
+-rw-r--r--   0 smgroves   (501) staff       (20)       80 2022-09-22 23:20:35.000000 booleabayes-0.1.9/pyproject.toml
+-rw-r--r--   0 smgroves   (501) staff       (20)       38 2022-12-22 22:28:39.000000 booleabayes-0.1.9/setup.cfg
+-rw-r--r--   0 smgroves   (501) staff       (20)     1446 2022-12-22 22:28:03.000000 booleabayes-0.1.9/setup.py
+drwxr-xr-x   0 smgroves   (501) staff       (20)        0 2022-12-22 22:28:39.000000 booleabayes-0.1.9/tests/
+-rw-r--r--   0 smgroves   (501) staff       (20)        0 2022-11-04 21:47:16.000000 booleabayes-0.1.9/tests/__init__.py
```

### Comparing `booleabayes-0.1.7/LICENSE` & `booleabayes-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `booleabayes-0.1.7/PKG-INFO` & `booleabayes-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booleabayes
-Version: 0.1.7
+Version: 0.1.9
 Summary: A suite for network inference from transcriptomics data
 Home-page: https://github.com/smgroves/BooleaBayes
 Author: Sarah Groves
 Author-email: sarahmaddoxgroves@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -44,7 +44,8 @@
 * ``net`` = make or modify network structure
 * ``load`` = loading data
 * ``proc`` = processing
 * ``rw`` = random walk
 * ``plot`` = plotting
 * ``tl`` = tools
 * ``utils`` = utilities
+
```

### Comparing `booleabayes-0.1.7/README.rst` & `booleabayes-0.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 
 * ``net`` = make or modify network structure
 * ``load`` = loading data
 * ``proc`` = processing
 * ``rw`` = random walk
 * ``plot`` = plotting
 * ``tl`` = tools
-* ``utils`` = utilities
+* ``utils`` = utilities
+
```

### Comparing `booleabayes-0.1.7/booleabayes/enrichr.py` & `booleabayes-0.1.9/booleabayes/enrichr.py`

 * *Files identical despite different names*

### Comparing `booleabayes-0.1.7/booleabayes/load.py` & `booleabayes-0.1.9/booleabayes/load.py`

 * *Files identical despite different names*

### Comparing `booleabayes-0.1.7/booleabayes/make_tf_network.py` & `booleabayes-0.1.9/booleabayes/make_tf_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,41 +83,41 @@
     #                if len(edges[target]['db']) < 2: G.remove_edge(tf, target)
     return prune(G)
 
 
 def make_network(
     tfs,
     outdir="",
-    prune=True,
+    do_prune=True,
     prune_sinks=True,
     prune_sources=True,
-    prune_info=True,
+    do_prune_info=True,
     prune_self_loops=True,
-    prune_to_chea=True,
+    do_prune_to_chea=True,
     save_unfiltered=False,
     network_name="network",
 ):
     """Make network from list of tfs and save as csv files with various levels of pruning.
 
     :param tfs: List of transcription factor gene names that will be searched in enrichR databases.
     :type tfs: List[str]
     :param outdir: Output directory where network csvs will be saved, defaults to ""
     :type outdir: str or None
-    :param prune: Prune network to remove nodes with no sinks and/or sources and generate a new network file called <network_name>_pruned.csv, defaults to True
-    :type prune: bool, optional
+    :param do_prune: Prune network to remove nodes with no sinks and/or sources and generate a new network file called <network_name>_pruned.csv, defaults to True
+    :type do_prune: bool, optional
     :param prune_sinks: Whether to prune sink nodes from the network (no outgoing nodes), defaults to True
     :type prune_sinks: bool, optional
     :param prune_sources: Whether to prune source nodes the network (no incoming nodes), defaults to True
     :type prune_sources: bool, optional
-    :param prune_info: Whether to prune the network to edges with evidence in more than one database from enrichR and generate a new network file called <network_name>_high_evidence.csv, defaults to True
-    :type prune_info: bool, optional
+    :param do_prune_info: Whether to prune the network to edges with evidence in more than one database from enrichR and generate a new network file called <network_name>_high_evidence.csv, defaults to True
+    :type do_prune_info: bool, optional
     :param prune_self_loops: Whether to prune self-loops in the network (edges where parent node == child node), defaults to True
     :type prune_self_loops: bool, optional
-    :param prune_to_chea: Whether to prune the network to only edges with evidence in ChEA databases and generate a new network file called <network_name>_chea.csv, defaults to True
-    :type prune_to_chea: bool, optional
+    :param do_prune_to_chea: Whether to prune the network to only edges with evidence in ChEA databases and generate a new network file called <network_name>_chea.csv, defaults to True
+    :type do_prune_to_chea: bool, optional
     :param save_unfiltered: Whether to save the unfiltered network before pruning, defaults to False. Note that if all pruning options are False and this is set to False, no network will be saved.
     :type save_unfiltered: bool, optional
     :param network_name: Prefix name of network csv files, defaults to `network`
     :type network_name: str
     :return: Network with highest level of pruning
     :rtype: NetworkX Graph
     """
@@ -145,41 +145,41 @@
             os.path.join(outdir, f"{network_name}_unfiltered.csv"),
             "w",
         )
         for edge in G.edges():
             outfile.write("%s,%s\n" % (edge[0], edge[1]))
         outfile.close()
 
-    if prune:
+    if do_prune:
         Gp = prune(G, prune_sinks=prune_sinks, prune_sources=prune_sources)
 
         outfile = open(
             os.path.join(outdir, f"{network_name}_pruned.csv"),
             "w",
         )
         for edge in Gp.edges():
             outfile.write("%s,%s\n" % (edge[0], edge[1]))
         outfile.close()
     else:
         Gp = G
 
-    if prune_info:
+    if do_prune_info:
         Gpp = prune_info(Gp, prune_self_loops=prune_self_loops)
 
         outfile = open(
             os.path.join(outdir, f"{network_name}_high_evidence.csv"),
             "w",
         )
         for edge in Gpp.edges():
             outfile.write("%s,%s\n" % (edge[0], edge[1]))
         outfile.close()
     else:
         Gpp = Gp
 
-    if prune_to_chea:
+    if do_prune_to_chea:
         Gppp = prune_to_chea(Gpp, prune_self_loops=prune_self_loops)
 
         outfile = open(
             os.path.join(outdir, f"{network_name}_chea.csv"),
             "w",
         )
         for edge in Gppp.edges():
```

### Comparing `booleabayes-0.1.7/booleabayes/plot.py` & `booleabayes-0.1.9/booleabayes/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,70 @@
 import glob
 import networkx as nx
 from graph_tool import all as gt
 
 
 ### ------------ ACCURACY PLOTS ------------ ###
 
+def plot_sklearn_summ_stats(summary_stats, VAL_DIR, fname = ""):
+    df = pd.melt(summary_stats, id_vars='gene')
+    df = df.astype({'variable':'string'})
+    q1 = df.groupby(df.variable).quantile(0.25)['value']
+    q3 = df.groupby(df.variable).quantile(0.75)['value']
+    outlier_top_lim = q3 + 1.5 * (q3 - q1)
+    outlier_bottom_lim = q1 - 1.5 * (q3 - q1)
+    plt.figure()
+    sns.boxplot(x="variable", y="value", data=pd.melt(summary_stats.drop('gene', axis = 1)))
+    col_dict = {i:j for i,j in zip(summary_stats.drop('gene', axis = 1).columns,range(len(summary_stats.columns)-1))}
+    for row in df.itertuples():
+        variable = row.variable
+        val = row.value
+        if (val > outlier_top_lim[variable]) or (val < outlier_bottom_lim[variable]):
+            print(val, row.gene)
+            plt.annotate(s = row.gene, xy = (col_dict[variable]+0.1,val), fontsize = 8)
+    plt.xticks(rotation = 45, ha = 'right')
+    plt.xlabel("Model Metric")
+    plt.ylabel("Score")
+    plt.title("Metrics for BooleaBayes Rule Fitting across All TFs")
+    plt.tight_layout()
+    plt.savefig(f"{VAL_DIR}/summary_stats_boxplot{fname}.pdf")
+    
+def plot_sklearn_metrics(VAL_DIR, show = False, save = True):
+    try:
+        summary_stats = pd.read_csv(f"{VAL_DIR}/summary_stats.csv", header = 0, index_col=0)
+    except FileNotFoundError:
+        print("You must run tl.get_sklearn_metrics first.")
+    if save:
+        try:
+            os.mkdir(f"{VAL_DIR}/summary_plots")
+        except FileExistsError:
+            pass
+    metric_dict = {'accuracy':{"Best":'1', "Worst":'0'},
+                   'balanced_accuracy_score':{"Best":'1', "Worst":'0'},
+                   'f1':{"Best":'1', "Worst":'0'},
+                   'roc_auc_score':{"Best":'1', "Worst":'0'},
+                   "precision":{"Best":'1', "Worst":'0'},
+                   "recall":{"Best":'1', "Worst":'0'},
+                   "explained_variance":{"Best":'1', "Worst":'0'},
+                   'max_error':{"Best":'0', "Worst":"High"},
+                   'r2':{"Best":'1', "Worst":'0'},
+                   'log-loss':{"Best":"Low", "Worst":"High"}}
+    for c in sorted(list(set(summary_stats.columns).difference({'gene'}))):
+        print(c)
+        plt.figure(figsize = (20,8))
+        my_order = summary_stats.sort_values(c)['gene'].values
+        sns.barplot(data = summary_stats, x = 'gene', y = c, order = my_order)
+        plt.xticks(rotation = 90, fontsize = 8)
+        plt.ylabel(f"{c.capitalize()} (Best: {metric_dict[c]['Best']}, Worst: {metric_dict[c]['Worst']})")
+        plt.title(c.capitalize())
+        if show:
+            plt.show()
+        if save:
+            plt.savefig(f"{VAL_DIR}/summary_plots/{c}.pdf")
+            plt.close()
 
 def plot_roc(
     fprs, tprs, area, node, save=False, save_dir=None,  show_plot=True
 ):
     fig = plt.figure()
     ax = plt.subplot()
     plt.plot(fprs, tprs, "-", marker="o")
@@ -720,42 +776,47 @@
         if rescaled:
             norm_df = df.copy()[['cluster', 'attr', 'radius', 'mean']]
             df_agg = df.groupby(['cluster','radius']).agg('mean')
             norm = df_agg.xs('random', level = 'cluster')
             for i,r in norm.iterrows():
                 norm_df.loc[norm_df['radius']==i,'mean'] = norm_df.loc[norm_df['radius']==i,'mean']/r["mean"]
             norm_df = norm_df.sort_values(by = "cluster")
+            plt.figure()
             sns.lineplot(x = 'radius',y = 'mean',err_style=err_style,hue = 'cluster', palette=colormap,
                          data = norm_df, markers = True)
             plt.legend(bbox_to_anchor=(1.05, 1), loc='upper left', borderaxespad=0, title = "Attractor Subtypes")
 
             plt.xticks(list(np.unique(norm_df['radius'])))
             plt.xlabel("Radius of Basin")
-            plt.ylabel("Scaled mean number of steps to leave basin (Fold-change from control mean)")
+            plt.ylabel(f"Scaled Mean number of steps to leave basin \n (Fold-change from control mean)")
             plt.title("Scaled Stability of Attractors by Subtype")
             plt.tight_layout()
             if show:
                 plt.show()
             if save:
                 plt.savefig(f"{walks_dir}/scaled_stability_plot.pdf")
+                plt.close()
 
     df = df.sort_values(by = "cluster")
+    plt.figure()
     sns.lineplot(x = 'radius',y = 'mean',err_style=err_style,hue = 'cluster', palette=colormap,
                       data = df, markers = True)
     plt.legend(bbox_to_anchor=(1.05, 1), loc='upper left', borderaxespad=0, title = "Attractor Subtypes")
 
     plt.xticks(list(np.unique(df['radius'])))
     plt.xlabel("Radius of Basin")
     plt.ylabel("Mean number of steps to leave basin")
     plt.title("Stability of Attractors by Subtype")
     plt.tight_layout()
     if show:
         plt.show()
     if save:
         plt.savefig(f"{walks_dir}/stability_plot.pdf")
+        plt.close()
+    return df
 
 # att_list = list of attractor states
 # phenotypes = list of phenotypes
 # phenotype_color = should be st by the function; user can pass in customPallete instead
 # radius = radius used for the walk
 # num_paths = max number of paths to plot? i think
 # PCA graphs **
```

### Comparing `booleabayes-0.1.7/booleabayes/proc.py` & `booleabayes-0.1.9/booleabayes/proc.py`

 * *Files identical despite different names*

### Comparing `booleabayes-0.1.7/booleabayes/rw.py` & `booleabayes-0.1.9/booleabayes/rw.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,14 @@
                                     "perturbations/%d,%s,%s,knockdown,%f\n"
                                     % (start_idx, k, expt_node, stabilized),
                                 )
                             )
                         outfile.close()
     
     if random_start > 0:
-        print(save_dir)
         try:
             os.mkdir(f"{save_dir}/walks/random")
         except FileExistsError:
             pass
         random_list = []
         for i in range(random_start):
             rand_state = random.choices([0,1], k=len(nodes))
@@ -348,16 +347,16 @@
 
                 # Perform walks without perturbations first
                 # Print progress of random walk every 10% of the way through iters
                 prog = 0
                 for iter_ in range(iters):
                     # print("Iteration:", iter_)
                     # print("Progress:")
-                    if iter_ % 100 == 0:
-                        prog = iter_ / 10
+                    if iter_/iters*100 % 10 == 0:
+                        prog = iter_/iters*100
                         print("Progress: ", prog)
 
                     # 'counts': histogram of walk
                     # 'switches': count which TFs flipped
                     # 'distance': starting state to current state; walk until take max steps or leave basin
                     if reach_or_leave == "leave":
                         (
```

### Comparing `booleabayes-0.1.7/booleabayes/tl.py` & `booleabayes-0.1.9/booleabayes/tl.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from matplotlib.patches import Patch
 import matplotlib.gridspec as gridspec
 import matplotlib.pyplot as plt
 import sklearn.model_selection as ms
 from scipy.stats import mannwhitneyu
 from statsmodels.stats.multitest import multipletests
 import json
+from sklearn.metrics import *
 
 
 ### ------------ RULE FITTING ----------- ###
 
 
 def reorder_binary_decision_tree(old_regulator_order, regulators):
     n = len(regulators)
@@ -520,15 +521,15 @@
         outfile.write(f"{nodes[n]},{a} \n")
     outfile.close()
 
 
 # Function to run fit validation
 # first runs plot_acuracy(_scvelo)() to get validation dataframe
 # then it calculates roc giving the user the option to plot and save the dataframes and/or plots
-# val_type = validation type; use the plot scvelo accuracy funrction or just the plot_accuracy function
+# val_type = validation type; use the plot scvelo accuracy function or just the plot_accuracy function
 # fname = optional name to append to default file save name
 # returns: validation, tprs_all, fprs_all, and area_all
 def fit_validation(
     data_test,
     nodes,
     regulators_dict,
     rules,
@@ -630,14 +631,62 @@
         )
         tpr_all[node] = tprs
         fpr_all[node] = fprs
         area_all.append(area)
     return tpr_all, fpr_all, area_all
 
 
+def get_sklearn_metrics(VAL_DIR, plot_cm = True, show = False, save = True, save_stats = True):
+    files = glob.glob(f"{VAL_DIR}/accuracy_plots/*.csv")
+    summary_stats = pd.DataFrame(columns = ['gene','accuracy','balanced_accuracy_score','f1','roc_auc_score', "precision",
+                                                "recall", "explained_variance", 'max_error', 'r2','log-loss'])
+    if len(files) == 0:
+        print("You must first run tl.fit_validation() to generate the appropriate files.")
+        return summary_stats
+    else:
+
+        for f in files:
+            val_df = pd.read_csv(f, header = 0, index_col=0)
+            val_df['actual_binary'] = [{True:1, False:0}[x] for x in val_df['actual']> 0.5]
+            val_df['predicted_binary'] = [{True:1, False:0}[x] for x in val_df['predicted']> 0.5]
+            gene = f.split("/")[-1].split("_")[0]
+            #classification stats
+            acc = accuracy_score(val_df['actual_binary'], val_df['predicted_binary'])
+            bal_acc = balanced_accuracy_score(val_df['actual_binary'], val_df['predicted_binary'])
+            f1 = f1_score(val_df['actual_binary'], val_df['predicted_binary'])
+            prec = precision_score(val_df['actual_binary'], val_df['predicted_binary'])
+            rec = recall_score(val_df['actual_binary'], val_df['predicted_binary'])
+
+            #regression stats
+            roc_auc = roc_auc_score(val_df['actual_binary'], val_df['predicted'])
+            expl_var = explained_variance_score(val_df['actual'], val_df['predicted'])
+            max_err = max_error(val_df['actual'], val_df['predicted'])
+            r2 = r2_score(val_df['actual'], val_df['predicted'])
+            ll = log_loss(val_df['actual_binary'], val_df['predicted'])
+
+            summary_stats = summary_stats.append(pd.Series([gene, acc, bal_acc,f1,roc_auc,prec,rec,expl_var,max_err,r2,ll],
+                                                        index=summary_stats.columns),ignore_index=True)
+            if plot_cm:
+                plt.figure()
+                cm = confusion_matrix(val_df['actual_binary'], val_df['predicted_binary'])
+                disp = ConfusionMatrixDisplay(confusion_matrix=cm)
+                disp.plot(cmap = "Blues")
+                plt.title(gene)
+                if show:
+                    plt.show()
+                if save:
+                    plt.savefig(f"{VAL_DIR}/accuracy_plots/{gene}_confusion_matrix.pdf")
+                    plt.close()
+        
+        summary_stats = summary_stats.sort_values('gene').reset_index().drop("index",axis = 1)
+
+        if save_stats:
+            summary_stats.to_csv(f"{VAL_DIR}/summary_stats.csv")
+        return summary_stats
+
 ### ------------ ATTRACTORS ------------ ###
 
 # tf_basin --> if -1, use average distance between clusters. otherwise use the same size basin for all phenotypes
 def find_attractors(
     binarized_data,
     rules,
     nodes,
```

### Comparing `booleabayes-0.1.7/booleabayes/utils.py` & `booleabayes-0.1.9/booleabayes/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -616,8 +616,78 @@
         attr = pd.read_csv(f'{ATTRACTOR_DIR}/attractors_unfiltered.txt', sep = ',', header = 0, index_col = 0)
     for i,r in attr.iterrows():
         attractor_dict[i] = []
 
     for i,r in attr.iterrows():
         attractor_dict[i].append(state_bool2idx(list(r)))
     
-    return attractor_dict
+    return attractor_dict
+
+def print_graph_info(graph, vertex_dict, nodes, fname, brcd = "", dir_prefix = "", plot = True,
+                     fillcolor = 'lightcyan', gene2color = None, layout = None, add_edge_weights = True,
+                     ew_df = None):
+    print("==================================")
+    print("Graph properties")
+    print("==================================")
+    print(graph)
+    # print("Edge and vertex properties: ", graph.list_properties())
+    print("Number of nodes:", len(nodes))
+    print('Nodes: ', nodes)
+    sources = []
+    sinks = []
+    for i in range(len(nodes)):
+        if graph.vp.source[i] == 1: sources.append(graph.vp.name[i])
+        if graph.vp.sink[i] == 1: sinks.append(graph.vp.name[i])
+    print("Sources: ", len(sources), sources)
+    print("Sinks: ",len(sinks), sinks)
+
+    #treat network as if it is undirected to ensure largest component includes all nodes and edges
+    u = gt.extract_largest_component(graph, directed=False)
+    print("Network is a single connected component: ", gt.isomorphism(graph,u))
+    if gt.isomorphism(graph,u) == False:
+        print("\t Largest component of network: ")
+        print("\t", u)
+    print("Directed acyclic graph: ", gt.is_DAG(graph))
+    print("==================================")
+
+    if plot:
+        vertex2gene = graph.vertex_properties['name']
+        vertex_colors = fillcolor
+        if gene2color is not None:
+            vertex_colors = graph.new_vertex_property("string")
+            for gene in gene2color.keys():
+                vertex_colors[vertex_dict[gene]] = gene2color[gene]
+        edge_weights = graph.new_edge_property("float")
+        edge_color = graph.new_edge_property("vector<float>")
+
+        for edge in graph.edges():
+            edge_weights[edge] = 0.2
+            edge_color[edge] = [0,0,0,1]
+
+        if add_edge_weights:
+            min_ew = np.min(ew_df['score'])
+            max_ew = np.max(ew_df['score'])
+
+            for edge in graph.edges():
+                vs, vt = edge.source(), edge.target()
+                source = vertex2gene[vs]
+                target = vertex2gene[vt]
+                w = float(2*(np.mean(ew_df.loc[(ew_df['source']==source)&(ew_df['target']==target)]['score'].values)-min_ew)/max_ew+0.2)
+                if np.isnan(w):
+                    edge_weights[edge] = .2
+                    edge_color[edge] = [0,0,0,.1]
+                else:
+                    edge_weights[edge] = w
+                    edge_color[edge] = [0,0,0,(w-0.2)/2]
+
+        graph.edge_properties["edge_weights"] = edge_weights
+        graph.edge_properties["edge_color"] = edge_color
+        vprops = {"text": vertex2gene, "shape": "circle", "size": 20, "pen_width": 1, 'fill_color': vertex_colors}
+        eprops = {"color": edge_color}
+
+        if layout == 'circle':
+            state = gt.minimize_nested_blockmodel_dl(graph, B_min = 10)
+            state.draw(vprops=vprops,output=f"{dir_prefix}/{brcd}/{fname}_simple_circle_network.pdf", output_size=(1000, 1000))  # mplfig=ax[0,1])
+        else:
+            pos = gt.sfdp_layout(graph, mu = 1, eweight=edge_weights, max_iter=1000)
+            gt.graph_draw(graph, pos=pos, vprops = vprops, eprops = eprops, edge_pen_width = edge_weights, output=f"{dir_prefix}/{brcd}/{fname}_simple_network.pdf", output_size=(1000, 1000))
+
```

### Comparing `booleabayes-0.1.7/booleabayes.egg-info/PKG-INFO` & `booleabayes-0.1.9/booleabayes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booleabayes
-Version: 0.1.7
+Version: 0.1.9
 Summary: A suite for network inference from transcriptomics data
 Home-page: https://github.com/smgroves/BooleaBayes
 Author: Sarah Groves
 Author-email: sarahmaddoxgroves@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -44,7 +44,8 @@
 * ``net`` = make or modify network structure
 * ``load`` = loading data
 * ``proc`` = processing
 * ``rw`` = random walk
 * ``plot`` = plotting
 * ``tl`` = tools
 * ``utils`` = utilities
+
```

### Comparing `booleabayes-0.1.7/setup.py` & `booleabayes-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 readme = open("README.rst").read()
 
 
 setup(
     name="booleabayes",
-    version="0.1.7",
+    version="0.1.9",
     description="A suite for network inference from transcriptomics data",
     long_description=readme,
     long_description_content_type="text/x-rst",
     author="Sarah Groves",
     author_email="sarahmaddoxgroves@gmail.com",
     url="https://github.com/smgroves/BooleaBayes",
     install_requires=install_requires,
```

