# Comparing `tmp/TorchEase-0.0.2.tar.gz` & `tmp/TorchEase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchEase-0.0.2.tar", last modified: Fri May  5 15:37:58 2023, max compression
+gzip compressed data, was "TorchEase-0.0.5.tar", last modified: Sat May  6 10:16:26 2023, max compression
```

## Comparing `TorchEase-0.0.2.tar` & `TorchEase-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.626500 TorchEase-0.0.2/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:37:58.626500 TorchEase-0.0.2/PKG-INFO
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.622499 TorchEase-0.0.2/TorchEase/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)      213 2023-05-05 15:15:14.000000 TorchEase-0.0.2/TorchEase/__init__.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     6900 2023-05-05 11:31:46.000000 TorchEase-0.0.2/TorchEase/fuser.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     3185 2023-05-05 11:37:01.000000 TorchEase-0.0.2/TorchEase/modelbase.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     8253 2023-05-05 15:30:58.000000 TorchEase-0.0.2/TorchEase/trainer.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     2107 2023-05-05 12:09:09.000000 TorchEase-0.0.2/TorchEase/user.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1733 2023-05-05 12:06:08.000000 TorchEase-0.0.2/TorchEase/utilities.py
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.626500 TorchEase-0.0.2/TorchEase.egg-info/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/PKG-INFO
--rw-rw-r--   0 broxy     (1000) broxy     (1000)      298 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/SOURCES.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)        1 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/dependency_links.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)       37 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/requires.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)       10 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/top_level.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)       38 2023-05-05 15:37:58.626500 TorchEase-0.0.2/setup.cfg
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1366 2023-05-05 15:36:53.000000 TorchEase-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:16:26.312593 TorchEase-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:16:26.312593 TorchEase-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:16:26.312593 TorchEase-0.0.5/TorchEase/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-06 10:16:06.000000 TorchEase-0.0.5/TorchEase/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:16:26.312593 TorchEase-0.0.5/TorchEase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:16:26.000000 TorchEase-0.0.5/TorchEase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 10:16:26.000000 TorchEase-0.0.5/TorchEase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:16:26.000000 TorchEase-0.0.5/TorchEase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 10:16:26.000000 TorchEase-0.0.5/TorchEase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 10:16:26.000000 TorchEase-0.0.5/TorchEase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:16:26.312593 TorchEase-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-06 10:16:06.000000 TorchEase-0.0.5/setup.py
```

### Comparing `TorchEase-0.0.2/PKG-INFO` & `TorchEase-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.2
+Version: 0.0.5
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.2/TorchEase/fuser.py` & `TorchEase-0.0.5/TorchEase/fuser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import torch
 from .modelbase import ModelBase
 from torch.utils.data import DataLoader
+
+
 class ModelFuser(ModelBase):
     """
     Class for fusing the predictions of multiple models.
 
     Parameters
     ----------
     *models : ModelBase objects
@@ -69,21 +71,21 @@
 
         self.models = models
         self.n_models = len(models)
         self.test_loader = test_loader
         self.n_classes = 9
         self.device = device
         assert isinstance(test_loader, torch.utils.data.DataLoader), "Loader is not of type DataLoader"
+
     def fuse(self):
         """
         Fuses the predictions of all models.
         """
         import torch
         import numpy as np
-        import pandas as pd
         assert self.test_loader, "Kein Testdatensatz!"
 
         predictions = []
         targets = []
         for model in self.models:
             prediction = []
             model.to(self.device)
@@ -104,28 +106,21 @@
         combined_probability = np.apply_along_axis(lambda row: self.combine_probabilities(row), axis=1, arr=probabilities.reshape([-1, self.n_models * self.n_classes]))
         all_pred = predictions.detach().cpu().numpy().argmax(3).reshape((self.n_models, -1))
         all_target = target[0].detach().cpu().numpy().reshape(-1)
         data = np.vstack([all_target, all_pred]).T
         probabilities = probabilities.reshape((self.n_models, -1, self.n_classes))
         for i in probabilities:
             data = np.hstack([data, i])
-        # get_class(all_pred)
         fused_prediction = np.apply_along_axis(lambda row: self.apply_voting(row), axis=1, arr=data)
         result = np.vstack([all_target, fused_prediction])
         self.target = all_target.reshape(-1)
         self.fused_prediction = fused_prediction.reshape(-1)
         self.evaluation_target = self.target
         self.evaluation_prediction = self.fused_prediction
         self.probability = combined_probability
-        # df = pd.DataFrame(data=data, columns=["Model1", "Model2", "Model3", "Target"])
-        # df["Probabilites"] = probabilities[0]
-        # print("HERE")
-        from sklearn.metrics import confusion_matrix
-        # confusion_matrix(predictions.detach().cpu().numpy(), self.y_pred.argmax(1).detach().cpu().numpy())
-        # return result
 
     def combine_probabilities(self, row):
         """
         Computes the combined probability of all models for each class.
 
         Parameters
         ----------
