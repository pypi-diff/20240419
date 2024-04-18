# Comparing `tmp/hygeoclas-0.4.tar.gz` & `tmp/hygeoclas-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hygeoclas-0.4.tar", last modified: Wed Mar 27 06:23:34 2024, max compression
+gzip compressed data, was "hygeoclas-0.5.1.tar", last modified: Thu Apr 18 22:55:14 2024, max compression
```

## Comparing `hygeoclas-0.4.tar` & `hygeoclas-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.719843 hygeoclas-0.4/
--rw-rw-rw-   0        0        0    11536 2024-03-09 00:13:05.000000 hygeoclas-0.4/LICENSE
--rw-rw-rw-   0        0        0      274 2024-03-27 06:23:34.713472 hygeoclas-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       74 2024-03-09 16:54:29.000000 hygeoclas-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.628997 hygeoclas-0.4/hygeoclas/
--rw-rw-rw-   0        0        0       50 2024-03-15 19:24:09.000000 hygeoclas-0.4/hygeoclas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.658852 hygeoclas-0.4/hygeoclas/fonts/
--rw-rw-rw-   0        0        0       21 2024-03-11 02:37:57.000000 hygeoclas-0.4/hygeoclas/fonts/__init__.py
--rw-rw-rw-   0        0        0      335 2024-03-11 02:38:29.000000 hygeoclas-0.4/hygeoclas/fonts/cambria.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.666572 hygeoclas-0.4/hygeoclas/models/
--rw-rw-rw-   0        0        0       55 2024-03-17 05:07:23.000000 hygeoclas-0.4/hygeoclas/models/__init__.py
--rw-rw-rw-   0        0        0    18256 2024-03-27 06:23:29.000000 hygeoclas-0.4/hygeoclas/models/annhcmod.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.679414 hygeoclas-0.4/hygeoclas/neuralnetworks/
--rw-rw-rw-   0        0        0      129 2024-03-11 02:23:18.000000 hygeoclas-0.4/hygeoclas/neuralnetworks/__init__.py
--rw-rw-rw-   0        0        0     4593 2024-03-26 07:36:24.000000 hygeoclas-0.4/hygeoclas/neuralnetworks/dinet.py
--rw-rw-rw-   0        0        0     8121 2024-03-23 21:14:48.000000 hygeoclas-0.4/hygeoclas/neuralnetworks/resnet1d.py
--rw-rw-rw-   0        0        0     5013 2024-03-27 06:20:37.000000 hygeoclas-0.4/hygeoclas/neuralnetworks/squeezenet1d.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.708708 hygeoclas-0.4/hygeoclas/utils/
--rw-rw-rw-   0        0        0      395 2024-03-24 17:37:40.000000 hygeoclas-0.4/hygeoclas/utils/__init__.py
--rw-rw-rw-   0        0        0      379 2024-03-16 03:58:47.000000 hygeoclas-0.4/hygeoclas/utils/changeover.py
--rw-rw-rw-   0        0        0     2406 2024-03-17 07:38:01.000000 hygeoclas-0.4/hygeoclas/utils/crawl.py
--rw-rw-rw-   0        0        0      855 2024-03-11 02:23:18.000000 hygeoclas-0.4/hygeoclas/utils/dynamic.py
--rw-rw-rw-   0        0        0    15042 2024-03-27 04:39:24.000000 hygeoclas-0.4/hygeoclas/utils/graphic.py
--rw-rw-rw-   0        0        0     2695 2024-03-24 04:31:36.000000 hygeoclas-0.4/hygeoclas/utils/methods.py
--rw-rw-rw-   0        0        0     2170 2024-03-24 17:37:22.000000 hygeoclas-0.4/hygeoclas/utils/numeric.py
--rw-rw-rw-   0        0        0     3905 2024-03-24 17:44:10.000000 hygeoclas-0.4/hygeoclas/utils/support.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:23:34.711439 hygeoclas-0.4/hygeoclas.egg-info/
--rw-rw-rw-   0        0        0      274 2024-03-27 06:23:34.000000 hygeoclas-0.4/hygeoclas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-03-27 06:23:34.000000 hygeoclas-0.4/hygeoclas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:23:34.000000 hygeoclas-0.4/hygeoclas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-03-27 06:23:34.000000 hygeoclas-0.4/hygeoclas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 06:23:34.000000 hygeoclas-0.4/hygeoclas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 06:23:34.720839 hygeoclas-0.4/setup.cfg
--rw-rw-rw-   0        0        0      354 2024-03-18 21:41:32.000000 hygeoclas-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:14.039454 hygeoclas-0.5.1/
+-rw-rw-rw-   0        0        0    11536 2024-03-09 00:13:05.000000 hygeoclas-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      276 2024-04-18 22:55:14.027452 hygeoclas-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2024-03-09 16:54:29.000000 hygeoclas-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:13.926449 hygeoclas-0.5.1/hygeoclas/
+-rw-rw-rw-   0        0        0       50 2024-03-15 19:24:09.000000 hygeoclas-0.5.1/hygeoclas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:13.960448 hygeoclas-0.5.1/hygeoclas/fonts/
+-rw-rw-rw-   0        0        0       21 2024-03-11 02:37:57.000000 hygeoclas-0.5.1/hygeoclas/fonts/__init__.py
+-rw-rw-rw-   0        0        0      335 2024-03-11 02:38:29.000000 hygeoclas-0.5.1/hygeoclas/fonts/cambria.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:13.975464 hygeoclas-0.5.1/hygeoclas/models/
+-rw-rw-rw-   0        0        0       55 2024-03-17 05:07:23.000000 hygeoclas-0.5.1/hygeoclas/models/__init__.py
+-rw-rw-rw-   0        0        0    18552 2024-04-08 23:20:38.000000 hygeoclas-0.5.1/hygeoclas/models/annhcmod.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:13.988444 hygeoclas-0.5.1/hygeoclas/neuralnetworks/
+-rw-rw-rw-   0        0        0      129 2024-03-11 02:23:18.000000 hygeoclas-0.5.1/hygeoclas/neuralnetworks/__init__.py
+-rw-rw-rw-   0        0        0     4343 2024-04-17 19:48:42.000000 hygeoclas-0.5.1/hygeoclas/neuralnetworks/dinet.py
+-rw-rw-rw-   0        0        0     8698 2024-04-18 22:12:33.000000 hygeoclas-0.5.1/hygeoclas/neuralnetworks/resnet1d.py
+-rw-rw-rw-   0        0        0     5045 2024-04-17 01:47:35.000000 hygeoclas-0.5.1/hygeoclas/neuralnetworks/squeezenet1d.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:14.020453 hygeoclas-0.5.1/hygeoclas/utils/
+-rw-rw-rw-   0        0        0      395 2024-03-24 17:37:40.000000 hygeoclas-0.5.1/hygeoclas/utils/__init__.py
+-rw-rw-rw-   0        0        0      379 2024-03-16 03:58:47.000000 hygeoclas-0.5.1/hygeoclas/utils/changeover.py
+-rw-rw-rw-   0        0        0     2406 2024-03-17 07:38:01.000000 hygeoclas-0.5.1/hygeoclas/utils/crawl.py
+-rw-rw-rw-   0        0        0      855 2024-03-11 02:23:18.000000 hygeoclas-0.5.1/hygeoclas/utils/dynamic.py
+-rw-rw-rw-   0        0        0    15851 2024-04-16 12:27:21.000000 hygeoclas-0.5.1/hygeoclas/utils/graphic.py
+-rw-rw-rw-   0        0        0     2695 2024-03-24 04:31:36.000000 hygeoclas-0.5.1/hygeoclas/utils/methods.py
+-rw-rw-rw-   0        0        0     2170 2024-03-24 17:37:22.000000 hygeoclas-0.5.1/hygeoclas/utils/numeric.py
+-rw-rw-rw-   0        0        0     3905 2024-03-24 17:44:10.000000 hygeoclas-0.5.1/hygeoclas/utils/support.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:55:14.025443 hygeoclas-0.5.1/hygeoclas.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-04-18 22:55:13.000000 hygeoclas-0.5.1/hygeoclas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-04-18 22:55:13.000000 hygeoclas-0.5.1/hygeoclas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 22:55:13.000000 hygeoclas-0.5.1/hygeoclas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-18 22:55:13.000000 hygeoclas-0.5.1/hygeoclas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 22:55:13.000000 hygeoclas-0.5.1/hygeoclas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 22:55:14.040457 hygeoclas-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      356 2024-04-18 22:54:03.000000 hygeoclas-0.5.1/setup.py
```

### Comparing `hygeoclas-0.4/LICENSE` & `hygeoclas-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas/models/annhcmod.py` & `hygeoclas-0.5.1/hygeoclas/models/annhcmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import numpy as np
 import pandas as pd
 import torch
 
 from datetime import datetime
 from scipy.stats import shapiro
