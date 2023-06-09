# Comparing `tmp/TorchSisso-1.0.8.tar.gz` & `tmp/TorchSisso-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.8.tar", last modified: Thu Jun  8 12:10:52 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.9.tar", last modified: Fri Jun  9 14:26:49 2023, max compression
```

## Comparing `TorchSisso-1.0.8.tar` & `TorchSisso-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-08 12:10:52.213169 TorchSisso-1.0.8/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-08 12:10:52.212169 TorchSisso-1.0.8/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-08 12:10:52.191175 TorchSisso-1.0.8/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    18335 2023-06-08 11:26:56.000000 TorchSisso-1.0.8/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8313 2023-06-07 17:42:10.000000 TorchSisso-1.0.8/TorchSisso/SISSO_REGRESSOR_TORCH.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      228 2023-06-08 12:10:38.000000 TorchSisso-1.0.8/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5879 2023-06-08 12:06:17.000000 TorchSisso-1.0.8/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-08 12:10:52.209159 TorchSisso-1.0.8/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-08 12:10:51.000000 TorchSisso-1.0.8/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      303 2023-06-08 12:10:52.000000 TorchSisso-1.0.8/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-08 12:10:51.000000 TorchSisso-1.0.8/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-08 12:10:51.000000 TorchSisso-1.0.8/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-08 12:10:51.000000 TorchSisso-1.0.8/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-08 12:10:52.214164 TorchSisso-1.0.8/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-08 12:10:01.000000 TorchSisso-1.0.8/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.128782 TorchSisso-1.0.9/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-09 14:26:49.126790 TorchSisso-1.0.9/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.108788 TorchSisso-1.0.9/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    18780 2023-06-09 14:13:32.000000 TorchSisso-1.0.9/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8511 2023-06-09 14:15:23.000000 TorchSisso-1.0.9/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      228 2023-06-08 12:10:38.000000 TorchSisso-1.0.9/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5407 2023-06-09 14:24:20.000000 TorchSisso-1.0.9/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.123787 TorchSisso-1.0.9/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      303 2023-06-09 14:26:49.000000 TorchSisso-1.0.9/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-09 14:26:49.128788 TorchSisso-1.0.9/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-09 14:26:42.000000 TorchSisso-1.0.9/setup.py
```

### Comparing `TorchSisso-1.0.8/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.9/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     # Get the names of the zero variance columns
     zero_var_cols = variance[variance == 0].index
 
     # Drop the zero variance columns from the dataframe
     self.df = self.df.drop(zero_var_cols, axis=1)
 
     self.df.rename(columns = {f'{self.df.columns[0]}':'Target'},inplace=True)
-    self.Target_column = self.df.pop('Target')
+    self.Target_column = torch.tensor(self.df.pop('Target')).to(self.device)
 
     # Get the column values and convert it to tensor 
     self.df_feature_values = torch.tensor(self.df.values).to(self.device)
     #Create a dataframe for appending new datavalues 
     self.new_features_values = pd.DataFrame()
 
     #Get the column headers 