@@ -134,17 +129,15 @@
 
         Returns
         -------
         numpy.ndarray
             Combined probability for each class.
         """
         import numpy as np
-        from scipy.special import softmax
         probabilities = row.reshape([self.n_models, self.n_classes])
-        #probabilities = softmax(probabilities, axis=1)
         combined_probability = np.mean(probabilities, axis=0)
         return combined_probability
 
     def apply_voting(self, row):
         """
         Applies voting mechanism to select final prediction.
 
@@ -164,15 +157,14 @@
         vote_array = row[1:self.n_models+1].astype(int)
         total_votes = self.n_models
         votes_for_results = math.ceil(total_votes/2)
         max_val = np.argmax(np.bincount(vote_array))
         unique_vals, counts = np.unique(vote_array, return_counts=True)
 
         if counts.shape[0] <= votes_for_results:
-            # print("Voting Successful")
             voted_value = max_val
             return voted_value
         else:
             range_probabilities = self.n_classes * self.n_models
             probabilities = row[-range_probabilities:].reshape([self.n_models, self.n_classes])
             probabilities = softmax(probabilities, axis=1)
             combined_probability = np.mean(probabilities, axis=0)
```

### Comparing `TorchEase-0.0.2/TorchEase/modelbase.py` & `TorchEase-0.0.5/TorchEase/modelbase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 
 class ModelBase:
     """
     A base class for machine learning models.
-
-    Attributes:
-        cm (numpy.ndarray): Confusion matrix computed during evaluation.
-        evaluation_target (numpy.ndarray): True labels for evaluation.
-        evaluation_prediction (numpy.ndarray): Predicted labels for evaluation.
-
     """
     def evaluate_result(self):
         """
         Computes and displays evaluation metrics such as accuracy, precision, recall, f1-score, and confusion matrix.
         """
-        import numpy as np
-        import matplotlib.pyplot as plt
-        from sklearn.metrics import classification_report, confusion_matrix, roc_curve, accuracy_score
+        from sklearn.metrics import confusion_matrix
         target = self.evaluation_target
         prediction = self.evaluation_prediction
         self.cm = confusion_matrix(y_true=target, y_pred=prediction)
         import numpy as np
         import pandas as pd
         import copy
         cm = self.cm
```

### Comparing `TorchEase-0.0.2/TorchEase/trainer.py` & `TorchEase-0.0.5/TorchEase/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
             self.train()
             if self.eval_loader:
                 self.eval()
                 if self.early_stop and self.early_stop.early_stop(validation_loss=self.eval_loss, verbose=self.eval_verbose and self.verbose):
                     break
         self.test()
 
-
     def train(self):
         """
         Trains the model on the training dataset.
         """
         self.model.train()
         for batch, (feature, target) in enumerate(self.train_loader):
             feature, target = feature.to(self.device), target.to(self.device)
@@ -142,16 +141,14 @@
             for batch, (feature, target) in enumerate(self.test_loader):
                 feature, target = feature.to(self.device), target.to(self.device)
                 prediction = self.model(feature)
                 self.test_target.append(target)
                 self.test_prediction.append(prediction)
             self.test_target = torch.stack(self.test_target, dim=0).reshape(-1)
             self.test_prediction = torch.stack(self.test_prediction, dim=0).reshape(-1, self.n_classes)