-from sklearn.metrics import f1_score, confusion_matrix, recall_score
+from sklearn.metrics import confusion_matrix, f1_score, precision_score, recall_score
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 from tqdm import tqdm
 
 from hygeoclas.utils.crawl import get_udf_record
 from hygeoclas.utils.methods import DataCompressor
 
@@ -289,41 +289,44 @@
             trainLoader, validationLoader, testLoader = create_data_loaders(XTrain, XValidation, XTest, yTrain, yValidation, yTest, self.batchSize)
 
             self.net.reset_weights()
             self.net.fit(trainLoader, validationLoader, epochs=self.epochs)
             self.net.evaluate(testLoader)
 
             yPredicted = self.net.predictions
-            f1Score = f1_score(self.yTest, yPredicted, average="binary")
+            precisionScore = precision_score(self.yTest, yPredicted, average="binary", zero_division=0)
             recallScore = recall_score(self.yTest, yPredicted, average="binary")
+            f1Score = f1_score(self.yTest, yPredicted, average="binary")
             confusionMatrix = confusion_matrix(self.yTest, yPredicted)
 
-            self.metrics.append((self.net.error, self.net.accuracy, f1Score, recallScore, confusionMatrix, self.net.trainLosses, self.net.validationLosses, self.net.state_dict()))
+            self.metrics.append((self.net.error, self.net.accuracy, precisionScore, recallScore, f1Score, confusionMatrix, self.net.trainLosses, self.net.validationLosses, self.net.state_dict()))
             
         self.averageError = sum(metric[0] for metric in self.metrics)/self.cycles
         self.averageAccuracy = sum(metric[1] for metric in self.metrics)/self.cycles
