# Comparing `tmp/popfinder-0.0.3.tar.gz` & `tmp/popfinder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popfinder-0.0.3.tar", last modified: Wed Mar  1 00:53:17 2023, max compression
+gzip compressed data, was "popfinder-0.0.4.tar", last modified: Sat May  6 17:19:44 2023, max compression
```

## Comparing `popfinder-0.0.3.tar` & `popfinder-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 00:53:17.553769 popfinder-0.0.3/
--rw-rw-rw-   0        0        0     1085 2022-12-23 17:58:11.000000 popfinder-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    13429 2023-03-01 00:53:17.552769 popfinder-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13179 2023-02-07 21:53:38.000000 popfinder-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 00:53:17.533582 popfinder-0.0.3/popfinder/
--rw-rw-rw-   0        0        0      110 2022-12-28 16:34:34.000000 popfinder-0.0.3/popfinder/__init__.py
--rw-rw-rw-   0        0        0     3055 2023-01-23 17:09:25.000000 popfinder-0.0.3/popfinder/_helper.py
--rw-rw-rw-   0        0        0     4654 2023-02-07 18:32:24.000000 popfinder-0.0.3/popfinder/_multiboots.py
--rw-rw-rw-   0        0        0     1589 2023-01-23 17:09:35.000000 popfinder-0.0.3/popfinder/_neural_networks.py
--rw-rw-rw-   0        0        0       21 2023-03-01 00:51:18.000000 popfinder-0.0.3/popfinder/_version.py
--rw-rw-rw-   0        0        0     3639 2023-01-04 19:51:12.000000 popfinder-0.0.3/popfinder/_visualize.py
--rw-rw-rw-   0        0        0    17665 2023-01-24 17:42:58.000000 popfinder-0.0.3/popfinder/classifier.py
--rw-rw-rw-   0        0        0     4619 2023-01-24 00:32:55.000000 popfinder-0.0.3/popfinder/cli_classifier.py
--rw-rw-rw-   0        0        0     5362 2023-01-18 00:26:07.000000 popfinder-0.0.3/popfinder/cli_regressor.py
--rw-rw-rw-   0        0        0    13719 2023-01-24 17:12:22.000000 popfinder-0.0.3/popfinder/dataloader.py
--rw-rw-rw-   0        0        0    41317 2023-03-01 00:44:38.000000 popfinder-0.0.3/popfinder/regressor.py
-drwxrwxrwx   0        0        0        0 2023-03-01 00:53:17.546417 popfinder-0.0.3/popfinder.egg-info/
--rw-rw-rw-   0        0        0    13429 2023-03-01 00:53:17.000000 popfinder-0.0.3/popfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-03-01 00:53:17.000000 popfinder-0.0.3/popfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 00:53:17.000000 popfinder-0.0.3/popfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-03-01 00:53:17.000000 popfinder-0.0.3/popfinder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-03-01 00:53:17.000000 popfinder-0.0.3/popfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-01 00:53:17.554769 popfinder-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-02-07 22:39:42.000000 popfinder-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 00:53:17.549762 popfinder-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2022-12-23 18:27:11.000000 popfinder-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0    19624 2023-02-07 18:43:00.000000 popfinder-0.0.3/tests/test_popfinder.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.727401 popfinder-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2022-12-23 17:58:11.000000 popfinder-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    13429 2023-05-06 17:19:44.727401 popfinder-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13179 2023-02-07 21:53:38.000000 popfinder-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.707694 popfinder-0.0.4/popfinder/
+-rw-rw-rw-   0        0        0      110 2022-12-28 16:34:34.000000 popfinder-0.0.4/popfinder/__init__.py
+-rw-rw-rw-   0        0        0     3153 2023-05-05 16:35:33.000000 popfinder-0.0.4/popfinder/_helper.py
+-rw-rw-rw-   0        0        0     5077 2023-04-27 18:17:57.000000 popfinder-0.0.4/popfinder/_multiboots.py
+-rw-rw-rw-   0        0        0     1751 2023-04-19 23:55:13.000000 popfinder-0.0.4/popfinder/_neural_networks.py
+-rw-rw-rw-   0        0        0       21 2023-05-06 17:17:19.000000 popfinder-0.0.4/popfinder/_version.py
+-rw-rw-rw-   0        0        0     4039 2023-05-06 16:41:07.000000 popfinder-0.0.4/popfinder/_visualize.py
+-rw-rw-rw-   0        0        0    33410 2023-05-06 17:12:00.000000 popfinder-0.0.4/popfinder/classifier.py
+-rw-rw-rw-   0        0        0     4619 2023-01-24 00:32:55.000000 popfinder-0.0.4/popfinder/cli_classifier.py
+-rw-rw-rw-   0        0        0     5362 2023-01-18 00:26:07.000000 popfinder-0.0.4/popfinder/cli_regressor.py
+-rw-rw-rw-   0        0        0    14471 2023-05-05 16:34:03.000000 popfinder-0.0.4/popfinder/dataloader.py
+-rw-rw-rw-   0        0        0    42337 2023-04-27 18:04:52.000000 popfinder-0.0.4/popfinder/regressor.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.717293 popfinder-0.0.4/popfinder.egg-info/
+-rw-rw-rw-   0        0        0    13429 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:19:44.727401 popfinder-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-02-07 22:39:42.000000 popfinder-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.723782 popfinder-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-23 18:27:11.000000 popfinder-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    19624 2023-02-07 18:43:00.000000 popfinder-0.0.4/tests/test_popfinder.py
```

### Comparing `popfinder-0.0.3/LICENSE` & `popfinder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.3/PKG-INFO` & `popfinder-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popfinder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Genetic population assignment using neural networks
 Author: Katie Birchard
 Author-email: katie.birchard@apexrms.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # popfinder