@@ -234,14 +234,15 @@
 
   ##########################################################################################################
 
   '''
 
   def feature_space(self):
     #based on the dimension we will be performing the feature space creation
+    if self.no_of_operators+1 > 9: print('****************************************************** \n','Currently TorchSisso supports Feature Space Expansion till complexity of 7, provided input argument > 7. Featureee Expansion with complexity of 7 will be returned \n', '*******************************************************')
     start_time = time.time()
     basic_operators = [op for op in self.operators if op in ['+', '-', '*', '/']]
     other_operators = [op for op in self.operators if op not in ['+', '-', '*', '/']]
     
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     #Merging two dataframes
@@ -253,135 +254,133 @@
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
+    del space_created,values,values1
     self.columns = self.columns + names + names1 
+    del names, names1
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
     space = space.round(7)
     space = space.T.drop_duplicates().T
-    del space_created
-    del values, values1, names, names1
+    space = space.dropna(axis=1, how='any')
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
-    print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
+    del space_created_2,space
+    print('Second Feature Space building is completed with features count: ',int(self.df_feature_values.shape[1]))
     print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
           start = time.time()
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
           #space_created_3 = torch.cat((values,self.df_feature_values),dim=1).to(self.device)
-          del space_created_2
+          del values,values1
           self.columns = self.columns + names + names1
+          del names,names1
           #self.columns = names + self.columns
           space1 = space_created_3.cpu().numpy()
+          del space_created_3
           space = pd.DataFrame(space1,columns = self.columns)
+          del space1
           space = space.dropna(axis=1, how='any')
           space = space.round(7)
           # Transpose the dataframe
           space = space.T.drop_duplicates().T
-          del values, names,
           self.columns = space.columns.tolist()
           self.df_feature_values = torch.tensor(space.values).to(self.device)
-          print('Third Feature Space building is completed',space.shape[1])
+          del space
+          print('Third Feature Space building is completed',self.df_feature_values.shape[1])
           print('Time taken to build the phi3 is',  round(time.time()-start,3) ,'seconds')
           if self.no_of_operators+1 == 5:
-            space.insert(0,'Target',self.Target_column)
-            space = space.dropna(axis=1, how='any')
-            #returniung the dataframe
-            return space
+            return self.df_feature_values,self.Target_column,self.columns  #space
           else:
             continue
         if i == 5:
           start = time.time()
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_4 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
-          del space_created_3
+          del values,values1
           self.columns = self.columns + names + names1
+          del names,names1
           space1 = space_created_4.cpu().numpy()
+          del space_created_4
           space = pd.DataFrame(space1,columns = self.columns)
+          del space1
           space = space.dropna(axis=1, how='any')
           space = space.round(7)
           # Transpose the dataframe
           space = space.T.drop_duplicates().T
-          del values, values1, names, names1
           self.df_feature_values = torch.tensor(space.values).to(self.device)
           self.columns = space.columns.tolist()
           self.df_feature_values = torch.tensor(space.values).to(self.device)
+          del space
           print('Third Feature Space building is completed',space.shape[1])
-          print('Time taken to build the phi3 is',  round(time.time()-start,3) ,'seconds')
+          print('Time taken to build the phi4 is',  round(time.time()-start,3) ,'seconds')
           if self.no_of_operators+1 == 6:
-            space.insert(0,'Target',self.Target_column)
-            space = space.dropna(axis=1, how='any')
-            #returniung the dataframe
-            return space
+            return self.df_feature_values,self.Target_column,self.columns
           else:
             continue
         if i == 6:
           start = time.time()
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_5 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
-          del space_created_4
+          del values,values1
           self.columns = self.columns + names + names1
-          del values, values1, names, names1
+          del names, names1
           space1 = space_created_5.cpu().numpy()
           space = pd.DataFrame(space1,columns = self.columns)
+          del space1
           space = space.dropna(axis=1, how='any')
           space = space.round(7)
           # Transpose the dataframe
           space = space.T.drop_duplicates().T
           self.df_feature_values = torch.tensor(space.values).to(self.device)
           self.columns = space.columns.tolist()
+          del space
           print('Third Feature Space building is completed',space.shape[1])
-          print('Time taken to build the phi3 is',  round(time.time()-start,3) ,'seconds')
+          print('Time taken to build the phi5 is',  round(time.time()-start,3) ,'seconds')
           if self.no_of_operators+1 == 7:
-            space.insert(0,'Target',self.Target_column)
-            space = space.dropna(axis=1, how='any')
-            #returniung the dataframe
-            return space
+            return self.df_feature_values,self.Target_column,self.columns
           else:
             continue
         if i == 7:
           start = time.time()
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_6 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
-          del space_created_5
+          del values,values1
           self.columns = self.columns + names + names1
-          del values, values1, names, names1
+          del names, names1
           space1 = space_created_6.cpu().numpy()
           space = pd.DataFrame(space1,columns = self.columns)
+          del space1
           space = space.dropna(axis=1, how='any')
           space = space.round(7)
           # Transpose the dataframe
           space = space.T.drop_duplicates().T
           self.df_feature_values = torch.tensor(space.values).to(self.device)
           self.columns = space.columns.tolist()
+          del space
           print('Third Feature Space building is completed',space.shape[1])
-          print('Time taken to build the phi3 is',  round(time.time()-start,3) ,'seconds')
+          print('Time taken to build the phi6 is',  round(time.time()-start,3) ,'seconds')
           
           if self.no_of_operators+1 == 8:
-            space.insert(0,'Target',self.Target_column)
-            space = space.dropna(axis=1, how='any')
-            #returniung the dataframe
-            return space
+            return self.df_feature_values,self.Target_column,self.columns
           else:
-            continue
+              print('Currently TorchSisso supports Feature Space Expansion till complexity of 7, provided input argument > 7. Further Feature Expansion cannot be performed, returning the last expanded feature space')
+              return self.df_feature_values,self.Target_column,self.columns
           
 
     else:
-      space.insert(0,'Target',self.Target_column)
-      space = space.dropna(axis=1, how='any')
-      #returniung the dataframe
-      return space
+      return self.df_feature_values, self.Target_column,self.columns
```

### Comparing `TorchSisso-1.0.8/TorchSisso/SISSO_REGRESSOR_TORCH.py` & `TorchSisso-1.0.9/TorchSisso/SISSO_REGRESSOR_TORCH.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,16 @@
         self.indices = torch.arange(1, (self.dimension*self.sis_features+1)).view(self.dimension*self.sis_features,1).to(self.device)
         self.residual = torch.empty(self.y_centered.shape).to(self.device)
         self.x_std_clone = torch.clone(self.x_standardized)
 
         
     
     def higher_dimension(self,iteration):
-        
-        min_error = torch.dot(self.y_centered,self.y_centered)
         #Indices values that needs to be assinged zero 
-        ind = self.indices[:,-1][~torch.isnan(self.indices[:,-1])]
+        ind = (self.indices[:,-1][~torch.isnan(self.indices[:,-1])]).to(self.device)
         self.x_standardized[:,ind.tolist()] = 0
         scores= torch.abs(torch.mm(self.residual,self.x_standardized))
         scores[torch.isnan(scores)] = 0
         self.x_standardized[:,ind.tolist()] = self.x_std_clone[:,ind.tolist()]
         sorted_scores, sorted_indices = torch.topk(scores, k= self.sis_features)
         sorted_indices = sorted_indices.T
         sorted_indices_earlier = self.indices[:((iteration-1)*self.sis_features),(iteration-1)].unsqueeze(1)
@@ -55,23 +53,25 @@
             remaining = (self.sis_features*self.dimension) - int(sorted_indices.shape[0])
             #zeros = torch.zeros(remaining,1)
             nan = torch.full((remaining,1),float('nan')).to(self.device)
             sorted_indices = torch.cat((sorted_indices,nan),dim=0)
             self.indices = torch.cat((self.indices,sorted_indices),dim=1)
         else:
             self.indices = torch.cat((self.indices,sorted_indices),dim=1)
-        
+
         comb1 = self.indices[:,-1][~torch.isnan(self.indices[:,-1])]
         combinations_generated = torch.combinations(comb1,(int(self.indices.shape[1])-1))
-        y_centered_clone = self.y_centered.unsqueeze(1).repeat(len(combinations_generated.tolist()),1,1)
+        y_centered_clone = self.y_centered.unsqueeze(1).repeat(len(combinations_generated.tolist()),1,1).to(self.device)
         comb_tensor = self.x_standardized.T[combinations_generated.tolist(),:]
         #Reshaping to match
         x_p = comb_tensor.permute(0,2,1)
+        
         start_c = time.time()
-        sol = x_p.pinverse().to(self.device) @ y_centered_clone
+        #sol = x_p.pinverse().to(self.device) @ y_centered_clone
+        sol, _, _, _ = torch.linalg.lstsq(x_p, y_centered_clone)
         predicted = torch.matmul(x_p,sol)
         residuals = y_centered_clone - predicted
         square = torch.square(residuals)
         mean = torch.mean(square,dim=1,keepdim=True)
         min_value, min_index = torch.min(mean, dim=0)
         print('Time taken to go through all combinations is:', time.time()-start_c)
         rmse = torch.sqrt(min_value)
@@ -97,40 +97,40 @@
         for i in range(1,self.dimension+1):
             
             if i ==1:
                 
                 start_1D = time.time()
                 #calculate the scores 
                 scores = torch.abs(torch.mm(self.y_centered.unsqueeze(1).T,self.x_standardized))
-                
                 #Set the NaN values claculation to zero, instead of removing 
                 scores[torch.isnan(scores)] = 0
                 
                 #Sort the top number of scores based on the sis_features 
                 sorted_scores, sorted_indices = torch.topk(scores,k=self.sis_features)
                 sorted_indices = sorted_indices.T
-                remaining = (self.sis_features*self.dimension) - int(sorted_indices.shape[0])
+                remaining = torch.tensor((self.sis_features*self.dimension) - int(sorted_indices.shape[0])).to(self.device)
                 #replace the remaining indices with nan
                 nan = torch.full((remaining,1),float('nan')).to(self.device)
                 #zeros = torch.zeros(remaining,1)
                 sorted_indices = torch.cat((sorted_indices,nan),dim=0)
                 #store the sorted indices as next column
                 self.indices = torch.cat((self.indices,sorted_indices),dim=1)
                 #selected_index = self.indices[0,0]
                 selected_index = self.indices[0,1]
                 x_in = self.x[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
-                x_with_bias = torch.cat((torch.ones_like(x_in), x_in), dim=1)
+                x_with_bias = torch.cat((torch.ones_like(x_in), x_in), dim=1).to(self.device)
                 #Calculate the intercept and coefficient, Non standardized
+                #coef1, _, _, _ = torch.linalg.lstsq(x_with_bias, self.y)
                 coef1 = torch.pinverse(x_with_bias).to(self.device) @ self.y
-                
                 #Calculate the residuals based on the standardized and centered values
                 x_in1 = self.x_standardized[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias1 = torch.cat((torch.ones_like(x_in1), x_in1), dim=1)
+                #coef, _, _, _ = torch.linalg.lstsq(x_with_bias1, self.y_centered)
                 coef = torch.pinverse(x_with_bias1).to(self.device) @ self.y_centered
                 self.residual = (self.y_centered - (coef[1]*self.x_standardized[:, int(selected_index)])).unsqueeze(1).T
                 rmse = float(torch.sqrt(torch.mean(self.residual**2)))
                 #self.residual = residual
                 coefficient = coef1[1]
                 intercept = coef1[0]
                 if intercept > 0:
```

### Comparing `TorchSisso-1.0.8/TorchSisso/testRegressor.py` & `TorchSisso-1.0.9/TorchSisso/testRegressor.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,20 +28,17 @@
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 operators = ['+','/']
 y = 10*((df.iloc[:,0])/(df.iloc[:,1]*(df.iloc[:,2]+df.iloc[:,3]))) + 3 + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y)
 start = time.time()
 fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cpu')
-df_created = fc.feature_space()
-print(time.time()-start)
-#Create Instace for class 
-x = torch.tensor(df_created.iloc[:,1:].values)
-y = torch.tensor(df_created.iloc[:,0])
-names = df_created.iloc[:,1:].columns
+x,y,names= fc.feature_space()
+print('Time taken to create feature space: ',time.time()-start,'seconds')
+
 sr = SISSO_REGRESSOR_TORCH.SISSORegressor(x, y, names,1,20,'L0','cpu')
 rmse,equation = sr.SISSO()
 print(rmse,equation)
 #sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cpu','L0')
 #rmse, equation = sr.SISSO()
 print('SISSO Completed',time.time()-start,'\n')
 print('\n')
@@ -63,20 +60,16 @@
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y1 = 3*np.sqrt(df.iloc[:,1]) + 2.10*np.sin(df.iloc[:,2]) + 2.10 + 0.010*np.random.normal(0,1,10)
 df.insert(0,'Target',y1)
 operators = ['sqrt','sin']
 start_c = time.time()
 FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
-df_created = FC.feature_space()
-print(time.time()-start_c)
-#Create Instace for class 
-x = torch.tensor(df_created.iloc[:,1:].values)
-y = torch.tensor(df_created.iloc[:,0])
-names = df_created.iloc[:,1:].columns
+x,y,names= FC.feature_space()
+print('Time taken to create feature space: ',time.time()-start_c,'seconds')
 start = time.time()
 sr = SISSO_REGRESSOR_TORCH.SISSORegressor(x,y,names,2,10,'L0','cpu')
 sr.SISSO()
 print(time.time()-start)
 print("SISSO Completed: ",time.time()-start_c,'\n')
 import os 
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/2/')
@@ -97,20 +90,16 @@
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y2 = 3*(np.exp(df.iloc[:,3])/(df.iloc[:,2]+np.exp(df.iloc[:,1]))) + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y2)
 operators = ['/','+','exp']
 start_c = time.time()
 FC = FeatureSpaceConstruction.feature_space_construction(operators, df,4,'cpu')
-df_created= FC.feature_space()
-print(time.time()-start_c)
-#Create Instace for class 
-x = torch.tensor(df_created.iloc[:,1:].values)
-y = torch.tensor(df_created.iloc[:,0])
-names = df_created.iloc[:,1:].columns
+x,y,names= FC.feature_space()
+print('Time taken to create feature space: ',time.time()-start_c,'seconds')
 start = time.time()
 sr = SISSO_REGRESSOR_TORCH.SISSORegressor(x,y,names,1,20,'cuda')
 rmse, equation = sr.SISSO()
 
 print("SISSO Completed: ",time.time()-start_c,'\n')
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/3/')
 df.to_csv('train.csv')
@@ -125,26 +114,23 @@
 
 ##############################################################################################################
 
 '''
 df = pd.read_csv('/home/muthyala.7/Downloads/NOMAD_TEST_FILE.csv')
 
 operators = ['+','-','*','/']
