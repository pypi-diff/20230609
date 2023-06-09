# Comparing `tmp/torchbones-1.2.0.tar.gz` & `tmp/torchbones-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.2.0.tar", last modified: Tue Jun  6 08:49:04 2023, max compression
+gzip compressed data, was "torchbones-1.2.1.tar", last modified: Thu Jun  8 05:24:22 2023, max compression
```

## Comparing `torchbones-1.2.0.tar` & `torchbones-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-06 08:49:04.689027 torchbones-1.2.0/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-06 08:49:04.689027 torchbones-1.2.0/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-06 08:48:30.000000 torchbones-1.2.0/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.0/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16880 2023-06-06 08:48:20.000000 torchbones-1.2.0/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-08 05:24:22.443946 torchbones-1.2.1/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-08 05:24:22.443946 torchbones-1.2.1/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-08 05:24:22.443946 torchbones-1.2.1/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-08 05:24:10.000000 torchbones-1.2.1/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-08 05:24:22.433112 torchbones-1.2.1/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.1/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16963 2023-06-08 05:22:46.000000 torchbones-1.2.1/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-08 05:24:22.443946 torchbones-1.2.1/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-08 05:24:22.000000 torchbones-1.2.1/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-08 05:24:22.000000 torchbones-1.2.1/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-08 05:24:22.000000 torchbones-1.2.1/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-08 05:24:22.000000 torchbones-1.2.1/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-08 05:24:22.000000 torchbones-1.2.1/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.2.0/torchbones/main.py` & `torchbones-1.2.1/torchbones/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,34 +15,38 @@
 
 
 
 class Net(nn.Module):
     def __init__(self, *args):
         super(Net, self).__init__()
         sizes, self.convs, lins, csizes,  dropout, self.resnet, self.activation = args  
-        
         if self.resnet:
             pads = ((np.array(csizes)-1)/2).astype(int)
             lsize = self.convs[-1] * sizes[0]*sizes[1]
         elif self.convs:
             pads = np.zeros(len(csizes)).astype(int)
             lsize = self.convs[-1]
             for i in range(len(sizes)):
                 lsize *= (sizes[i] - sum(csizes) + len(csizes))
         else: 
             lsize = 1
             for i in range(len(sizes)):
                 lsize *= sizes[i]
-        
+
+        ##Define convolution size to use
+        if len(sizes) == 1: conv_layer = nn.Conv1d
+        elif len(sizes) == 2: conv_layer = nn.Conv2d
+        elif len(sizes) == 3: conv_layer = nn.Conv3d
+
         ## Create List of Convolution Layers
         if len(self.convs):
             self.convs = np.append([1,], self.convs)
             self.cfcs = nn.ModuleList()        
             for i in range(len(self.convs)-1):
-                self.cfcs.append(nn.Conv2d(self.convs[i], self.convs[i+1], csizes[i], padding = pads[i]).double())
+                self.cfcs.append(conv_layer(self.convs[i], self.convs[i+1], csizes[i], padding = pads[i]).double())
 
         ## Create List of Linear Layers
         self.lfcs = nn.ModuleList()
         if lins:
             lins = np.append([lsize,], lins)
             for i in range(len(lins)-1):
                 self.lfcs.append( nn.Linear(lins[i], lins[i+1], ))
@@ -70,15 +74,15 @@
                     new = self.cfcs[i](output)
                     output = new/torch.mean(new) + old
                     repnum = int((self.convs[(i+2)%len(self.convs)])/self.convs[i+1])
                 else:
                     output = self.cfcs[i](output)
                      
             #Create Embedding  
-            output = output.view(output.size()[0], -1)
+            output = output.flatten(start_dim = 1)
             output = torch.unsqueeze(output, 1)
                              
         #Run linear layers and activations
         for i in range(len(self.lfcs)):
             output = self.lfcs[i](output)
             if self.activation:
                 output = self.acts[i](output)
@@ -115,17 +119,14 @@
                 self.test_set = (self.test_set,)
         if not self.train_frac == 4/5 and self.test_set:
             warnings.warn('Specifying a training set supercedes specifying a training fraction')
         
         
         self.data = self.data_prep()
         self.datadims = len(self.indata.shape) - 1
-        if self.datadims != 2 and self.convs:
-            raise Exception('convolutions are only supported for 2d data')
-
                 
         self.dropout = kwargs.get('dropout', 0)
         self.net = Net(self.indata.shape[1:], self.convs, self.lins,  self.csizes, self.dropout, 
                              self.resnet, self.activation).double()
         
         self.init_lr = self.lr
         self.lr_decay = kwargs.get('lr_decay', 1)
@@ -342,16 +343,16 @@
             ax[2].plot(xs, self.testerr, label = 'Test loss')
             ax[2].set_xlabel('Epoch')
             ax[2].set_ylabel('Loss')
             ax[2].legend()
             ax[2].set_yscale('log')
         else: fig, ax = plt.subplots(1, 2, figsize = (15, 4))
             
-        x, y = self.data[4], np.squeeze(np.squeeze(self.testout.detach().numpy()))
-        yt, xt = self.net(self.data[0]).squeeze().squeeze().detach().numpy(), self.data[1]
+        x, y = self.data[4], self.testout.flatten(start_dim = 1).detach().numpy()
+        yt, xt = self.net(self.data[0]).flatten(start_dim = 1).detach().numpy(), self.data[1]
         
          
         ax[1].set_xlabel('test truth')
         ax[1].set_ylabel('test predication')
         ax[0].set_xlabel('train truth')
         ax[0].set_ylabel('train predication')
         
@@ -371,16 +372,16 @@
 
                 # Display values inside the plot
                 thresh = cm[i].max() / 2
                 for k in range(num_classes):
                     for j in range(num_classes):
                         ax[i].text(j, k, cm[i][k, j], ha='center', va='center', color='white' if cm[i][k, j] > thresh else 'black')
         else:
-            ax[0].hist2d(xt, yt, bins = 30)
-            ax[1].hist2d(x, y, bins = 30)
+            ax[0].hist2d(xt, np.squeeze(yt), bins = 30)
+            ax[1].hist2d(x, np.squeeze(y), bins = 30)
             
         fig.tight_layout()
         plt.show()
     
     def data_prep(self):
         data = torch.tensor(self.indata).double()
```