```

### Comparing `popfinder-0.0.3/README.md` & `popfinder-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.3/popfinder/_helper.py` & `popfinder-0.0.4/popfinder/_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from torch.utils.data import DataLoader, TensorDataset
 from torch.autograd import Variable
 from sklearn import preprocessing
 import numpy as np
 import dill
 import os
 
-def _generate_train_inputs(data_obj, valid_size, cv_splits, cv_reps, seed=123):
+def _generate_train_inputs(data_obj, valid_size, cv_splits, cv_reps, seed=123, bootstrap=False):
 
     if cv_splits == 1:
-        train_input, valid_input = data_obj.split_train_test(data_obj.train, test_size=valid_size, seed=seed)
+        train_input, valid_input = data_obj.split_train_test(
+            data_obj.train, test_size=valid_size, seed=seed, bootstrap=bootstrap)
         inputs = [(train_input, valid_input)]
 
     elif cv_splits > 1:
-        inputs = data_obj.split_kfcv(data_obj.train, n_splits=cv_splits, n_reps=cv_reps, seed=seed)
+        inputs = data_obj.split_kfcv(
+            data_obj.train, n_splits=cv_splits, n_reps=cv_reps, seed=seed, bootstrap=bootstrap)
 
     return inputs
 
 def _split_input_classifier(clf, input):
         
     train_input, valid_input = input
 
@@ -51,15 +53,15 @@
     return X_train, y_train, X_valid, y_valid
 
 def _generate_data_loaders(X_train, y_train, X_valid, y_valid, batch_size=16):
 
     train = TensorDataset(X_train, y_train)
     train_loader = DataLoader(train, batch_size=batch_size, shuffle=True)
     valid = TensorDataset(X_valid, y_valid)
-    valid_loader = DataLoader(valid, batch_size=batch_size, shuffle=True)
+    valid_loader = DataLoader(valid, batch_size=len(valid.tensors[0]), shuffle=True)
 
     return train_loader, valid_loader
 
 def _data_converter(x, y, variable=False):
 
     features = torch.from_numpy(np.vstack(np.array(x)).astype(np.float32))
     if torch.isnan(features).sum() != 0:
```

### Comparing `popfinder-0.0.3/popfinder/_multiboots.py` & `popfinder-0.0.4/popfinder/_multiboots.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,59 +6,63 @@
 
 from popfinder.dataloader import GeneticData
 from popfinder.regressor import PopRegressor
 
 def _train_on_bootstraps(arg_list):
 
     popfinder_path, nboots, epochs, valid_size, cv_splits, cv_reps, learning_rate, batch_size, dropout_prop, rep = arg_list