-        #from sklearn.metrics import classification_report, confusion_matrix, roc_curve, accuracy_score
-        #self.cm = confusion_matrix(test_target=self.target, y_pred=self.fused_prediction)
 
         self.evaluation_target = self.test_target.detach().cpu().numpy()
         self.evaluation_prediction = self.test_prediction.argmax(1).detach().cpu().numpy()
 
     def save_model(self, path="model.pth"):
         """
         Saves the PyTorch model to the specified path.
```

### Comparing `TorchEase-0.0.2/TorchEase/user.py` & `TorchEase-0.0.5/TorchEase/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     >>> use_model.evaluate()
     """
     def __init__(self, model, n_classes, dataset, device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
         self.model = model.to(device)
         self.n_classes = n_classes
         self.test_loader = dataset
         self.device = device
+
     def evaluate(self):
         """
         Evaluate the user model on the test dataset and calculate evaluation metrics.
         """
         self.model.eval()
         self.test_target = []
         self.test_prediction = []
@@ -38,13 +39,10 @@
             for batch, (feature, target) in enumerate(self.test_loader):
                 feature, target = feature.to(self.device), target.to(self.device)
                 prediction = self.model(feature)
                 self.test_target.append(target)
                 self.test_prediction.append(prediction)
             self.test_target = torch.stack(self.test_target, dim=0).reshape(-1)
             self.test_prediction = torch.stack(self.test_prediction, dim=0).reshape(-1, self.n_classes)
-        #from sklearn.metrics import classification_report, confusion_matrix, roc_curve, accuracy_score
-        #self.cm = confusion_matrix(test_target=self.target, y_pred=self.fused_prediction)
-
         self.evaluation_target = self.test_target.detach().cpu().numpy()
         self.evaluation_prediction = self.test_prediction.argmax(1).detach().cpu().numpy()
         self.evaluate_result()
```

### Comparing `TorchEase-0.0.2/TorchEase/utilities.py` & `TorchEase-0.0.5/TorchEase/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,35 @@
 class EarlyStopper:
     """
     Early stopper that stops training if the validation loss does not improve
     for a given number of epochs.
 
     Parameters
     ----------
-        patience (int): The number of epochs to wait if the validation loss
-            does not improve before stopping early.
-        min_delta (float): The minimum change in validation loss to be
-            considered as an improvement.
+        patience (int):
+            The number of epochs to wait if the validation loss does not improve before stopping early.
+        min_delta (float):
+            The minimum change in validation loss to be considered as an improvement.
 
-    Attributes:
-        patience (int): The number of epochs to wait if the validation loss
-            does not improve before stopping early.
-        min_delta (float): The minimum change in validation loss to be
-            considered as an improvement.
-        counter (int): The number of epochs that the validation loss has not
-            improved.
-        min_loss (float): The best validation loss so far.
+    Attributes
+    ----------
+        patience (int):
+            The number of epochs to wait if the validation loss does not improve before stopping early.
+        min_delta (float):
+            The minimum change in validation loss to be considered as an improvement.
+        counter (int):
+            The number of epochs that the validation loss has not improved.
+        min_loss (float):
+            The best validation loss so far.
+
+    Examples
+    --------
+    >>> from TorchEase import EarlyStopper
+    >>> early_stop = EarlyStopper(patience=15, min_delta=0.01)
+    >>> trainer = Trainer(model=model, optimizer=optimizer, loss_fn=loss_fn, early_stop=early_stop)
     """
     def __init__(self, patience=1, min_delta=0):
         self.patience = patience
         self.min_delta = min_delta
         self.counter = 0
         self.min_loss = np.inf
```

### Comparing `TorchEase-0.0.2/TorchEase.egg-info/PKG-INFO` & `TorchEase-0.0.5/TorchEase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.2
+Version: 0.0.5
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.2/setup.py` & `TorchEase-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
 DESCRIPTION = 'Simplifying working with PyTorch'
 LONG_DESCRIPTION = 'TorchEase is a Python package that simplifies working with PyTorch, a popular deep learning framework. It provides a set of easy-to-use tools for training, testing, and deploying machine learning models. TorchEase includes features like early stopping, model fusing, and model evaluation, among others, which help streamline the model development process. Additionally, TorchEase is designed to be highly modular, making it easy to integrate into existing PyTorch projects.'
 
+#with open(os.path.join(os.path.dirname(__file__), "TorchEase", "VERSION")) as version_file:
+#    version = version_file.read().strip()
+version = "0.0.5"
+
 # Setting up
 setup(
     name="TorchEase",
-    version=VERSION,
+    version=version,
     author="Philipp Steigerwald",
     author_email="info@b-stream.info",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=["scikit-learn", "matplotlib", "pandas", "torch"],
+    install_requires=["scikit-learn", "matplotlib", "pandas", "torch", "numpy", "scipy"],
     keywords=['python', 'torch', 'pytorch', 'early stop', 'trainer', 'tensor'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