-        self.averageF1Score = sum(metric[2] for metric in self.metrics)/self.cycles
+        self.averagePrecision = sum(metric[2] for metric in self.metrics)/self.cycles
         self.averageRecallScore = sum(metric[3] for metric in self.metrics)/self.cycles
+        self.averageF1Score = sum(metric[4] for metric in self.metrics)/self.cycles
 
         self.scores = []
         for metric in self.metrics:
-            average = ((1/metric[0]) + metric[1] + metric[2] + metric[3])/3
-            variance = np.var([(1/metric[0]), metric[1], metric[2], metric[3]])
+            average = ((1/metric[0]) + metric[1] + metric[2] + metric[3]+ metric[4])/3
+            variance = np.var([(1/metric[0]), metric[1], metric[2], metric[3], metric[4]])
             score = average - variance
             self.scores.append(abs(score))
         index = self.scores.index(max(self.scores))
 
-        self.bestMetrics = self.metrics[index][:5]
+        self.bestMetrics = self.metrics[index][:6]
         
         self.net.reset_parameters()
+        self.net.error = self.metrics[index][0]
         self.net.accuracy = self.metrics[index][1]
-        self.net.trainLosses = self.metrics[index][5]
-        self.net.validationLosses = self.metrics[index][6]
+        self.net.trainLosses = self.metrics[index][6]
+        self.net.validationLosses = self.metrics[index][7]
 
-        self.bestWeights = self.metrics[index][7]
+        self.bestWeights = self.metrics[index][8]
         self.net.load_state_dict(self.bestWeights)
 
     def execute(self, **kwargs) -> None:
         self.filePathOfNWPresence = kwargs.get("filePathOfNWPresence", self.filePathOfNWPresence)
         self.filePathOfWPresence = kwargs.get("filePathOfWPresence", self.filePathOfWPresence)
         self.compressedDatabase = kwargs.get("compressedDatabase", self.compressedDatabase)
         self.saveDatabase = kwargs.get("saveDatabase", self.saveDatabase)
```

### Comparing `hygeoclas-0.4/hygeoclas/neuralnetworks/dinet.py` & `hygeoclas-0.5.1/hygeoclas/neuralnetworks/dinet.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,21 +39,21 @@
     def reset_weights(self):
         self.apply(reset_weights)   
 
     def reset_parameters(self):
         self.trainLosses = []
         self.validationLosses = []
         self.predictions = []
