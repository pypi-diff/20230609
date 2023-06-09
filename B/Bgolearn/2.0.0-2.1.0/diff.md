# Comparing `tmp/Bgolearn-2.0.0.tar.gz` & `tmp/Bgolearn-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.0.0.tar", last modified: Sun Apr 23 02:21:21 2023, max compression
+gzip compressed data, was "Bgolearn-2.1.0.tar", last modified: Fri Jun  9 00:02:08 2023, max compression
```

## Comparing `Bgolearn-2.0.0.tar` & `Bgolearn-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.588804 Bgolearn-2.0.0/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.587920 Bgolearn-2.0.0/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.0.0/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.0.0/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.0.0/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.0.0/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    19956 2023-04-23 02:19:14.000000 Bgolearn-2.0.0/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      401 2023-04-07 02:04:26.000000 Bgolearn-2.0.0/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-04-23 02:21:21.588523 Bgolearn-2.0.0/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-04-23 02:21:21.000000 Bgolearn-2.0.0/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-04-23 02:21:21.588681 Bgolearn-2.0.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.0.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-04-23 02:21:21.588843 Bgolearn-2.0.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-04-23 02:19:25.000000 Bgolearn-2.0.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:02:08.789800 Bgolearn-2.1.0/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:02:08.788911 Bgolearn-2.1.0/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.1.0/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.1.0/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.1.0/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.1.0/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    21185 2023-06-08 23:59:56.000000 Bgolearn-2.1.0/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      344 2023-06-08 23:50:53.000000 Bgolearn-2.1.0/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:02:08.789502 Bgolearn-2.1.0/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:02:08.000000 Bgolearn-2.1.0/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-06-09 00:02:08.000000 Bgolearn-2.1.0/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-09 00:02:08.000000 Bgolearn-2.1.0/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-06-09 00:02:08.000000 Bgolearn-2.1.0/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-06-09 00:02:08.000000 Bgolearn-2.1.0/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:02:08.789672 Bgolearn-2.1.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.1.0/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-09 00:02:08.789842 Bgolearn-2.1.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-06-09 00:01:30.000000 Bgolearn-2.1.0/setup.py
```

### Comparing `Bgolearn-2.0.0/Bgolearn/BGO_eval.py` & `Bgolearn-2.1.0/Bgolearn/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.0.0/Bgolearn/BGOclf.py` & `Bgolearn-2.1.0/Bgolearn/BGOclf.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.0.0/Bgolearn/BGOmax.py` & `Bgolearn-2.1.0/Bgolearn/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.0.0/Bgolearn/BGOmin.py` & `Bgolearn-2.1.0/Bgolearn/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.0.0/Bgolearn/BGOsampling.py` & `Bgolearn-2.1.0/Bgolearn/BGOsampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,56 +12,16 @@
 from sklearn.metrics import r2_score
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_squared_error
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import  RBF, WhiteKernel
 from sklearn.model_selection import KFold
 
-
-def Bgo_KFold(x_train, y_train,cv):
-    x_train = np.array(x_train)
-    y_train = np.array(y_train)
-    kfolder = KFold(n_splits=cv, shuffle=True,random_state=0)
-    kfold = kfolder.split(x_train, y_train)
-    return kfold
-
-def docu_name(CV_test):
-    if CV_test == 'LOOCV':
-        return 'LOOCV'
-    elif type(CV_test) == int:
-        return '{}-CVs'.format(CV_test)
-    else:
-        print('type error')
-
-
-def Classifier_selection(Classifier):
-    if Classifier == 'GaussianProcess':
-        from sklearn.gaussian_process import GaussianProcessClassifier 
-        model = GaussianProcessClassifier(kernel= 1*RBF(1.0) ,random_state=0)
-    elif Classifier == 'LogisticRegression':
-        from sklearn.linear_model import LogisticRegression
-        model = LogisticRegression(random_state=0,class_weight='balanced',multi_class='multinomial')
-    elif Classifier == 'NaiveBayes':
-        from sklearn.naive_bayes import GaussianNB
-        model = GaussianNB()
-    elif Classifier == 'SVM':
-        from sklearn.svm import SVC
-        model = SVC(probability=True)
-    elif Classifier == 'RandomForest':
-        from sklearn.ensemble import RandomForestClassifier
-        model = RandomForestClassifier(max_depth=4,random_state=0)
-    else :
-        print('type ERROR! -Classifier-')
-    return model
-
-
-
-
 class Bgolearn(object):
