# Comparing `tmp/BaseDT-0.0.6.tar.gz` & `tmp/BaseDT-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BaseDT-0.0.6.tar", last modified: Wed Jun  7 06:28:57 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.0.7.tar", last modified: Fri Jun  9 06:53:39 2023, max compression
```

## Comparing `BaseDT-0.0.6.tar` & `BaseDT-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.369519 BaseDT-0.0.6/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.365519 BaseDT-0.0.6/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.6/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    36851 2023-06-07 06:19:04.000000 BaseDT-0.0.6/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.6/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    12752 2023-06-06 05:32:46.000000 BaseDT-0.0.6/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.6/BaseDT/utils.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-07 06:28:57.369519 BaseDT-0.0.6/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-07 06:28:57.000000 BaseDT-0.0.6/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.6/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.6/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-07 06:28:57.369519 BaseDT-0.0.6/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.6/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-07 06:28:57.369519 BaseDT-0.0.6/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-07 06:14:46.000000 BaseDT-0.0.6/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.7/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37221 2023-06-09 06:53:01.000000 BaseDT-0.0.7/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12752 2023-06-06 05:32:46.000000 BaseDT-0.0.7/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.7/BaseDT/utils.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.7/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.7/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-09 06:53:39.000000 BaseDT-0.0.7/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.7/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-09 06:53:39.000000 BaseDT-0.0.7/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-09 06:53:21.000000 BaseDT-0.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `BaseDT-0.0.6/BaseDT/data.py` & `BaseDT-0.0.7/BaseDT/data.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.6/BaseDT/data_image.py` & `BaseDT-0.0.7/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.6/BaseDT/dataset.py` & `BaseDT-0.0.7/BaseDT/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,15 +739,15 @@
             try:
                 self.check_cls()
                 self.print_folder_structure(self.dataset_path)
             except Exception as e:
                 print(e)
 
 
-def split_tab_dataset(data_path, data_column,label_column=[-1],train_val_ratio=0.8,random_seed=42):
+def split_tab_dataset(data_path, data_column,label_column=[-1],train_val_ratio=0.8,random_seed=42,normalize=False):
 
     # 读取提取后的特征和标签
     data = np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=data_column)
     label =  np.loadtxt(data_path, dtype=float, delimiter=',',skiprows=1,usecols=label_column)
 
     # 设置随机种子，以获得可复现的划分结果
     np.random.seed(random_seed)
@@ -776,14 +776,19 @@
     if len(train_y.shape) == 1:
         train_y = train_y.reshape(-1,1)
     if len(val_x.shape) == 1:
         val_x = val_x.reshape(-1,1)
     if len(val_y.shape) == 1:
         val_y = val_y.reshape(-1,1)
     # print(len(train_x.shape),len(train_y.shape))
+    if normalize == True:
+        from sklearn.preprocessing import MinMaxScaler
+        scaler = MinMaxScaler()
+        train_x = scaler.fit_transform(train_x)
+        val_x = scaler.transform(val_x)
 
     data_np_train = np.concatenate((train_x, train_y), axis=1)
     # print(data_np_train)
     data_np_val = np.concatenate((val_x, val_y), axis=1)
     # # 添加表头
     if isinstance(data_column, int):
         len_data = 1
@@ -866,7 +871,12 @@
     train_file = file_name[0]+"_train."+file_name[1]
     val_file = file_name[0]+"_val."+file_name[1]
     np.savetxt(train_file, train_data_with_header, delimiter=",", fmt="%s")
     np.savetxt(val_file, val_data_with_header, delimiter=",", fmt="%s")
 
     return train_x,train_y, val_x, val_y
 
+if __name__=="__main__":
+    path = "../iris/iris.csv"
+    train_x,train_y,val_x,val_y = split_tab_dataset(path,data_column=range(0,4),label_column=4)
+
+
```

### Comparing `BaseDT-0.0.6/BaseDT/io.py` & `BaseDT-0.0.7/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.6/BaseDT/plot.py` & `BaseDT-0.0.7/BaseDT/plot.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.6/BaseDT/utils.py` & `BaseDT-0.0.7/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.6/setup.py` & `BaseDT-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.6',
+    version='0.0.7',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