-        self.accuracy = 0
+        self.error = None
+        self.accuracy = None
 
     def fit(self, trainLoader, validationLoader, epochs):
         self.trainLosses = []
         self.validationLosses = []
         earlyStopper = EarlyStopper(patience=1, minDelta=0)
-        bestValidationLoss = float("inf")
 
         for epoch in range(epochs):
             trainLossSummation = 0
             self.train()
             for data, target in trainLoader:
                 data = data.to(self.device)
                 target = target.to(self.device)
@@ -82,20 +82,14 @@
                     validationLossSummation += loss.item()
             validationLoss = validationLossSummation/len(validationLoader)
             self.validationLosses.append(validationLoss)
 
             for param_group in self.optimizer.param_groups:
                 param_group["lr"] *= 0.9
 
-            if validationLoss < bestValidationLoss:
-                bestValidationLoss = validationLoss
-            else:
-                for param_group in self.optimizer.param_groups:
-                    param_group["lr"] /= 10
-
             if earlyStopper.early_stop(self, validationLossSummation):
                 print(f"Stopping training early at epoch {epoch}")
                 self.trainLosses = self.trainLosses[:-1]
                 self.validationLosses = self.validationLosses [:-1]
                 break
         self.error = self.trainLosses[-1]
```

### Comparing `hygeoclas-0.4/hygeoclas/neuralnetworks/resnet1d.py` & `hygeoclas-0.5.1/hygeoclas/neuralnetworks/resnet1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
 
 from hygeoclas.utils.support import EarlyStopper
-from hygeoclas.utils.support import reset_weights
+
+def kaiming_init(module):
+    nn.init.kaiming_normal_(module.weight, mode="fan_out", nonlinearity="relu")
+    if module.bias is not None:
+        nn.init.constant_(module.bias, 0)
+
+def reset_weights(self):
+    for module in self.modules():
+        if isinstance(module, nn.Conv1d) or isinstance(module, nn.Linear):
+            kaiming_init(module)
+        elif isinstance(module, nn.BatchNorm1d):
+            nn.init.constant_(module.weight, 1)
+            nn.init.constant_(module.bias, 0)
 
 class BasicBlock1D(nn.Module):
     def __init__(self, inputChannels, outputChannels, inputStride):
         super(BasicBlock1D, self).__init__()
         self.conv1 = nn.Conv1d(inputChannels, outputChannels, kernel_size=3, stride=inputStride, padding=1, dilation=1)
         self.conv2 = nn.Conv1d(outputChannels, outputChannels, kernel_size=3, stride=1, padding=1, dilation=1)
         self.bn = nn.BatchNorm1d(outputChannels)
@@ -66,33 +78,35 @@
         hx = fx + self.shortcut(x)
         hx = self.relu(hx)
         return hx
 
 class ResNet1D(nn.Module):
     def __init__(self, block=BasicBlock1D, nBlocks=[2,2,2,2], nClasses=2):
         super(ResNet1D, self).__init__()
+        self.block = block
         self.nClasses = nClasses
         self.M = 224
 
         self.conv1 = nn.Conv1d(1, 64, kernel_size=7, stride=2, padding=3, dilation=1)
         self.bn1 = nn.BatchNorm1d(64)
         self.relu = nn.ReLU()
         self.mp = nn.MaxPool1d(kernel_size=3, stride=2, padding=1, dilation=1)
-        try:
+        if block == BasicBlock1D:
             self.rl1 = self._make_layer(block, 64, 64, nBlocks[0], 1)
             self.rl2 = self._make_layer(block, 64, 128, nBlocks[1], 2)
             self.rl3 = self._make_layer(block, 128, 256, nBlocks[2], 2)
             self.rl4 = self._make_layer(block, 256, 512, nBlocks[3], 2)
-        except:
+        else:
             self.rl1 = self._make_layer(block, 64, 256, nBlocks[0], 1)
             self.rl2 = self._make_layer(block, 256, 512, nBlocks[1], 2)
             self.rl3 = self._make_layer(block, 512, 1024, nBlocks[2], 2)
             self.rl4 = self._make_layer(block, 1024, 2048, nBlocks[3], 2)
         self.ap = nn.AdaptiveAvgPool1d(1)
-        self.fc = None
+        self.fc512 = nn.Linear(512, self.nClasses)
+        self.fc2048 = nn.Linear(2048, self.nClasses)
 
         self.optimizer = optim.SGD(self.parameters(), lr=0.1, momentum=0.9, weight_decay=0.0001) 
         self.lossFunction = nn.CrossEntropyLoss()
         self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.to(self.device)
 
     def _make_layer(self, block, inputChannels, outputChannels, nBlocks, inputStride):