-
-    popfinder = PopRegressor.load(os.path.join(popfinder_path, "regressor.pkl"))
-    popfinder.output_folder = os.path.join(popfinder_path, "rep{}".format(rep))
-    os.makedirs(popfinder.output_folder, exist_ok=True)
-
-    test_locs_final = pd.DataFrame({"sampleID": [], "pop": [], "x": [],
+    test_locs_final = pd.DataFrame({"bootstrap": [], "sampleID": [], "pop": [], "x": [],
                                     "y": [], "x_pred": [], "y_pred": []})
-    pred_locs_final = pd.DataFrame({"sampleID": [], "pop": [], 
-                                    "x_pred": [], "y_pred": []})    
-
-    # Use bootstrap to randomly select sites from training/test/unknown data
-    num_sites = popfinder.data.train["alleles"].values[0].shape[0]
+    pred_locs_final = pd.DataFrame({"bootstrap": [], "sampleID": [], "pop": [], 
+                                    "x_pred": [], "y_pred": []})   
+    for boot in range(nboots):
+
+        popfinder = PopRegressor.load(os.path.join(popfinder_path, "regressor.pkl"))
+        popfinder.output_folder = os.path.join(popfinder_path, "rep{}".format(rep))
+        os.makedirs(popfinder.output_folder, exist_ok=True)
 
-    for _ in range(nboots):
+        # Use bootstrap to randomly select sites from training/test/unknown data
+        num_sites = popfinder.data.train["alleles"].values[0].shape[0]
 
         site_indices = np.random.choice(range(num_sites), size=num_sites,
                                         replace=True)
 
-        boot_data = GeneticData()
-        boot_data.train = popfinder.data.train.copy()
-        boot_data.test = popfinder.data.test.copy()
-        boot_data.knowns = pd.concat([popfinder.data.train, popfinder.data.test])
-        boot_data.unknowns = popfinder.data.unknowns.copy()
+        popfinder.__boot_data = GeneticData()
+        popfinder.__boot_data.train = popfinder.data.train.copy()
+        popfinder.__boot_data.test = popfinder.data.test.copy()
+        popfinder.__boot_data.knowns = pd.concat([popfinder.data.train, popfinder.data.test])
+        popfinder.__boot_data.unknowns = popfinder.data.unknowns.copy()
 
         # Slice datasets by site_indices
-        boot_data.train["alleles"] = [a[site_indices] for a in popfinder.data.train["alleles"].values]
-        boot_data.test["alleles"] = [a[site_indices] for a in popfinder.data.test["alleles"].values]
-        boot_data.unknowns["alleles"] = [a[site_indices] for a in popfinder.data.unknowns["alleles"].values]
+        popfinder.__boot_data.train["alleles"] = [a[site_indices] for a in popfinder.data.train["alleles"].values]
+        popfinder.__boot_data.test["alleles"] = [a[site_indices] for a in popfinder.data.test["alleles"].values]
+        popfinder.__boot_data.unknowns["alleles"] = [a[site_indices] for a in popfinder.data.unknowns["alleles"].values]
 
         # Train on new training set
         popfinder.data
         popfinder.train(epochs=epochs, valid_size=valid_size,
                 cv_splits=cv_splits, cv_reps=cv_reps,
                 learning_rate=learning_rate, batch_size=batch_size,
-                dropout_prop=dropout_prop, boot_data=boot_data)
-        popfinder.test(boot_data=boot_data)
+                dropout_prop=dropout_prop)
+        popfinder.test()
         test_locs = popfinder.test_results.copy()
         test_locs["sampleID"] = test_locs.index
-        pred_locs = popfinder.assign_unknown(boot_data=boot_data, save=False)
+        test_locs["bootstrap"] = boot
+
+        if popfinder.data.unknowns.shape[0] > 0:
+
+            pred_locs = popfinder.assign_unknown(save=False)
+            pred_locs["bootstrap"] = boot
+            pred_locs_final = pd.concat([pred_locs_final,
+                pred_locs[["bootstrap", "sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
 
         test_locs_final = pd.concat([test_locs_final,
-            test_locs[["sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
-        pred_locs_final = pd.concat([pred_locs_final,
-            pred_locs[["sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
+            test_locs[["bootstrap", "sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
 
+        
     return test_locs_final, pred_locs_final
 
 
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-p", help="Path to PopRegressor object")
@@ -93,12 +97,16 @@
                                                dropout_prop, rep] for rep in range(nreps)])
     pool.close()
     pool.join()
 
     test_locs_final = pd.DataFrame()
     pred_locs_final = pd.DataFrame()
     for rep in range(nreps):
-        test_locs_final = pd.concat([test_locs_final, results[rep][0]])
-        pred_locs_final = pd.concat([pred_locs_final, results[rep][1]])
+        test_locs = results[rep][0]
+        pred_locs = results[rep][1]
+        test_locs["rep"] = rep
+        pred_locs["rep"] = rep
+        test_locs_final = pd.concat([test_locs_final, test_locs])
+        pred_locs_final = pd.concat([pred_locs_final, pred_locs])
 
-    test_locs_final.to_csv(os.path.join(popfinder_path, "test_locs_final.csv"))
-    pred_locs_final.to_csv(os.path.join(popfinder_path, "pred_locs_final.csv"))
+    test_locs_final.to_csv(os.path.join(popfinder_path, "test_locs_final.csv"), index=False)
+    pred_locs_final.to_csv(os.path.join(popfinder_path, "pred_locs_final.csv"), index=False)
```

### Comparing `popfinder-0.0.3/popfinder/_neural_networks.py` & `popfinder-0.0.4/popfinder/_neural_networks.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,20 @@
         super(RegressorNet, self).__init__()
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.fc1 = nn.Linear(input_size, hidden_size)
         self.batch1 = nn.BatchNorm1d(hidden_size)
         self.fc2 = nn.Linear(hidden_size, batch_size)
         self.batch2 = nn.BatchNorm1d(batch_size)
-        self.fc3 = nn.Linear(batch_size, 2)
+        self.fc3 = nn.Linear(batch_size, batch_size)
+        self.fc4 = nn.Linear(batch_size, 2)
+        self.fc5 = nn.Linear(2, 2)
         self.dropout = nn.Dropout(dropout_prop)
 
     def forward(self, x):
-        x = self.batch1(self.dropout(F.relu(self.fc1(x))))
-        x = self.batch2(self.dropout(F.relu(self.fc2(x))))
-        x = self.fc3(x)
+        x = self.batch1(self.dropout(F.elu(self.fc1(x))))
+        x = self.batch2(self.dropout(F.elu(self.fc2(x))))
+        x = F.elu(self.fc3(x))
+        x = F.elu(self.fc3(x))
+        x = self.fc5(self.fc4(x))
 
         return x
```

### Comparing `popfinder-0.0.3/popfinder/_visualize.py` & `popfinder-0.0.4/popfinder/_visualize.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 import matplotlib.pyplot as plt
 from matplotlib.colors import ListedColormap
 import pandas as pd
 import numpy as np
 import itertools
 import os
 
-def _plot_training_curve(train_history, nn_type, output_folder, save):
+def _plot_training_curve(train_history, nn_type, output_folder, save, facet_by_split_rep):
 
-    plt.switch_backend("agg")
-    fig = plt.figure(figsize=(3, 1.5), dpi=200)
-    plt.rcParams.update({"font.size": 7})
-    ax1 = fig.add_axes([0, 0, 1, 1])
-    ax1.plot(train_history["valid"][3:], "--", color="black",
-        lw=0.5, label="Validation Loss")
-    ax1.plot(train_history["train"][3:], "-", color="black",
-        lw=0.5, label="Training Loss")
-    ax1.set_xlabel("Epoch")
-    ax1.legend()
+    plot_data = train_history.rename(columns={"valid": "validation"})
+    plot_data = pd.melt(plot_data, id_vars=["epoch", "split", "rep"], 
+            value_vars=["train", "validation"], 
+            var_name="dataset", value_name="loss")
+
+    d = {'color': ['C0', 'k'], "ls" : ["-","--"]}
+
+    if facet_by_split_rep:
+        g = sns.FacetGrid(plot_data, col="split", row="rep", 
+                          hue="dataset", hue_kws=d, height=2, aspect=1.5)
+    else:
+        g = sns.FacetGrid(plot_data, hue="dataset", hue_kws=d, height=2, aspect=1.5)
+    
+    g.map(sns.lineplot, "epoch", "loss", lw=0.5)
+    g.add_legend(title="")
 
     if save:
-        fig.savefig(os.path.join(output_folder, nn_type + "_training_history.png"),
+        g.savefig(os.path.join(output_folder, nn_type + "_training_history.png"),
             bbox_inches="tight")
 
 def _plot_confusion_matrix(test_results, confusion_matrix, nn_type,
     output_folder, save):
 
     true_labels = test_results["true_pop"] # test w/ classifier
 
@@ -45,22 +50,25 @@
             color="white" if cm[i, j] > thresh else "black")
     plt.tight_layout()
 
     if save:
         plt.savefig(os.path.join(output_folder, nn_type + "_confusion_matrix.png"))
 
 def _plot_assignment(e_preds, col_scheme, output_folder,
-    nn_type, save):
-
+    nn_type, save, best_model_only):
+        
     e_preds.set_index("sampleID", inplace=True)
 
     if nn_type == "regressor":
-        e_preds = pd.get_dummies(e_preds["classification"])
+        e_preds = pd.get_dummies(e_preds["classification"], dtype=float)
     elif nn_type == "classifier":
-        e_preds = pd.get_dummies(e_preds["assigned_pop"])
+        e_preds = pd.get_dummies(e_preds["assigned_pop"], dtype=float)
+
+    if not best_model_only:
+        e_preds = e_preds.reset_index().groupby("sampleID").mean()
 
     num_classes = len(e_preds.columns)
 
     sns.set()
     sns.set_style("ticks")
     e_preds.plot(kind="bar", stacked=True,
         colormap=ListedColormap(sns.color_palette(col_scheme, num_classes)),
```

### Comparing `popfinder-0.0.3/popfinder/cli_classifier.py` & `popfinder-0.0.4/popfinder/cli_classifier.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.3/popfinder/cli_regressor.py` & `popfinder-0.0.4/popfinder/cli_regressor.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.3/popfinder/dataloader.py` & `popfinder-0.0.4/popfinder/dataloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,26 +125,31 @@
         """
         # Split data into known and unknown
         unknown = data[data["pop"].isnull()]
         known = data[data["pop"].notnull()]
 
         return known, unknown
 
-    def split_train_test(self, data=None, stratify_by_pop=True, test_size=0.2, seed=123):
+    def split_train_test(self, data=None, stratify_by_pop=True, test_size=0.2, seed=123, bootstrap=False):
         """
         Splits data into training and testing sets.
         
         Parameters
-        ----------  
+        ----------
+        data : Pandas DataFrame
+            Contains information on corresponding sampleID and
+            genetic information. This is the output of `read_data()`.  
         stratify_by_pop : bool
             Whether to stratify the data by population. Default is True.
         test_size : float
             Proportion of data to be used for testing. Default is 0.2.
         seed : int
             Random seed for reproducibility. Default is 123.
+        bootstrap : bool
+            Whether to bootstrap the training data. Default is False.
             
         Returns
         -------
         train : Pandas DataFrame
             Contains information on corresponding sampleID and
             genetic information for training samples.
         test : Pandas DataFrame
@@ -153,30 +158,35 @@
         """
         # Split data into training and testing
         if stratify_by_pop is True:
             train, test = self._stratified_split(data, test_size=test_size, seed=seed)
         else:
             train, test = self._random_split(data, test_size=test_size, seed=seed)
 
+        if bootstrap:
+            train = train.sample(frac=1, replace=True, random_state=seed)
+
         return train, test
 
-    def split_kfcv(self, data=None, n_splits=5, n_reps=1, seed=123, stratify_by_pop=True):
+    def split_kfcv(self, data=None, n_splits=5, n_reps=1, seed=123, stratify_by_pop=True, bootstrap=False):
         """
         Splits data into training and testing sets.
 
         Parameters
         ----------
         n_splits : int
             Number of splits for cross-validation. Default is 5.
         n_reps : int
             Number of repetitions for cross-validation. Default is 1.
         stratify_by_pop : bool
             Whether to stratify the data by population. Default is True.
         seed : int
             Seed for random number generator. Default is 123.
+        bootstrap : bool
+            Whether to bootstrap the training data. Default is False.
 
         Returns
         -------
         list of tuples
             Each tuple contains a training and testing set. The length
             of the list is n_splits * n_reps.
         """
@@ -191,21 +201,29 @@
 
         if stratify_by_pop:
             for _, (train_ind, test_ind) in enumerate(rskf.split(known_data["alleles"],
                                                                  known_data["pop"], 
                                                                  groups=known_data["pop"])):
                 train = known_data.iloc[train_ind]
                 test = known_data.iloc[test_ind]
+
+                if bootstrap:
+                    train = train.sample(frac=1, replace=True, random_state=seed)
+
                 dataset_tuple = (train, test)
                 dataset_list.append(dataset_tuple)
         else:
             for _, (train_ind, test_ind) in enumerate(rskf.split(known_data["alleles"], 
                                                                  known_data["pop"])):
                 train = known_data.iloc[train_ind]
                 test = known_data.iloc[test_ind]
+
+                if bootstrap:
+                    train = train.sample(frac=1, replace=True, random_state=seed)
+                    
                 dataset_tuple = (train, test)
                 dataset_list.append(dataset_tuple)
 
         return dataset_list
 
     def _initialize(self, test_size=0.2, seed=123):
```

### Comparing `popfinder-0.0.3/popfinder/regressor.py` & `popfinder-0.0.4/popfinder/regressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 from torch.autograd import Variable
+from torch.optim.lr_scheduler import ReduceLROnPlateau
 from scipy import spatial
 from scipy import stats
 from sklearn.metrics import accuracy_score, confusion_matrix, f1_score, precision_score, recall_score
 from subprocess import call
 import matplotlib.pyplot as plt
 import matplotlib.image as mpimg
 import matplotlib
@@ -85,15 +86,15 @@
     classification_f1 : float
         Classification F1 score.
     classification_confusion_matrix : numpy.ndarray
         Classification confusion matrix.
 
     Methods
     -------
-    train(epochs=100, valid_size=0.2, cv_splits=1, cv_reps=1, learning_rate=0.001, batch_size=16, dropout_prop=0, boot_data=None)
+    train(epochs=100, valid_size=0.2, cv_splits=1, cv_reps=1, learning_rate=0.001, batch_size=16, dropout_prop=0)
         Train the regressor.
     test()
         Test the regressor.
     assign_unknown()
         Assign unknown samples.
     rank_site_importance()
         Rank the importance of each site.
@@ -118,14 +119,15 @@
 
         self.__data = data # GeneticData object
         self.__nboots = nboots
         self.__random_state = random_state
         if output_folder is None:
             output_folder = os.getcwd()
         self.__output_folder = output_folder
+        self.__boot_data = None
         self.__train_history = None
         self.__best_model = None
         self.__test_results = None
         self.__regression = None
         self.__median_distance = None
         self.__mean_distance = None
         self.__r2_lat = None
@@ -158,14 +160,22 @@
         return self.__output_folder
 
     @output_folder.setter
     def output_folder(self, output_folder):
         self.__output_folder = output_folder
 
     @property
+    def boot_data(self):
+        return self.__boot_data
+    
+    @boot_data.setter
+    def boot_data(self, boot_data):
+        self.__boot_data = boot_data
+
+    @property
     def train_history(self):
         return self.__train_history
 
     @property
     def best_model(self):
         return self.__best_model
 
@@ -230,15 +240,15 @@
         return self.__nn_type
 
     @property
     def lowest_val_loss(self):
         return self.__lowest_val_loss
 
     def train(self, epochs=100, valid_size=0.2, cv_splits=1, cv_reps=1,
-              learning_rate=0.001, batch_size=16, dropout_prop=0, boot_data=None):
+              learning_rate=0.001, batch_size=16, dropout_prop=0):
         """
         Trains the regression neural network to estimate xy coordinates of 
         a sample's origin.
         
         Parameters
         ----------
         epochs : int, optional
@@ -251,80 +261,119 @@
             Number of cross-validation repetitions. The default is 1.
         learning_rate : float, optional
             Learning rate for the neural network. The default is 0.001.
         batch_size : int, optional
             Batch size for the neural network. The default is 16.
         dropout_prop : float, optional
             Dropout proportion for the neural network. The default is 0.
-        boot_data : GeneticData, optional
-            GeneticData object to use for bootstrapping. This argument
-            is used internally. The default is None.
             
         Returns
         -------
         None.
         """
         self._validate_train_inputs(epochs, valid_size, cv_splits, cv_reps,
-                            learning_rate, batch_size, dropout_prop, boot_data)
+                            learning_rate, batch_size, dropout_prop)
 
-        if boot_data is None:
+        if self.__boot_data is None:
             inputs = _generate_train_inputs(self.data, valid_size, cv_splits,
                                             cv_reps, seed=self.random_state)
         else:
-            inputs = _generate_train_inputs(boot_data, valid_size, cv_splits,
+            inputs = _generate_train_inputs(self.__boot_data, valid_size, cv_splits,
                                             cv_reps, seed=self.random_state)
 
         loss_df_final = pd.DataFrame({"rep": [], "split": [], "epoch": [],
                                       "train": [], "valid": []})
+        lowest_val_loss = 9999
 
         for i, input in enumerate(inputs):
 
             X_train, y_train, X_valid, y_valid = _split_input_regressor(input)
-            net = RegressorNet(input_size=X_train.shape[1], hidden_size=16,
+            net = RegressorNet(input_size=X_train.shape[1], hidden_size=32,
                                batch_size=batch_size, dropout_prop=dropout_prop)
             optimizer = torch.optim.Adam(net.parameters(), lr=learning_rate)
-            loss_func = self._euclidean_dist_loss
+            scheduler = ReduceLROnPlateau(optimizer, factor=0.5)
+            # loss_func = self._euclidean_dist_loss
+            loss_func = torch.nn.MSELoss()
+
+            y_train = torch.tensor(self._normalize_locations(y_train))
+            y_valid = torch.tensor(self._normalize_locations(y_valid))
 
             train_loader, valid_loader = _generate_data_loaders(X_train, y_train,
                                                                 X_valid, y_valid)
+            loss_dict = {"epoch": [], "train": [], "valid": []}
+
+            for epoch in range(epochs):
+
+                train_loss = 0
+                valid_loss = 0
+
+                for _, (data, target) in enumerate(train_loader):
+                    optimizer.zero_grad()
+                    output = net(data)
+                    loss = loss_func(output.squeeze(), target.squeeze().float())
+                    loss.backward()
+                    optimizer.step()
+                    train_loss += loss.data.item()
+            
+                # Calculate average train loss
+                avg_train_loss = train_loss / len(train_loader)
+
+                for _, (data, target) in enumerate(valid_loader):
+                    output = net(data)
+                    loss = loss_func(output.squeeze(), target.squeeze().long())
+                    valid_loss += loss.data.item()
+
+                    if valid_loss < lowest_val_loss:
+                        lowest_val_loss = valid_loss
+                        torch.save(net, os.path.join(self.output_folder, "best_model.pt"))
+
+                # Step scheduler for LR decay
+                scheduler.step(valid_loss)
+
+                # Calculate average validation loss
+                avg_valid_loss = valid_loss / len(valid_loader)
+
+                loss_dict["epoch"].append(epoch)
+                loss_dict["train"].append(avg_train_loss)
+                loss_dict["valid"].append(avg_valid_loss)
+
+            loss_df = pd.DataFrame(loss_dict)
 
-            loss_df = self._fit_regressor_model(epochs, train_loader,
-                    valid_loader, net, optimizer, loss_func)
+            # loss_df = self._fit_regressor_model(epochs, train_loader,
+            #         valid_loader, net, optimizer, scheduler, loss_func)
 
             split = i % cv_splits + 1
             rep = int(i / cv_splits) + 1
 
             loss_df["rep"] = rep
             loss_df["split"] = split
 
-        loss_df_final = pd.concat([loss_df_final, loss_df])
+            loss_df_final = pd.concat([loss_df_final, loss_df])
 
         self.__train_history = loss_df_final
         self.__best_model = torch.load(os.path.join(self.output_folder, "best_model.pt"))
 
-    def test(self, boot_data=None, save=True, verbose=False):
+    def test(self, save=True, verbose=False):
         """
         Tests the regression neural network on the test data.
         
         Parameters
         ----------
-        boot_data : GeneticData, optional
-            GeneticData object to use for bootstrapping. The default is None.
         verbose : bool, optional
             Whether to print the test results. The default is False.
 
         Returns
         -------
         None.
         """
         
-        if boot_data is None:
+        if self.__boot_data is None:
             test_input = self.data.test
         else:
-            test_input = boot_data.test
+            test_input = self.__boot_data.test
 
         X_test = test_input["alleles"]    
         y_test = test_input[["x", "y"]]
         X_test, y_test = _data_converter(X_test, y_test)
         y_test = self._unnormalize_locations(y_test)
 
         y_pred = self.best_model(X_test).detach().numpy()
@@ -352,34 +401,32 @@
 
         self.__summary = self.get_assignment_summary()
 
         if verbose:
             print(self.summary)
 
 
-    def assign_unknown(self, save=True, boot_data=None):
+    def assign_unknown(self, save=True):
         """
         Assigns unknown samples to their predicted origin.
         
         Parameters
         ----------
         save : bool, optional
             Whether to save the results to a csv file. The default is True.
-        boot_data : GeneticData, optional
-            GeneticData object to use for bootstrapping. The default is None.
         
         Returns
         -------
         None.
         """
         
-        if boot_data is None:
+        if self.__boot_data is None:
             unknown_data = self.data.unknowns
         else:
-            unknown_data = boot_data.unknowns
+            unknown_data = self.__boot_data.unknowns
 
         X_unknown = unknown_data["alleles"]
         X_unknown = _data_converter(X_unknown, None)
 
         y_pred = self.best_model(X_unknown).detach().numpy()
         y_pred = self._unnormalize_locations(y_pred)
         unknown_data.loc[:, "x_pred"] = y_pred[:, 0]
@@ -388,14 +435,43 @@
         self.__regression = unknown_data
 
         if save:
             unknown_data.to_csv(os.path.join(self.output_folder,
                                 "regressor_assignment_results.csv"))
 
         return unknown_data
+    
+    def perform_bootstrap_regression(self, nboots=5, nreps=5,
+        epochs=100, valid_size=0.2, cv_splits=1, cv_reps=1,
+        learning_rate=0.001, batch_size=16, dropout_prop=0, 
+        jobs=-1, save_plots=True, save=True):
+        """
+        Generates many predictions using bootstraps of the original data.
+
+        Parameters
+        ----------
+        nboots : int, optional
+            Number of bootstraps to perform. The default is 5.
+        nreps : int, optional
+            Number of repetitions for each bootstrap. The default is 5.
+        save_plots : bool, optional
+            Whether to save the contour plots. The default is True.
+        save : bool, optional
+            Whether to save the classification results. The default is True.
+        
+        Returns
+        -------
+        None.
+        """
+        self._generate_bootstrap_results(nboots, nreps, epochs, valid_size,
+                                  cv_splits, cv_reps, learning_rate, batch_size,
+                                  dropout_prop, jobs) 
+
+        test_locs = self.test_locs_final
+        pred_locs = self.pred_locs_final
 
     def classify_by_contours(self, nboots=5, nreps=5, num_contours=5,
         epochs=100, valid_size=0.2, cv_splits=1, cv_reps=1,
         learning_rate=0.001, batch_size=16, dropout_prop=0, 
         jobs=-1, save_plots=True, save=True):
         """
         Classifies unknown samples by kernel density estimates (contours).
@@ -418,15 +494,15 @@
         
         Returns
         -------
         None.
         """
         self._validate_contour_inputs(nboots, num_contours, save_plots, save)
 
-        self._generate_bootstraps(nboots, nreps, epochs, valid_size,
+        self._generate_bootstrap_results(nboots, nreps, epochs, valid_size,
                                   cv_splits, cv_reps, learning_rate, batch_size,
                                   dropout_prop, jobs) 
 
         test_locs = self.test_locs_final
         pred_locs = self.pred_locs_final
 
         self.__classification_test_results = self._test_classification(test_locs,
@@ -704,14 +780,17 @@
         save : bool, optional
             Whether to save the plot to a png file. The default is True.
         
         Returns
         -------
         None.
         """
+        if self.classification_test_results is None:
+            raise ValueError("No classification results to plot.")
+
         _plot_confusion_matrix(self.classification_test_results,
             self.classification_confusion_matrix,
             self.nn_type, self.output_folder, save)
 
 
     def plot_assignment(self, save=True, col_scheme="Spectral"):
         """
@@ -795,18 +874,26 @@
         -------
         None
         """
         return _load(load_path)
 
     # Hidden functions below
     def _fit_regressor_model(self, epochs, train_loader, valid_loader, 
-                             net, optimizer, loss_func):
+                             net, optimizer, scheduler, loss_func):
 
         loss_dict = {"epoch": [], "train": [], "valid": []}
 
+        # Testing
+        # model = nn.Sequential(
+        #     nn.Linear(2, 10),
+        #     nn.ReLU(),
+        #     nn.Linear(10, 1)
+        # )
+        ####
+
         for epoch in range(epochs):
 
             train_loss = 0
             valid_loss = 0
 
             for _, (data, target) in enumerate(train_loader):
                 optimizer.zero_grad()
@@ -824,14 +911,17 @@
                 loss = loss_func(output.squeeze(), target.squeeze().long())
                 valid_loss += loss.data.item()
 
                 if valid_loss < self.lowest_val_loss:
                     self.__lowest_val_loss = valid_loss
                     torch.save(net, os.path.join(self.output_folder, "best_model.pt"))
 
+            # Step scheduler for LR decay
+            scheduler.step(valid_loss)
+
             # Calculate average validation loss
             avg_valid_loss = valid_loss / len(valid_loader)
 
             loss_dict["epoch"].append(epoch)
             loss_dict["train"].append(avg_train_loss)
             loss_dict["valid"].append(avg_valid_loss)
 
@@ -846,67 +936,31 @@
         loss = np.sqrt(np.sum(np.square(y_pred - y_true)))
         loss = Variable(torch.tensor(loss), requires_grad=True)
 
         return loss
 
     def _unnormalize_locations(self, y_pred):
 
-        y_pred_norm = np.array(
+        y_pred_unnorm = np.array(
             [[x[0] * self.data.sdlong + self.data.meanlong,
               x[1] * self.data.sdlat + self.data.meanlat
             ] for x in y_pred])
 
-        return y_pred_norm
-
-    def _train_on_bootstraps(self, arg_list):
-
-        nboots, epochs, valid_size, cv_splits, cv_reps, learning_rate, batch_size, dropout_prop = arg_list
+        return y_pred_unnorm
+    
+    def _normalize_locations(self, y_pred):
 
-        test_locs_final = pd.DataFrame({"sampleID": [], "pop": [], "x": [],
-                                        "y": [], "x_pred": [], "y_pred": []})
-        pred_locs_final = pd.DataFrame({"sampleID": [], "pop": [], 
-                                        "x_pred": [], "y_pred": []})    
-
-        # Use bootstrap to randomly select sites from training/test/unknown data
-        num_sites = self.data.train["alleles"].values[0].shape[0]
-
-        for _ in range(nboots):
-
-            site_indices = np.random.choice(range(num_sites), size=num_sites,
-                                            replace=True)
-
-            boot_data = GeneticData()
-            boot_data.train = self.data.train.copy()
-            boot_data.test = self.data.test.copy()
-            boot_data.knowns = pd.concat([self.data.train, self.data.test])
-            boot_data.unknowns = self.data.unknowns.copy()
-
-            # Slice datasets by site_indices
-            boot_data.train["alleles"] = [a[site_indices] for a in self.data.train["alleles"].values]
-            boot_data.test["alleles"] = [a[site_indices] for a in self.data.test["alleles"].values]
-            boot_data.unknowns["alleles"] = [a[site_indices] for a in self.data.unknowns["alleles"].values]
-
-            # Train on new training set
-            self.train(epochs=epochs, valid_size=valid_size,
-                    cv_splits=cv_splits, cv_reps=cv_reps,
-                    learning_rate=learning_rate, batch_size=batch_size,
-                    dropout_prop=dropout_prop, boot_data=boot_data)
-            self.test(boot_data=boot_data, save=False)
-            test_locs = self.test_results.copy()
-            test_locs["sampleID"] = test_locs.index
-            pred_locs = self.assign_unknown(boot_data=boot_data, save=False)
-
-            test_locs_final = pd.concat([test_locs_final,
-                test_locs[["sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
-            pred_locs_final = pd.concat([pred_locs_final,
-                pred_locs[["sampleID", "pop", "x", "y", "x_pred", "y_pred"]]])
+        y_pred_norm = np.array(
+            [[(x[0] - self.data.meanlong) / self.data.sdlong,
+              (x[1] - self.data.meanlat) / self.data.sdlat
+            ] for x in y_pred])
 
-        return test_locs_final, pred_locs_final
+        return y_pred_norm
 
-    def _generate_bootstraps(self, nboots, nreps, epochs, valid_size,
+    def _generate_bootstrap_results(self, nboots, nreps, epochs, valid_size,
                              cv_splits, cv_reps, learning_rate, batch_size,
                              dropout_prop, jobs):
 
         # Create tempfolder
         tempfolder = tempfile.mkdtemp()
         self.save(save_path=tempfolder)
 
@@ -1082,15 +1136,15 @@
             if not isinstance(output_folder, str):
                 raise TypeError("output_folder must be a string")
 
             if not os.path.isdir(output_folder):
                 raise ValueError("output_folder must be a valid directory")
 
     def _validate_train_inputs(self, epochs, valid_size, cv_splits, cv_reps,
-                            learning_rate, batch_size, dropout_prop, boot_data):
+                            learning_rate, batch_size, dropout_prop):
 
         if not isinstance(epochs, int):
             raise TypeError("epochs must be an integer")
         
         if not isinstance(valid_size, float):
             raise TypeError("valid_size must be a float")
 
@@ -1114,18 +1168,14 @@
 
         if not isinstance(dropout_prop, float) and not isinstance(dropout_prop, int):
             raise TypeError("dropout_prop must be a float")
 
         if dropout_prop > 1 or dropout_prop < 0:
             raise ValueError("dropout_prop must be between 0 and 1")
 
-        if boot_data is not None:
-            if not isinstance(boot_data, GeneticData):
-                raise TypeError("boot_data must be an instance of GeneticData")
-
     def _validate_contour_inputs(self, nboots, num_contours, save_plots, save):
             
         if not isinstance(nboots, int):
             raise TypeError("nboots must be an integer")
 
         if not isinstance(num_contours, int):
             raise TypeError("num_contours must be an integer")
```

### Comparing `popfinder-0.0.3/popfinder.egg-info/PKG-INFO` & `popfinder-0.0.4/popfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popfinder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Genetic population assignment using neural networks
 Author: Katie Birchard
 Author-email: katie.birchard@apexrms.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # popfinder
```

### Comparing `popfinder-0.0.3/setup.py` & `popfinder-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.3/tests/test_popfinder.py` & `popfinder-0.0.4/tests/test_popfinder.py`

 * *Files identical despite different names*