-start_time = time.time()
+start_c = time.time()
 FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
-df_created = FC.feature_space()
-print(time.time()-start_time)
-x = torch.tensor(df_created.iloc[:,1:].values)
-y = torch.tensor(df_created.iloc[:,0])
-names = df_created.iloc[:,1:].columns
+x,y,names= FC.feature_space()
+print('Time taken to create feature space: ',time.time()-start_c,'seconds')
 
 sr = SISSO_REGRESSOR_TORCH.SISSORegressor(x,y,names,3,20,'L0','cpu')
 sr.SISSO()
 
-print("SISSO Completed: ",time.time()-start_time,'\n')
+print("SISSO Completed: ",time.time()-start_c,'\n')
 
 '''
 ##########################################################################################################
 
 #CaseStudy-5
 
 #########################################################################################################
@@ -155,19 +141,16 @@
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y2 = 3*df.iloc[:,0]**3 + 2*df.iloc[:,1]**2 - 3.5*(df.iloc[:,2]) - 2 + 0.01*np.random.normal(0,1,size=20)
 df.insert(0,'Target',y2)
 operators = ['^3','^2']
 start_c = time.time()
 FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
-df_created= FC.feature_space()
-print(time.time()-start_c)
-x = torch.tensor(df_created.iloc[:,1:].values)
-y = torch.tensor(df_created.iloc[:,0])
-names = df_created.iloc[:,1:].columns
+x,y,names= FC.feature_space()
+print('Time taken to create feature space: ',time.time()-start_c,'seconds')
 sr = SISSO_REGRESSOR_TORCH.SISSORegressor(x,y,names,3,5,'L0','cpu')
 sr.SISSO()
 #sr = SISSORegressor.SISSO_Regressor(x,y,names,3,5,'cpu')
 #rmse, equation = sr.SISSO()
 print("SISSO Completed: ",time.time()-start_c,'\n')
 #os.mkdir('/home/muthyala.7/TorchSisso/Case_Studies/4')
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/4/')
```

### Comparing `TorchSisso-1.0.8/setup.py` & `TorchSisso-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.8",
+    version="1.0.9",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