@@ -106,30 +120,31 @@
     def reset_weights(self):
         self.apply(reset_weights) 
 
     def reset_parameters(self):
         self.trainLosses = []
         self.validationLosses = []
         self.predictions = []
-        self.accuracy = 0
+        self.error = None
+        self.accuracy = None
 
     def forward(self, x):
         x = self.conv1(x)
         x = self.bn1(x)
-        x = self.relu(x)
         x = self.mp(x)
         x = self.rl1(x)
         x = self.rl2(x)
         x = self.rl3(x)
         x = self.rl4(x)
         x = self.ap(x)
         x = torch.flatten(x, 1)
-        if self.fc is None:
-            self.fc = nn.Linear(x.size(1), self.nClasses).to(self.device)
-        x = self.fc(x)
+        if self.block == BasicBlock1D:
+            x = self.fc512(x)
+        else:
+            x = self.fc2048(x)
         return x
 
     def fit(self, trainLoader, validationLoader, epochs):
         self.trainLosses = []
         self.validationLosses = []
         bestValidationLoss = float("inf")
         earlyStopper = EarlyStopper(patience=1, minDelta=0)
```

### Comparing `hygeoclas-0.4/hygeoclas/neuralnetworks/squeezenet1d.py` & `hygeoclas-0.5.1/hygeoclas/neuralnetworks/squeezenet1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,26 @@
     def reset_weights(self):
         self.apply(reset_weights)   
 
     def reset_parameters(self):
         self.trainLosses = []
         self.validationLosses = []
         self.predictions = []
-        self.accuracy = 0
+        self.error = None
+        self.accuracy = None
 
     def forward(self, x):
         x = self.features(x)
         return x
     
     def fit(self, trainLoader, validationLoader, epochs):
         self.trainLosses = []
         self.validationLosses = []
         earlyStopper = EarlyStopper(patience=1, minDelta=0)
-        scheduler = torch.optim.lr_scheduler.LambdaLR(self.optimizer, lr_lambda=lambda epoch: (1-epoch/epochs)**1.0)
+        scheduler = torch.optim.lr_scheduler.LambdaLR(self.optimizer, lr_lambda=lambda epoch: (1-(epoch/epochs))**1.0)
         
         for epoch in range(epochs):  
             trainLossSummation = 0
             self.train()
             for data, target in trainLoader:
                 data = data.to(self.device)
                 target = target.to(self.device)