-    def fit(self,data_matrix, Measured_response, virtual_samples, Mission ='Regression', Classifier = 'GaussianProcess',noise_std = 0.01, Kriging_model = None, opt_num = 1 ,min_search = True, CV_test = False, ):
+    def fit(self,data_matrix, Measured_response, virtual_samples, Mission ='Regression', Classifier = 'GaussianProcess',noise_std = None, Kriging_model = None, opt_num = 1 ,min_search = True, CV_test = False, ):
         
         """
         PACKAGE: Bayesian global optimization learn .
 
         6 Apr 2023, version 1.4, Bin Cao, ZheJiang LAB, Hangzhou, CHINA. (MGI, SHU, Shanghai, CHINA).
 
         :param data_matrix: data matrix of training dataset, X .
@@ -78,21 +38,24 @@
                 five different classifiers are pre-setd in Bgolearn:
                 'GaussianProcess' --> Gaussian Process Classifier (default)
                 'LogisticRegression' --> Logistic Regression
                 'NaiveBayes' --> Naive Bayes Classifier
                 'SVM' --> Support Vector Machine Classifier
                 'RandomForest' --> Random Forest Classifier
 
-        :param noise_std: float or ndarray of shape (n_samples,), default=0.01
+        :param noise_std: float or ndarray of shape (n_samples,), default=None
                 Value added to the diagonal of the kernel matrix during fitting.
                 This can prevent a potential numerical issue during fitting, by
                 ensuring that the calculated values form a positive definite matrix.
                 It can also be interpreted as the variance of additional Gaussian.
                 measurement noise on the training observations.
 
+                if noise_std is not None, a noise value will be estimated by maximum likelihood
+                on training dataset.
+
         :param Kriging_model (default None): a user defined callable Kriging model, has an attribute of <fit_pre>
                 if user isn't applied one, Bgolearn will call a pre-set Kriging model
                 atribute <fit_pre> : 
                 input -> xtrain, ytrain, xtest ; 
                 output -> predicted  mean and std of xtest
                 e.g. (take GaussianProcessRegressor in sklearn as an example):
                 class Kriging_model(object):
@@ -131,27 +94,44 @@
                 print('Type Error! Classifier should be one of the following:')
                 print('GaussianProcess; LogisticRegression;NaiveBayes;SVM;RandomForest')
 
 
         elif Mission == 'Regression':
         
             if Kriging_model == None:
-                kernel = RBF() + WhiteKernel()
-                if type(noise_std) == float:
+                kernel = 1 * RBF() 
+                if noise_std == None:
+                    # call the default model;
+                    class Kriging_model(object):
+                        def fit_pre(self,xtrain,ytrain,xtest,):
+                            # estimating Noise Level of training dataset
+                            noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.5))
+                            GPr = GaussianProcessRegressor(kernel= 1 * RBF()+noise_ker,normalize_y=True).fit(xtrain,ytrain)
+                            noise_level = np.exp(GPr.kernel_.theta[1])
+        
+                            # ret_std is a placeholder for homogenous noise
+                            # instantiated mode
+                            mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_level).fit(xtrain,ytrain)
+                            # defined the attribute's outputs
+                            mean,std = mdoel.predict(xtest,return_std=True)
+                            return mean,std 
+                    print('The internal model is instantiated with optimized homogenous noise: %s' % noise_std)  
+
+                elif type(noise_std) == float:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,):
                             # ret_std is a placeholder for homogenous noise
                             # instantiated mode
                             mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
                             # defined the attribute's outputs
                             mean,std = mdoel.predict(xtest,return_std=True)
                             return mean,std 
                     print('The internal model is instantiated with homogenous noise: %s' % noise_std)  
-                    
+                
                 elif type(noise_std) == np.ndarray:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,ret_std = 0.0):
                             # instantiated model
                             if len(xtrain) == len(noise_std):
                                 mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_std**2).fit(xtrain,ytrain)
@@ -397,7 +377,43 @@
         print('Evaluation is executed')
         
         Eval_model = BGO_Efficient(Ture_fun,Def_Domain, Kriging_model, opt_num, ret_noise,min_search)
         return Eval_model
       
   
 
+
+def Bgo_KFold(x_train, y_train,cv):
+    x_train = np.array(x_train)
+    y_train = np.array(y_train)
+    kfolder = KFold(n_splits=cv, shuffle=True,random_state=0)
+    kfold = kfolder.split(x_train, y_train)
+    return kfold
+
+def docu_name(CV_test):
+    if CV_test == 'LOOCV':
+        return 'LOOCV'
+    elif type(CV_test) == int:
+        return '{}-CVs'.format(CV_test)
+    else:
+        print('type error')
+
+
+def Classifier_selection(Classifier):
+    if Classifier == 'GaussianProcess':
+        from sklearn.gaussian_process import GaussianProcessClassifier 
+        model = GaussianProcessClassifier(kernel= 1*RBF(1.0) ,random_state=0)
+    elif Classifier == 'LogisticRegression':
+        from sklearn.linear_model import LogisticRegression
+        model = LogisticRegression(random_state=0,class_weight='balanced',multi_class='multinomial')
+    elif Classifier == 'NaiveBayes':
+        from sklearn.naive_bayes import GaussianNB
+        model = GaussianNB()
+    elif Classifier == 'SVM':
+        from sklearn.svm import SVC
+        model = SVC(probability=True)
+    elif Classifier == 'RandomForest':
+        from sklearn.ensemble import RandomForestClassifier
+        model = RandomForestClassifier(max_depth=4,random_state=0)
+    else :
+        print('type ERROR! -Classifier-')
+    return model
```

### Comparing `Bgolearn-2.0.0/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.1.0/Bgolearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.0.0/PKG-INFO` & `Bgolearn-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.0.0/README.md` & `Bgolearn-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.0.0/setup.py` & `Bgolearn-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='2.0.0',  # 版本
+    version='2.1.0',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