```

### Comparing `hygeoclas-0.4/hygeoclas/utils/crawl.py` & `hygeoclas-0.5.1/hygeoclas/utils/crawl.py`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas/utils/dynamic.py` & `hygeoclas-0.5.1/hygeoclas/utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas/utils/graphic.py` & `hygeoclas-0.5.1/hygeoclas/utils/graphic.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,41 +37,45 @@
 
     Args:
         trainLosses (np.ndarray): The training losses.
         validationLosses (np.ndarray): The validation losses.
 
     Kwargs:
         fontFamily (str): The font family to use in the plot. Default is "Cambria".
+        axisLabelNames (list): A list of two names for the axis labels. Default is ["Epoch", "Error"].
+        legendLabelNames (list): A list of two names for the legend labels. Default is ["Training", "Validation"].
         fontSize (int): The font size to use in the plot. Default is 11.
         dotSize (int): The size of the dots. Default is 15.
         labelFontSize (int): The font size to use for the labels. Default is 12.
         numberFontSize (int): The font size to use for the numbers. Default is 10.
         legendFontSize (int): The font size to use for the legend. Default is 10.
         save (bool): If True, saves the figure to a file. Default is False.
         savePath (str): The path where the figure will be saved. Default is "./fig.png".
     """
     plt.rcParams["font.family"] = kwargs.get("fontFamily", "Cambria")
     plt.rcParams["font.size"] = kwargs.get("fontSize", 11)
     
+    legendLabelNames =kwargs.get("legendLabelNames", ["Training", "Validation"])
+    axisLabelNames = kwargs.get("axisLabelNames", ["Epoch", "Error"])
     dotSize = kwargs.get("dotSize", 15)
     labelFontSize = kwargs.get("labelFontSize", 12)
 
     red = rgb_to_matplotlib((136, 0, 21))
     blue = rgb_to_matplotlib((0, 2, 61))
 
     if len(trainLosses) == 1:
         print("Only one value was found in the losses, impossible to generate a training-validation curve.")
     else:
         fig, ax = plt.subplots()
 
-        plot_curve(ax, np.linspace(1, len(trainLosses), len(trainLosses)), trainLosses, red, "Entrenamiento", dotSize)
-        plot_curve(ax, np.linspace(1, len(validationLosses), len(validationLosses)), validationLosses, blue, "Validación", dotSize)
+        plot_curve(ax, np.linspace(1, len(trainLosses), len(trainLosses)), trainLosses, red, legendLabelNames[0], dotSize)
+        plot_curve(ax, np.linspace(1, len(validationLosses), len(validationLosses)), validationLosses, blue, legendLabelNames[1], dotSize)
 
-        ax.set_xlabel("Epoca", fontsize=labelFontSize)
-        ax.set_ylabel("Error", fontsize=labelFontSize)
+        ax.set_xlabel(axisLabelNames[0], fontsize=labelFontSize)
+        ax.set_ylabel(axisLabelNames[1], fontsize=labelFontSize)
         ax.tick_params(axis="both", which="major", labelsize=kwargs.get("numberFontSize", 10))
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
         
         sns.despine()
         for axis in ["bottom","left"]:
             ax.spines[axis].set_linewidth(1.2) 
         
@@ -89,67 +93,67 @@
     This function generates plots from the data contained in a pandas DataFrame. 
     The plots represent the presence and absence of water in a compressed database.
 
     Parameters:
     compressedDatabase (pd.DataFrame): A pandas DataFrame containing the data to be plotted.
     **kwargs: Additional arguments for customizing the plots. Possible arguments are:
         - colors (list): A list of two colors for the plots. Default is ["gray", "blue"].
+        - axisLabelNames (list): A list of two names for the axis labels. Default is ["Coefficient", "Amplitude"].
         - numberSize (int): The size of the numbers on the plots. Default is 10.
         - legendFontSize (int): The font size of the legend. Default is 9.
-        - legendLabelNames (list): A list of two names for the legend labels. Default is ["NWP", "WP"].
+        - legendLabelNames (list): A list of two names for the legend labels. Default is ["NPoW", "PoW"].
         - fontFamily (str): The font family for the plots. Default is "Cambria".
         - fontSize (int): The font size for the plots. Default is 11.
         - formatterAx1 (str): The format of the y-axis for the first plot. Default is "normal".
         - formatterAx3 (str): The format of the y-axis for the third plot. Default is "normal".
         - saveFigures (bool): If True, saves the plots as .png files. Default is False.
         - savePaths (list): A list of three file paths to save the plots. Default is ["fig1.png", "fig2.png", "fig3.png"].
 
     Returns:
     None. Displays the plots and, if saveFigures is True, saves the plots at the specified paths.
     """
-    
     data = {
         "NPoW": compressedDatabase[compressedDatabase["Label"] == 0],
         "PoW": compressedDatabase[compressedDatabase["Label"] == 1]
     }
 
-    coefficients = np.arange(1, len(data["WP"].mean()[1:])+1)
+    coefficients = np.arange(1, len(data["PoW"].mean()[1:])+1)
     formatters = {
         "normal": FuncFormatter(lambda y, _: "{:.16g}".format(y*1e-0)),
         "kilo": FuncFormatter(lambda y, _: "{:.16g}K".format(y*1e-3)),
         "mega": FuncFormatter(lambda y, _: "{:.16g}M".format(y*1e-6))
     }
 
     colors = kwargs.get("colors", ["gray", "blue"])
-    #
-    labelSize = kwargs.get("numberSize", 10)
+    axisLabelNames = kwargs.get("axisLabelNames", ["Coefficient", "Amplitude"])
+    numberSize = kwargs.get("numberSize", 10)
     legendFontSize = kwargs.get("legendFontSize", 9)
     legendLabelNames = kwargs.get("legendLabelNames", ["NPoW", "PoW"])
 
     plt.rcParams["font.family"] = kwargs.get("fontFamily", "Cambria")
     plt.rcParams["font.size"] = kwargs.get("fontSize", 11)
     
     figs = []
     for i, (set, color) in enumerate(zip(["NPoW", "PoW"], colors)):
         fig, ax = plt.subplots()
         ax.fill_between(coefficients, data[set].min()[1:], data[set].max()[1:], color=color, alpha=0.3)
         ax.plot(coefficients, data[set].mean()[1:], color=color)
-        ax.set_xlabel("Coeficiente")
-        ax.set_ylabel("Amplitud")
-        ax.tick_params(axis="both", which="major", labelsize=labelSize)
+        ax.set_xlabel(axisLabelNames[0])
+        ax.set_ylabel(axisLabelNames[1])
+        ax.tick_params(axis="both", which="major", labelsize=numberSize)
         ax.yaxis.set_major_formatter(formatters[kwargs.get(f"formatterAx{i+1}", "normal")])
         sns.despine()
         figs.append(fig)
 
     fig3, ax = plt.subplots()
-    for set, label, color in zip(["NWP", "WP"], legendLabelNames, colors):
+    for set, label, color in zip(["NPoW", "PoW"], legendLabelNames, colors):
         ax.fill_between(coefficients, data[set].min()[1:], data[set].max()[1:], color=color, alpha=0.3, label=label)
-    ax.set_xlabel("Coeficiente")
-    ax.set_ylabel("Amplitud")
-    ax.tick_params(axis="both", which="major", labelsize=labelSize)
+    ax.set_xlabel(axisLabelNames[0])
+    ax.set_ylabel(axisLabelNames[1])
+    ax.tick_params(axis="both", which="major", labelsize=numberSize)
     ax.yaxis.set_major_formatter(formatters[kwargs.get("formatterAx3", "normal")])
     legend = ax.legend(frameon=False, fontsize=kwargs.get("legendFontSize", 10), bbox_to_anchor=(1, 1.05))
     for handle in legend.legend_handles:
         handle.set_width(legendFontSize*2.25)
         handle.set_height(legendFontSize/2.75)
     sns.despine()
     figs.append(fig3)
@@ -280,35 +284,37 @@
 
     Args:
         scores (list): The performance scores to plot.
 
     Kwargs:
         fontFamily (str): The font family to use in the plot. Default is "Cambria".
         fontSize (int): The font size to use in the plot. Default is 11.
+        axisLabelNames (list): A list of two names for the axis labels. Default is ["Cycle", "Score"]
         labelFontSize (int): The font size to use for the labels. Default is 12.
         numberFontSize (int): The font size to use for the numbers. Default is 10.
         dotSize (int): The size of the dots. Default is 15.
         save (bool): If True, saves the figure to a file. Default is False.
         savePath (str): The path where the figure will be saved. Default is "./fig.png".
 
     Note:
         This function uses seaborn's despine to remove the top and right spines from the plot.
     """
     plt.rcParams["font.family"] = kwargs.get("fontFamily", "Cambria")
     plt.rcParams["font.size"] = kwargs.get("fontSize", 11)
 
+    axisLabelNames = kwargs.get("axisLabelNames", ["Cycle", "Score"])
     labelFontSize = kwargs.get("labelFontSize", 12)
 
     orange = rgb_to_matplotlib((240, 134, 80))
 
     fig, ax = plt.subplots()
     plot_curve(ax, np.linspace(1, len(scores), len(scores)), scores, orange, "", kwargs.get("dotSize", 15))
 
-    ax.set_xlabel("Ciclo", fontsize=labelFontSize)
-    ax.set_ylabel("Puntaje", fontsize=labelFontSize)
+    ax.set_xlabel(axisLabelNames[0], fontsize=labelFontSize)
+    ax.set_ylabel(axisLabelNames[1], fontsize=labelFontSize)
     ax.tick_params(axis="both", which="major", labelsize=kwargs.get("numberFontSize", 10))
     ax.xaxis.set_major_locator(MaxNLocator(integer=True))
 
     sns.despine()
     for axis in ["bottom","left"]:
         ax.spines[axis].set_linewidth(1.2)
```

### Comparing `hygeoclas-0.4/hygeoclas/utils/methods.py` & `hygeoclas-0.5.1/hygeoclas/utils/methods.py`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas/utils/numeric.py` & `hygeoclas-0.5.1/hygeoclas/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas/utils/support.py` & `hygeoclas-0.5.1/hygeoclas/utils/support.py`

 * *Files identical despite different names*

### Comparing `hygeoclas-0.4/hygeoclas.egg-info/SOURCES.txt` & `hygeoclas-0.5.1/hygeoclas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

