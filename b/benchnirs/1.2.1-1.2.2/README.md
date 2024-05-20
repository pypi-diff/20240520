# Comparing `tmp/benchnirs-1.2.1.tar.gz` & `tmp/benchnirs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchnirs-1.2.1.tar", last modified: Thu May 16 08:09:33 2024, max compression
+gzip compressed data, was "benchnirs-1.2.2.tar", last modified: Mon May 20 20:47:09 2024, max compression
```

## Comparing `benchnirs-1.2.1.tar` & `benchnirs-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.128163 benchnirs-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-16 08:09:24.000000 benchnirs-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11736 2024-05-16 08:09:33.128163 benchnirs-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11197 2024-05-16 08:09:24.000000 benchnirs-1.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 08:09:33.128163 benchnirs-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-16 08:09:24.000000 benchnirs-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.124163 benchnirs-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.126163 benchnirs-1.2.1/src/benchnirs/
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48933 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/learn.py
--rw-rw-rw-   0 root         (0) root         (0)    25059 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/load.py
--rw-rw-rw-   0 root         (0) root         (0)     2822 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.127163 benchnirs-1.2.1/src/benchnirs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11736 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:47:09.609653 benchnirs-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-20 20:47:00.000000 benchnirs-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7996 2024-05-20 20:47:09.609653 benchnirs-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7457 2024-05-20 20:47:00.000000 benchnirs-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:47:09.608653 benchnirs-1.2.2/benchnirs/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 20:47:00.000000 benchnirs-1.2.2/benchnirs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49450 2024-05-20 20:47:00.000000 benchnirs-1.2.2/benchnirs/learn.py
+-rw-rw-rw-   0 root         (0) root         (0)    25515 2024-05-20 20:47:00.000000 benchnirs-1.2.2/benchnirs/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2024-05-20 20:47:00.000000 benchnirs-1.2.2/benchnirs/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-20 20:47:00.000000 benchnirs-1.2.2/benchnirs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:47:09.609653 benchnirs-1.2.2/benchnirs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7996 2024-05-20 20:47:09.000000 benchnirs-1.2.2/benchnirs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-20 20:47:09.000000 benchnirs-1.2.2/benchnirs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 20:47:09.000000 benchnirs-1.2.2/benchnirs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-20 20:47:09.000000 benchnirs-1.2.2/benchnirs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-20 20:47:09.000000 benchnirs-1.2.2/benchnirs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 20:47:09.609653 benchnirs-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-20 20:47:00.000000 benchnirs-1.2.2/setup.py
```

### Comparing `benchnirs-1.2.1/LICENSE` & `benchnirs-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.1/setup.py` & `benchnirs-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="benchnirs",
-    version="1.2.1",
+    version="1.2.2",
     author="Johann Benerradi",
     author_email="johann.benerradi@gmail.com",
     description="Benchmarking framework for machine learning with fNIRS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/HanBnrd/benchnirs",
-    license='GNU GPLv3+',
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
+    license="GNU GPLv3+",
+    packages=setuptools.find_packages(),
     install_requires=[
+        "importlib",
+        "lazy_loader",
         "numpy",
         "pandas",
         "scipy",
         "mne",
         "matplotlib",
         "seaborn",
         "scikit-learn",
```

### Comparing `benchnirs-1.2.1/src/benchnirs/learn.py` & `benchnirs-1.2.2/benchnirs/learn.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 
 from pandas import DataFrame
 from torch.utils.data import DataLoader, Dataset
-from scipy.stats import linregress
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.metrics import (accuracy_score, precision_recall_fscore_support,
                              confusion_matrix)
 from sklearn.model_selection import (KFold, StratifiedKFold, GroupKFold,
                                      GridSearchCV, train_test_split)
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import LinearSVC
@@ -30,57 +29,15 @@
 C_LIST = [1e-3, 1e-2, 1e-1, 1e0]
 N_NEIGHBORS_LIST = list(range(1, 10))
 
 # Deep learning parameters
 PATIENCE = 5  # for early stopping
 
 
-def _extract_features(nirs, feature_list):
-    """
-    Perform feature extraction on NIRS data.
-
-    Parameters
-    ----------
-    nirs : array of shape (n_epochs, n_channels, n_times)
-        Processed NIRS data.
-
-    feature_list : list of strings
-        List of features to extract. The list can include ``'mean'`` for the
-        mean along the time axis, ``'std'`` for standard deviation along the
-        time axis and ``'slope'`` for the slope of the linear regression along
-        the time axis.
-
-    Returns
-    -------
-    nirs_features : array of shape (n_epochs, n_channels*n_features)
-        Features extracted from NIRS data.
-    """
-    nirs_features = []
-    for feature in feature_list:
-        if feature == 'mean':
-            feature = np.mean(nirs, axis=2)
-        elif feature == 'std':
-            feature = np.std(nirs, axis=2)
-        elif feature == 'slope':
-            x = range(nirs.shape[2])
-            feature = []
-            for epoch in nirs:
-                ep_slopes = []
-                for channel in epoch:
-                    ep_slopes.append(linregress(x, channel).slope)
-                feature.append(ep_slopes)
-        nirs_features.append(feature)
-
-    nirs_features = np.stack(nirs_features, axis=2)
-    nirs_features = nirs_features.reshape(len(nirs), -1)  # flatten data
-
-    return nirs_features
-
-
-def machine_learn(nirs, labels, groups, model, features, normalize=False,
+def machine_learn(nirs, labels, groups, model, normalize=None,
                   random_state=None, output_folder='./outputs'):
     """
     Perform nested k-fold cross-validation for standard machine learning models
     producing metrics and confusion matrices. The models include linear
     discriminant analysis (LDA), support vector classifier (SVC) with grid
     search for the regularization parameter (inner cross-validation), and
     k-nearest neighbors (kNN) with grid search for the number of neighbors
@@ -100,24 +57,19 @@
         cross-validation instead.
 
     model : string
         Standard machine learning to use. Either ``'lda'`` for a linear
         discriminant analysis, ``'svc'`` for a linear support vector
         classifier or ``'knn'`` for a k-nearest neighbors classifier.
 
-    features : list of strings
-        List of features to extract. The list can include ``'mean'`` for the
-        mean along the time axis, ``'std'`` for standard deviation along the
-        time axis and ``'slope'`` for the slope of the linear regression along
-        the time axis.
-
-    normalize : boolean
-        Whether to normalize data before feeding to the model with min-max
-        scaling based on the train set for each iteration of the outer
-        cross-validation. Defaults to ``False`` for no normalization.
+    normalize : tuple of integers | None
+        Axes on which to normalize data before feeding to the model with
+        min-max scaling based on the train set for each iteration of the outer
+        cross-validation. For example (0, 2) to normalize across epochs and
+        time. Defaults to ``None`` for no normalization.
 
     random_state : integer | None
         Controls the shuffling applied to data. Pass an integer for
         reproducible output across multiple function calls. Defaults to
         ``None`` for not setting the seed.
 
     output_folder : string
@@ -143,32 +95,29 @@
         of the outer cross-validation.
     """
     print(f'Machine learning: {model}')
 
     if not os.path.isdir(output_folder):
         os.makedirs(output_folder)
 
-    # Feature extraction
-    nirs = _extract_features(nirs, features)
-
     # K-fold cross-validator
     if groups is None:
         out_kf = StratifiedKFold(n_splits=OUTER_K)
         in_kf = StratifiedKFold(n_splits=INNER_K)
     else:
         out_kf = GroupKFold(n_splits=OUTER_K)
         in_kf = GroupKFold(n_splits=INNER_K)
     all_y_true = []
     all_y_pred = []
     accuracies = []
     additional_metrics = []
     all_hps = []
     out_split = out_kf.split(nirs, labels, groups)
     for k, out_idx in enumerate(out_split):
-        print(f'\tFOLD #{k+1}')
+        print(f'\tFOLD #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_train, labels_test = labels[out_idx[0]], labels[out_idx[1]]
 
         if groups is None:
             groups_train = None
             nirs_train, labels_train = shuffle(
                 nirs_train, labels_train, random_state=random_state)
@@ -178,32 +127,35 @@
                 nirs_train, labels_train, groups_train,
                 random_state=random_state)
 
         all_y_true += labels_test.tolist()
 
         # Min-max scaling
         if normalize:
-            maxs = nirs_train.max(axis=0)[np.newaxis, :]
-            mins = nirs_train.min(axis=0)[np.newaxis, :]
+            maxs = nirs_train.max(axis=normalize, keepdims=True)
+            mins = nirs_train.min(axis=normalize, keepdims=True)
             nirs_train = (nirs_train - mins) / (maxs - mins)
             nirs_test = (nirs_test - mins) / (maxs - mins)
 
+        nirs_train = nirs_train.reshape(len(nirs_train), -1)
+        nirs_test = nirs_test.reshape(len(nirs_test), -1)
+
         in_split = in_kf.split(nirs_train, labels_train, groups_train)
 
         # LDA
         if model == 'lda':
             lda = LinearDiscriminantAnalysis()
             lda.fit(nirs_train, labels_train)
             y_pred = lda.predict(nirs_test).tolist()
             all_hps.append(None)
 
         # SVC
         elif model == 'svc':
             parameters = {'C': C_LIST}
-            svc = LinearSVC(max_iter=MAX_ITER)
+            svc = LinearSVC(max_iter=MAX_ITER, dual='auto')
             clf = GridSearchCV(svc, parameters, scoring='accuracy',
                                cv=in_split)
             clf.fit(nirs_train, labels_train)
             y_pred = clf.predict(nirs_test).tolist()
             all_hps.append(clf.best_params_['C'])
 
         # kNN
@@ -255,14 +207,16 @@
     def __init__(self, n_classes):
         super(_ANNClassifier, self).__init__()
         self.fc1 = nn.Linear(12, 8)
         self.fc2 = nn.Linear(8, 4)
         self.fc3 = nn.Linear(4, n_classes)
 
     def forward(self, x):
+        batch_size = x.size(0)
+        x = x.view(batch_size, -1)
         x = F.relu(self.fc1(x))
         x = F.relu(self.fc2(x))
         x = self.fc3(x)
         return x
 
 
 class _CNNClassifier(nn.Module):
@@ -409,14 +363,17 @@
                 val_accuracies.append(correct / total)
                 last_sorted = sorted(val_losses[-PATIENCE:])
                 if epoch >= PATIENCE and val_losses[-PATIENCE:] == last_sorted:
                     print(f'\t\t>Early stopping after {epoch+1} epochs')
                     break
         # scheduler.step()
 
+    if device_count > 1:
+        clf = clf.module
+
     results = {'train_losses': train_losses,
                'train_accuracies': train_accuracies,
                'val_losses': val_losses,
                'val_accuracies': val_accuracies}
     return clf, results
 
 
@@ -459,16 +416,16 @@
             running_loss += loss.item()
         results = {'test_loss': running_loss / (i+1),
                    'test_accuracy': correct / total,
                    'y_true': y_true, 'y_pred': y_pred}
     return results
 
 
-def deep_learn(nirs, labels, groups, model_class, features=None,
-               normalize=False, batch_sizes=[4, 8, 16, 32, 64],
+def deep_learn(nirs, labels, groups, model_class, normalize=None,
+               batch_sizes=[4, 8, 16, 32, 64],
                lrs=[1e-5, 1e-4, 1e-3, 1e-2, 1e-1], max_epoch=100,
                random_state=None, output_folder='./outputs'):
     """
     Perform nested k-fold cross-validation for a deep learning model. Produces
     loss graph, accuracy graph and confusion matrice. This is made with early
     stopping (with a validation set of 20 %) once the model has been fine tuned
     on the inner loop of the nested k-fold cross-validation. The number of
@@ -489,25 +446,19 @@
 
     model_class : string | PyTorch nn.Module class
         The PyTorch model class to use. If a string, can be either ``'ann'``,
         ``'cnn'`` or ``'lstm'``. If a PyTorch ``nn.Module`` class, the
         ``__init__()`` method must accept the number of classes as a parameter,
         and this needs to be the number of output neurons.
 
-    features : list of strings | None
-        List of features to extract. The list can include ``'mean'`` for the
-        mean along the time axis, ``'std'`` for standard deviation along the
-        time axis and ``'slope'`` for the slope of the linear regression along
-        the time axis. Defaults to ``None`` for no feature extration and using
-        the raw data.
-
-    normalize : boolean
-        Whether to normalize data before feeding to the model with min-max
-        scaling based on the train set for each iteration of the outer
-        cross-validation. Defaults to ``False`` for no normalization.
+    normalize : tuple of integers | None
+        Axes on which to normalize data before feeding to the model with
+        min-max scaling based on the train set for each iteration of the outer
+        cross-validation. For example (0, 2) to normalize across epochs and
+        time. Defaults to ``None`` for no normalization.
 
     batch_sizes : list of integers
         List of batch sizes to test for optimization.
 
     lrs : list of floats
         List of learning rates to test for optimization.
 
@@ -526,15 +477,15 @@
     Returns
     -------
     accuracies : list of floats
         List of accuracies on the test sets (one for each iteration of the
         outer cross-validation).
 
     all_hps : list of tuples
-        List of hyperparameters (one tuple for each iteration of the outer
+        List of best hyperparameters (one tuple for each iteration of the outer
         cross-validation). Each tuple will be `(batch size, learning rate)`.
 
     additional_metrics : list of tuples
         List of tuples of metrics composed of (precision, recall, F1 score) on
         the outer cross-validation (one tuple for each iteration of the outer
         cross-validation). This uses the ``precision_recall_fscore_support``
         function from scikit-learn with ``average='weighted'``, ``y_true`` and
@@ -552,122 +503,136 @@
     elif model_class == 'cnn':
         model_class = _CNNClassifier
     elif model_class == 'lstm':
         model_class = _LSTMClassifier
 
     print(f'Deep learning: {model_class.__name__}')
 
-    # Feature extraction
-    if features is not None:
-        nirs = _extract_features(nirs, features)
-
+    # Outer split
     if os.path.isfile(f'{output_folder}/split.pickle'):
-        print('\tSaved training found, loading it...')
+        print('\tSaved k-fold split found, loading it...', end=' ')
         with open(f'{output_folder}/split.pickle', 'rb') as f:
             out_split = pickle.load(f)
-        print('\tDone!')
-
+        print('Done!')
     else:
         if groups is None:
             out_kf = StratifiedKFold(n_splits=OUTER_K)
-            in_kf = StratifiedKFold(n_splits=INNER_K)
         else:
             out_kf = GroupKFold(n_splits=OUTER_K)
-            in_kf = GroupKFold(n_splits=INNER_K)
         out_split = list(out_kf.split(nirs, labels, groups))
 
         if not os.path.isdir(output_folder):
             os.makedirs(output_folder)
         with open(f'{output_folder}/split.pickle', 'wb') as f:
             pickle.dump(out_split, f)
 
-        for k, out_idx in enumerate(out_split):
-            print(f'\tTraining outer fold #{k}')
-            nirs_train = nirs[out_idx[0]]
-            labels_train = labels[out_idx[0]]
-
-            if groups is None:
-                groups_train = None
-                nirs_train, labels_train = shuffle(
-                    nirs_train, labels_train, random_state=random_state)
-            else:
-                groups_train = groups[out_idx[0]]
-                nirs_train, labels_train, groups_train = shuffle(
-                    nirs_train, labels_train, groups_train,
-                    random_state=random_state)
+    # Inner split
+    if groups is None:
+        in_kf = StratifiedKFold(n_splits=INNER_K)
+    else:
+        in_kf = GroupKFold(n_splits=INNER_K)
 
-            # Min-max scaling
-            if normalize:
-                if features is not None:
-                    maxs = nirs_train.max(axis=0)[np.newaxis, :]
-                    mins = nirs_train.min(axis=0)[np.newaxis, :]
-                else:
-                    maxs = nirs_train.max(axis=(0, 2))
-                    maxs = maxs[np.newaxis, :, np.newaxis]
-                    mins = nirs_train.min(axis=(0, 2))
-                    mins = mins[np.newaxis, :, np.newaxis]
-                nirs_train = (nirs_train - mins) / (maxs - mins)
+    for k, out_idx in enumerate(out_split):
+        print(f'\tTraining outer fold #{k}')
+        nirs_train = nirs[out_idx[0]]
+        labels_train = labels[out_idx[0]]
 
+        if groups is None:
+            groups_train = None
+            nirs_train, labels_train = shuffle(
+                nirs_train, labels_train, random_state=random_state)
+        else:
+            groups_train = groups[out_idx[0]]
+            nirs_train, labels_train, groups_train = shuffle(
+                nirs_train, labels_train, groups_train,
+                random_state=random_state)
+
+        # Min-max scaling
+        if normalize:
+            maxs = nirs_train.max(axis=normalize, keepdims=True)
+            mins = nirs_train.min(axis=normalize, keepdims=True)
+            nirs_train = (nirs_train - mins) / (maxs - mins)
+
+        if os.path.isfile(f'{output_folder}/model_k{k}.pt'):
+            print('\t\tClassifier checkpoint found, skipping training')
+        else:
             # Train classifier for each combination of hyperparameters
             hp_list = list(itertools.product(batch_sizes, lrs))
-            in_accuracies = [[] for _ in hp_list]
-            for i, hp in enumerate(hp_list):
-                batch_size, lr = hp[0], hp[1]
-                in_split = in_kf.split(nirs_train, labels_train, groups_train)
-                for in_idx in in_split:
-                    nirs_in_train = nirs_train[in_idx[0]]
-                    labels_in_train = labels_train[in_idx[0]]
-                    nirs_val = nirs_train[in_idx[1]]
-                    labels_val = labels_train[in_idx[1]]
-
-                    clf = model_class(n_classes).double()
-                    clf, _ = _train_dl(nirs_in_train, labels_in_train,
-                                       clf, batch_size, lr, max_epoch,
-                                       early_stop=False,
-                                       random_state=random_state)
-                    results = _test_dl(nirs_val, labels_val, clf)
-                    in_accuracies[i].append(results['test_accuracy'])
-
-            # Get best hyperparameters
-            in_average_accuracies = np.mean(in_accuracies, axis=1)
-            index_best = np.argmax(in_average_accuracies)
-            best_hps = hp_list[index_best]
+            if len(hp_list) > 1:
+                in_accuracies = [[] for _ in hp_list]
+                for i, hp in enumerate(hp_list):
+                    batch_size, lr = hp[0], hp[1]
+                    in_split = in_kf.split(nirs_train, labels_train,
+                                           groups_train)
+                    for in_idx in in_split:
+                        nirs_in_train = nirs_train[in_idx[0]]
+                        labels_in_train = labels_train[in_idx[0]]
+                        nirs_val = nirs_train[in_idx[1]]
+                        labels_val = labels_train[in_idx[1]]
+
+                        clf = model_class(n_classes).double()
+                        clf, _ = _train_dl(nirs_in_train, labels_in_train,
+                                           clf, batch_size, lr, max_epoch,
+                                           early_stop=False,
+                                           random_state=random_state)
+                        results = _test_dl(nirs_val, labels_val, clf)
+                        in_accuracies[i].append(results['test_accuracy'])
+
+                # Get best hyperparameters
+                in_average_accuracies = np.mean(in_accuracies, axis=1)
+                index_best = np.argmax(in_average_accuracies)
+                best_hps = hp_list[index_best]
+            else:
+                best_hps = (batch_sizes[0], lrs[0])
 
             # Retrain with best hyperparameters
             clf = model_class(n_classes).double()
             clf, results = _train_dl(nirs_train, labels_train,
                                      clf, best_hps[0], best_hps[1], max_epoch,
                                      early_stop=True,
                                      random_state=random_state)
 
             # Save trained model and training results
+            clf.cpu()
             torch.save(clf.state_dict(), f'{output_folder}/model_k{k}.pt')
             with open(f'{output_folder}/hps_k{k}.pickle', 'wb') as f:
                 pickle.dump(best_hps, f)
             with open(f'{output_folder}/results_k{k}.pickle', 'wb') as f:
                 pickle.dump(results, f)
 
+            # Plot outer fold loss graph
+            _, ax = plt.subplots(figsize=(12, 6))
+            epochs = [epoch for epoch in range(len(results['train_losses']))]
+            dict_losses = {'Epoch': epochs,
+                           'Training': results['train_losses'],
+                           'Validation': results['val_losses']}
+            df_losses = DataFrame(dict_losses)
+            df_losses = df_losses.melt(
+                id_vars=['Epoch'], value_vars=['Training', 'Validation'],
+                var_name='Condition', value_name='Loss')
+            sns.lineplot(ax=ax, data=df_losses, y='Loss', x='Epoch',
+                         hue='Condition', estimator=None)
+            plt.savefig(f'{output_folder}/k{k}_graph.png',
+                        bbox_inches='tight')
+            plt.close()
+
     all_ks, all_epochs = [], []
     all_train_losses, all_val_losses = [], []
     all_train_accuracies, all_val_accuracies = [], []
     all_y_true, all_y_pred = [], []
     accuracies, all_hps, additional_metrics = [], [], []
     for k, out_idx in enumerate(out_split):
         print(f'\tTesting outer fold #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_test = labels[out_idx[1]]
 
-        # Min-max scaling
+        # Min-max scaling of test set using training set only to avoid leakage
         if normalize:
-            if features is not None:
-                maxs = nirs_train.max(axis=0)[np.newaxis, :]
-                mins = nirs_train.min(axis=0)[np.newaxis, :]
-            else:
-                maxs = nirs_train.max(axis=(0, 2))[np.newaxis, :, np.newaxis]
-                mins = nirs_train.min(axis=(0, 2))[np.newaxis, :, np.newaxis]
+            maxs = nirs_train.max(axis=normalize, keepdims=True)
+            mins = nirs_train.min(axis=normalize, keepdims=True)
             nirs_test = (nirs_test - mins) / (maxs - mins)
 
         # Load trained model, hyperparameters and training results
         clf = model_class(n_classes).double()
         clf.load_state_dict(torch.load(f'{output_folder}/model_k{k}.pt'))
         with open(f'{output_folder}/hps_k{k}.pickle', 'rb') as f:
             best_hps = pickle.load(f)
@@ -688,15 +653,15 @@
         all_y_true += results['y_true']
         all_y_pred += results['y_pred']
         accuracies.append(results['test_accuracy'])
         prfs = precision_recall_fscore_support(
             results['y_true'], results['y_pred'], average='weighted')
         additional_metrics.append(prfs[:-1])
 
-    # Plot loss and accuracy graphs
+    # Plot all loss and accuracy graphs
     _, axes = plt.subplots(ncols=2, figsize=(16, 6))
     dict_losses = {'k': all_ks, 'Epoch': all_epochs,
                    'Training': all_train_losses,
                    'Validation': all_val_losses}
     df_losses = DataFrame(dict_losses)
     df_losses = df_losses.melt(id_vars=['k', 'Epoch'],
                                value_vars=['Training', 'Validation'],
@@ -803,14 +768,18 @@
                     running_loss += loss.item()
                 val_losses.append(running_loss / (i+1))
                 last_sorted = sorted(val_losses[-PATIENCE:])
                 if epoch >= PATIENCE and val_losses[-PATIENCE:] == last_sorted:
                     print(f'\t\t>Early stopping after {epoch+1} epochs')
                     break
 
+    if device_count > 1:
+        encoder = encoder.module
+        decoder = decoder.module
+
     results = {'train_losses': train_losses,
                'val_losses': val_losses}
     return encoder, decoder, results
 
 
 def _test_encdec(x_test, y_test, encoder, decoder):
     """
@@ -849,68 +818,75 @@
 
 
 def _proxy_optim(nirs_train, targets_train, groups_train, enc_class, dec_class,
                  batch_sizes, lrs, max_epoch, random_state, output_folder):
     """
     Train and optimise encoder-decoder.
     """
+    if random_state:
+        torch.manual_seed(random_state)
 
     if not os.path.isdir(output_folder):
         os.makedirs(output_folder)
 
     if groups_train is None:
         in_kf = KFold(n_splits=INNER_K)
     else:
         in_kf = GroupKFold(n_splits=INNER_K)
 
     # Encoder-decoder optimization
     hp_list = list(itertools.product(batch_sizes, lrs))
-    in_losses = [[] for _ in hp_list]
-    for i, hp in enumerate(hp_list):
-        batch_size, lr = hp[0], hp[1]
-        in_split = in_kf.split(nirs_train, targets_train, groups_train)
-        for in_idx in in_split:
-            nirs_in_train = nirs_train[in_idx[0]]
-            targets_in_train = targets_train[in_idx[0]]
-            nirs_val = nirs_train[in_idx[1]]
-            targets_val = targets_train[in_idx[1]]
-
-            encoder = enc_class().double()
-            decoder = dec_class().double()
-            encoder, decoder, _ = _train_encdec(
-                nirs_in_train, targets_in_train, encoder, decoder,
-                batch_size, lr, max_epoch, early_stop=False,
-                random_state=random_state)
+    if len(hp_list) > 1:
+        in_losses = [[] for _ in hp_list]
+        for i, hp in enumerate(hp_list):
+            batch_size, lr = hp[0], hp[1]
+            in_split = in_kf.split(nirs_train, targets_train, groups_train)
+            for in_idx in in_split:
+                nirs_in_train = nirs_train[in_idx[0]]
+                targets_in_train = targets_train[in_idx[0]]
+                nirs_val = nirs_train[in_idx[1]]
+                targets_val = targets_train[in_idx[1]]
+
+                encoder = enc_class().double()
+                decoder = dec_class().double()
+                encoder, decoder, _ = _train_encdec(
+                    nirs_in_train, targets_in_train, encoder, decoder,
+                    batch_size, lr, max_epoch, early_stop=False,
+                    random_state=random_state)
 
-            results = _test_encdec(nirs_val, targets_val, encoder, decoder)
-            in_losses[i].append(results['test_loss'])
+                results = _test_encdec(nirs_val, targets_val, encoder, decoder)
+                in_losses[i].append(results['test_loss'])
 
-    # Get best hyperparameters
-    in_average_losses = np.mean(in_losses, axis=1)
-    index_best = np.argmin(in_average_losses)
-    best_hps = hp_list[index_best]
+        # Get best hyperparameters
+        in_average_losses = np.mean(in_losses, axis=1)
+        index_best = np.argmin(in_average_losses)
+        best_hps = hp_list[index_best]
+    else:
+        best_hps = (batch_sizes[0], lrs[0])
 
     # Retrain with best hyperparameters
     encoder = enc_class().double()
     decoder = dec_class().double()
     encoder, decoder, results = _train_encdec(
         nirs_train, targets_train, encoder, decoder,
         best_hps[0], best_hps[1], max_epoch, early_stop=True,
         random_state=random_state)
 
     # Save trained model and training results
+    encoder.cpu()
+    decoder.cpu()
     torch.save(encoder.state_dict(), f'{output_folder}/encoder.pt')
     torch.save(decoder.state_dict(), f'{output_folder}/decoder.pt')
     with open(f'{output_folder}/hps.pickle', 'wb') as f:
         pickle.dump(best_hps, f)
     with open(f'{output_folder}/results.pickle', 'wb') as f:
         pickle.dump(results, f)
 
     # Plot loss graph
-    _, ax = plt.subplots(figsize=(16, 6))
+    _, ax = plt.subplots(figsize=(12, 6))
     epochs = [epoch for epoch in range(len(results['train_losses']))]
     dict_losses = {'Epoch': epochs,
                    'Training': results['train_losses'],
                    'Validation': results['val_losses']}
     df_losses = DataFrame(dict_losses)
     df_losses = df_losses.melt(id_vars=['Epoch'],
                                value_vars=['Training', 'Validation'],
@@ -920,15 +896,15 @@
     plt.savefig(f'{output_folder}/graph.png', bbox_inches='tight')
     plt.close()
 
     return encoder, decoder
 
 
 def deep_transfer_learn(nirs, labels, groups, enc_class, dec_class,
-                        model_class, features=None, normalize=False,
+                        model_class, normalize=None,
                         batch_sizes=[4, 8, 16, 32, 64],
                         lrs=[1e-5, 1e-4, 1e-3, 1e-2, 1e-1], max_epoch=100,
                         random_state=None, output_folder='./outputs'):
     """
     Perform nested k-fold cross-validation for a deep transfer learning model.
     Produces loss graphs, accuracy graph and confusion matrice. This is made
     with early stopping (with a validation set of 20 %) once the model has been
@@ -958,25 +934,19 @@
     model_class : PyTorch nn.Module class
         The PyTorch classifier class to use for the overall classification
         containing the Hb encoders. The ``__init__()`` method must accept the
         number of classes, an encoder for HbO and an encoder for HbR as
         parameters. The number of classes needs to be the number of output
         neurons.
 
-    features : list of strings | None
-        List of features to extract. The list can include ``'mean'`` for the
-        mean along the time axis, ``'std'`` for standard deviation along the
-        time axis and ``'slope'`` for the slope of the linear regression along
-        the time axis. Defaults to ``None`` for no feature extration and using
-        the raw data.
-
-    normalize : boolean
-        Whether to normalize data before feeding to the model with min-max
-        scaling based on the train set for each iteration of the outer
-        cross-validation. Defaults to ``False`` for no normalization.
+    normalize : tuple of integers | None
+        Axes on which to normalize data before feeding to the model with
+        min-max scaling based on the train set for each iteration of the outer
+        cross-validation. For example (0, 2) to normalize across epochs and
+        time. Defaults to ``None`` for no normalization.
 
     batch_sizes : list of integers
         List of batch sizes to test for optimization.
 
     lrs : list of floats
         List of learning rates to test for optimization.
 
@@ -995,173 +965,208 @@
     Returns
     -------
     accuracies : list of floats
         List of accuracies for the overall classifier on the test sets (one for
         each iteration of the outer cross-validation).
 
     all_hps : list of tuples
-        List of hyperparameters for the overall classifier (one tuple for each
-        iteration of the outer cross-validation). Each tuple will be
+        List of best hyperparameters for the overall classifier (one tuple for
+        each iteration of the outer cross-validation). Each tuple will be
         `(batch size, learning rate)`.
 
     additional_metrics : list of tuples
         List of tuples of metrics composed of (precision, recall, F1 score) on
         the outer cross-validation (one tuple for each iteration of the outer
         cross-validation). This uses the ``precision_recall_fscore_support``
         function from scikit-learn with ``average='weighted'``, ``y_true`` and
         ``y_pred`` being the true and the predictions on the specific iteration
         of the outer cross-validation.
+
+    :meta private:
     """
+    if random_state:
+        torch.manual_seed(random_state)
+
     print(f'Labels: {set(labels)}')
     if 8 in set(labels):
         n_classes = len(set(labels)) - 1  # minus unlabelled
     else:
         n_classes = len(set(labels))
 
     print(f'Deep transfer learning: {enc_class.__name__}/'
           f'{dec_class.__name__}-{model_class.__name__}')
 
-    # Feature extraction
-    if features is not None:
-        nirs = _extract_features(nirs, features)
-
     # Get index to split channel types
     mid_idx = nirs.shape[1] / 2
     if mid_idx.is_integer():
         mid_idx = int(mid_idx)
 
+    # Outer split
     if os.path.isfile(f'{output_folder}/split.pickle'):
-        print('\tSaved training found, loading it...')
+        print('\tSaved k-fold split found, loading it...', end=' ')
         with open(f'{output_folder}/split.pickle', 'rb') as f:
             out_split = pickle.load(f)
-        print('\tDone!')
-
+        print('Done!')
     else:
         if groups is None:
             out_kf = StratifiedKFold(n_splits=OUTER_K)
-            in_kf = StratifiedKFold(n_splits=INNER_K)
         else:
             out_kf = GroupKFold(n_splits=OUTER_K)
-            in_kf = GroupKFold(n_splits=INNER_K)
         out_split = list(out_kf.split(nirs, labels, groups))
 
         if not os.path.isdir(output_folder):
-            os.mkdir(output_folder)
+            os.makedirs(output_folder)
         with open(f'{output_folder}/split.pickle', 'wb') as f:
             pickle.dump(out_split, f)
 
-        for k, out_idx in enumerate(out_split):
-            print(f'\tTraining outer fold #{k}')
-            nirs_train = nirs[out_idx[0]]
-            labels_train = labels[out_idx[0]]
-
-            if groups is None:
-                groups_train = None
-                nirs_train, labels_train = shuffle(
-                    nirs_train, labels_train, random_state=random_state)
-            else:
-                groups_train = groups[out_idx[0]]
-                nirs_train, labels_train, groups_train = shuffle(
-                    nirs_train, labels_train, groups_train,
-                    random_state=random_state)
+    # Inner split
+    if groups is None:
+        in_kf = StratifiedKFold(n_splits=INNER_K)
+    else:
+        in_kf = GroupKFold(n_splits=INNER_K)
 
-            # Min-max scaling
-            if normalize:
-                if features is not None:
-                    maxs = nirs_train.max(axis=0)[np.newaxis, :]
-                    mins = nirs_train.min(axis=0)[np.newaxis, :]
-                else:
-                    maxs = nirs_train.max(axis=(0, 2))
-                    maxs = maxs[np.newaxis, :, np.newaxis]
-                    mins = nirs_train.min(axis=(0, 2))
-                    mins = mins[np.newaxis, :, np.newaxis]
-                nirs_train = (nirs_train - mins) / (maxs - mins)
-
-            # Train and optimise proxy models
-            nirs_train_hbo = nirs_train[:, mid_idx:, :]
-            nirs_train_hbr = nirs_train[:, :mid_idx, :]
+    for k, out_idx in enumerate(out_split):
+        print(f'\tTraining outer fold #{k}')
+        nirs_train = nirs[out_idx[0]]
+        labels_train = labels[out_idx[0]]
+
+        if groups is None:
+            groups_train = None
+            nirs_train, labels_train = shuffle(
+                nirs_train, labels_train, random_state=random_state)
+        else:
+            groups_train = groups[out_idx[0]]
+            nirs_train, labels_train, groups_train = shuffle(
+                nirs_train, labels_train, groups_train,
+                random_state=random_state)
+
+        # Min-max scaling
+        if normalize:
+            maxs = nirs_train.max(axis=normalize, keepdims=True)
+            mins = nirs_train.min(axis=normalize, keepdims=True)
+            nirs_train = (nirs_train - mins) / (maxs - mins)
+
+        # Train and optimise self-supervised models
+        nirs_train_hbo = nirs_train[:, mid_idx:, :]
+        nirs_train_hbr = nirs_train[:, :mid_idx, :]
+        # HbO -> HbR
+        if os.path.isfile(f'{output_folder}/k{k}/hbo/encoder.pt'):
+            print('\t\tSaved HbO encoder found, loading it...', end=' ')
+            enc_hbo = enc_class().double()
+            enc_hbo.load_state_dict(
+                torch.load(f'{output_folder}/k{k}/hbo/encoder.pt'))
+            print('Done!')
+        else:
             enc_hbo, _ = _proxy_optim(
                 nirs_train_hbo, nirs_train_hbr, groups_train,
                 enc_class, dec_class, batch_sizes=batch_sizes, lrs=lrs,
                 max_epoch=max_epoch, random_state=random_state,
                 output_folder=f'{output_folder}/k{k}/hbo')
+        # HbR -> HbO
+        if os.path.isfile(f'{output_folder}/k{k}/hbr/encoder.pt'):
+            print('\t\tSaved HbR encoder found, loading it...', end=' ')
+            enc_hbr = enc_class().double()
+            enc_hbr.load_state_dict(
+                torch.load(f'{output_folder}/k{k}/hbr/encoder.pt'))
+            print('Done!')
+        else:
             enc_hbr, _ = _proxy_optim(
                 nirs_train_hbr, nirs_train_hbo, groups_train,
                 enc_class, dec_class, batch_sizes=batch_sizes, lrs=lrs,
                 max_epoch=max_epoch, random_state=random_state,
                 output_folder=f'{output_folder}/k{k}/hbr')
 
+        if os.path.isfile(f'{output_folder}/k{k}/clf.pt'):
+            print('\t\tClassifier checkpoint found, skipping training')
+        else:
             # Train classifier for each combination of hyperparameters
             hp_list = list(itertools.product(batch_sizes, lrs))
-            in_accuracies = [[] for _ in hp_list]
-            for i, hp in enumerate(hp_list):
-                batch_size, lr = hp[0], hp[1]
-                in_split = in_kf.split(nirs_train, labels_train, groups_train)
-                for in_idx in in_split:
-                    nirs_in_train = nirs_train[in_idx[0]]
-                    labels_in_train = labels_train[in_idx[0]]
-                    nirs_val = nirs_train[in_idx[1]]
-                    labels_val = labels_train[in_idx[1]]
-
-                    # Remove unlabelled examples
-                    idx_in_train = np.where(np.array(labels_in_train) != 8)
-                    labels_in_train = labels_in_train[idx_in_train]
-                    nirs_in_train = nirs_in_train[idx_in_train]
-                    idx_val = np.where(np.array(labels_val) != 8)
-                    labels_val = labels_val[idx_val]
-                    nirs_val = nirs_val[idx_val]
-
-                    clf = model_class(n_classes, enc_hbo, enc_hbr).double()
-                    clf, _ = _train_dl(nirs_in_train, labels_in_train,
-                                       clf, batch_size, lr, max_epoch,
-                                       early_stop=False,
-                                       random_state=random_state)
-                    results = _test_dl(nirs_val, labels_val, clf)
-                    in_accuracies[i].append(results['test_accuracy'])
-
-            # Get best hyperparameters
-            in_average_accuracies = np.mean(in_accuracies, axis=1)
-            index_max = np.argmax(in_average_accuracies)
-            best_hps = hp_list[index_max]
+            if len(hp_list) > 1:
+                in_accuracies = [[] for _ in hp_list]
+                for i, hp in enumerate(hp_list):
+                    batch_size, lr = hp[0], hp[1]
+                    in_split = in_kf.split(nirs_train, labels_train,
+                                           groups_train)
+                    for in_idx in in_split:
+                        nirs_in_train = nirs_train[in_idx[0]]
+                        labels_in_train = labels_train[in_idx[0]]
+                        nirs_val = nirs_train[in_idx[1]]
+                        labels_val = labels_train[in_idx[1]]
+
+                        # Remove unlabelled examples
+                        idx_in_train = np.where(np.array(labels_in_train) != 8)
+                        labels_in_train = labels_in_train[idx_in_train]
+                        nirs_in_train = nirs_in_train[idx_in_train]
+                        idx_val = np.where(np.array(labels_val) != 8)
+                        labels_val = labels_val[idx_val]
+                        nirs_val = nirs_val[idx_val]
+
+                        clf = model_class(n_classes, enc_hbo, enc_hbr).double()
+                        clf, _ = _train_dl(nirs_in_train, labels_in_train,
+                                           clf, batch_size, lr, max_epoch,
+                                           early_stop=False,
+                                           random_state=random_state)
+                        results = _test_dl(nirs_val, labels_val, clf)
+                        in_accuracies[i].append(results['test_accuracy'])
+
+                # Get best hyperparameters
+                in_average_accuracies = np.mean(in_accuracies, axis=1)
+                index_max = np.argmax(in_average_accuracies)
+                best_hps = hp_list[index_max]
+            else:
+                best_hps = (batch_sizes[0], lrs[0])
 
             # Retrain with best hyperparameters
             idx_train = np.where(np.array(labels_train) != 8)
             labels_train = labels_train[idx_train]
             nirs_train = nirs_train[idx_train]
             clf = model_class(n_classes, enc_hbo, enc_hbr).double()
             clf, results = _train_dl(nirs_train, labels_train,
                                      clf, best_hps[0], best_hps[1], max_epoch,
                                      early_stop=True,
                                      random_state=random_state)
 
             # Save trained model and training results
+            clf.cpu()
             torch.save(clf.state_dict(), f'{output_folder}/k{k}/clf.pt')
             with open(f'{output_folder}/k{k}/hps.pickle', 'wb') as f:
                 pickle.dump(best_hps, f)
             with open(f'{output_folder}/k{k}/results.pickle', 'wb') as f:
                 pickle.dump(results, f)
 
+            # Plot outer fold loss graph
+            _, ax = plt.subplots(figsize=(12, 6))
+            epochs = [epoch for epoch in range(len(results['train_losses']))]
+            dict_losses = {'Epoch': epochs,
+                           'Training': results['train_losses'],
+                           'Validation': results['val_losses']}
+            df_losses = DataFrame(dict_losses)
+            df_losses = df_losses.melt(
+                id_vars=['Epoch'], value_vars=['Training', 'Validation'],
+                var_name='Condition', value_name='Loss')
+            sns.lineplot(ax=ax, data=df_losses, y='Loss', x='Epoch',
+                         hue='Condition', estimator=None)
+            plt.savefig(f'{output_folder}/k{k}/clf_graph.png',
+                        bbox_inches='tight')
+            plt.close()
+
     all_ks, all_epochs = [], []
     all_train_losses, all_val_losses = [], []
     all_train_accuracies, all_val_accuracies = [], []
     all_y_true, all_y_pred = [], []
     accuracies, all_hps, additional_metrics = [], [], []
     for k, out_idx in enumerate(out_split):
         print(f'\tTesting outer fold #{k}')
         nirs_train, nirs_test = nirs[out_idx[0]], nirs[out_idx[1]]
         labels_test = labels[out_idx[1]]
 
-        # Min-max scaling
+        # Min-max scaling of test set using training set only to avoid leakage
         if normalize:
-            if features is not None:
-                maxs = nirs_train.max(axis=0)[np.newaxis, :]
-                mins = nirs_train.min(axis=0)[np.newaxis, :]
-            else:
-                maxs = nirs_train.max(axis=(0, 2))[np.newaxis, :, np.newaxis]
-                mins = nirs_train.min(axis=(0, 2))[np.newaxis, :, np.newaxis]
+            maxs = nirs_train.max(axis=normalize, keepdims=True)
+            mins = nirs_train.min(axis=normalize, keepdims=True)
             nirs_test = (nirs_test - mins) / (maxs - mins)
 
         # Load trained model, hyperparameters and training results
         enc_hbo = enc_class().double()
         enc_hbr = enc_class().double()
         enc_hbo.load_state_dict(
             torch.load(f'{output_folder}/k{k}/hbo/encoder.pt'))
@@ -1191,15 +1196,15 @@
         all_y_true += results['y_true']
         all_y_pred += results['y_pred']
         accuracies.append(results['test_accuracy'])
         prfs = precision_recall_fscore_support(
             results['y_true'], results['y_pred'], average='weighted')
         additional_metrics.append(prfs[:-1])
 
-    # Plot loss and accuracy graphs
+    # Plot all loss and accuracy graphs
     _, axes = plt.subplots(ncols=2, figsize=(16, 6))
     dict_losses = {'k': all_ks, 'Epoch': all_epochs,
                    'Training': all_train_losses,
                    'Validation': all_val_losses}
     df_losses = DataFrame(dict_losses)
     df_losses = df_losses.melt(id_vars=['k', 'Epoch'],
                                value_vars=['Training', 'Validation'],
```

### Comparing `benchnirs-1.2.1/src/benchnirs/load.py` & `benchnirs-1.2.2/benchnirs/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,16 +490,16 @@
         labels[0, time_left] = 2
         labels[0, time_foot] = 3
         data['labels'] = labels
 
         return data
 
 
-def load_dataset(dataset, path=None, bandpass=None, order=4, tddr=False,
-                 baseline=(None, 0), roi_sides=False):
+def load_dataset(dataset, path, bandpass=None, order=4, tddr=False,
+                 baseline=(None, 0), roi_sides=False, downsample=10):
     """
     Load and filter one of the open access dataset.
 
     Parameters
     ----------
     dataset : string
         Dataset to load.
@@ -510,47 +510,51 @@
         ``'shin_2018_wg'`` for word generation from Shin et al., 2018
         (epoch interval: -2 to 10 seconds).
         ``'shin_2016_ma'`` for mental arithmetic from Shin et al., 2016
         (epoch interval: -2 to 10 seconds).
         ``'bak_2019_me'`` for motor execution from Bak et al., 2019
         (epoch interval: -2 to 10 seconds).
 
-    path : string | None
-        Path of the dataset selected with the ``dataset`` parameter. Defaults
-        to ``None`` to use the default path.
+    path : string
+        Path of the dataset selected with the ``dataset`` parameter.
 
     bandpass : list of floats | None
-        Cutoff frequencies of the bandpass Butterworth filter. Defaults to
-        ``None`` for no filtering.
+        Cutoff frequencies of the bandpass Butterworth filter (in Hz). Defaults
+        to ``None`` for no filtering.
 
     order : integer
         Order of the bandpass Butterworth filter.
 
     tddr : boolean
         Whether to apply temporal derivative distribution repair.
 
     baseline : None or tuple of length 2
-        The time interval to apply baseline correction. If ``None`` do not
-        apply it. If a tuple ``(a, b)`` the interval is between ``a`` and ``b``
-        (in seconds). If ``a`` is ``None`` the beginning of the data is used
-        and if ``b`` is ``None`` then ``b`` is set to the end of the interval.
-        If ``(None, None)`` all the time interval is used. Correction is
-        applied by computing mean of the baseline period and subtracting it
+        The time interval to apply baseline correction (in sec). If ``None`` do
+        not apply it. If a tuple ``(a, b)`` the interval is between ``a`` and
+        ``b`` (in seconds). If ``a`` is ``None`` the beginning of the data is
+        used and if ``b`` is ``None`` then ``b`` is set to the end of the
+        interval. If ``(None, None)`` all the time interval is used. Correction
+        is applied by computing mean of the baseline period and subtracting it
         from the data. The baseline ``(a, b)`` includes both endpoints, i.e.
         all timepoints ``t`` such that ``a <= t <= b``.
 
     roi_sides : boolean
-        Whether to average channels by side.
+        Whether to average channels by hemisphere in the task related regions
+        of interest.
+
+    downsample : float | None
+        Downsample data with the specified frequency (in Hz). Defaults to
+        ``10``. Ignored if ``None`` or higher than the dataset's original
+        sampling frequency.
 
     Returns
     -------
     epochs : MNE Epochs object
-        MNE epochs of filtered data with associated labels, downsampled to
-        10 Hz for comparison purposes. Subject IDs are contained in the
-        ``metadata`` property.
+        MNE epochs data with associated labels. Subject IDs are contained in
+        the ``metadata`` property.
     """
     print('Loading epochs...')
     raws = None
     groups = []
 
     if dataset == 'herff_2014_nb':
         loader = _DatasetHerff2014NB()
@@ -562,18 +566,21 @@
         loader = _DatasetShin2016MA()
     elif dataset == 'bak_2019_me':
         loader = _DatasetBak2019ME()
     else:
         loader = None
 
     for subj_id, subj in enumerate(loader.subject_list):
-        if path is None:
-            data = loader.load(subj)
-        else:
+        try:
             data = loader.load(subj, path)
+        except FileNotFoundError:
+            raise FileNotFoundError(
+                f"dataset not found, please make sure the dataset has been "
+                f"downloaded and the proper path has been provided (cf. "
+                f"https://hanbnrd.gitlab.io/benchnirs/install.html)")
 
         # Create MNE raw object from delta_c
         info = mne.create_info(ch_names=data['ch_names'], sfreq=data['sfreq'],
                                ch_types=data['ch_types'])
         raw = mne.io.RawArray(data['delta_c'], info, verbose=False)
 
         # TDDR
@@ -642,10 +649,13 @@
     # Cut epochs
     all_events = mne.find_events(raws, stim_channel='STI', shortest_event=1,
                                  verbose=False)
     groups = DataFrame(groups, columns=['Subject_ID'])
     epochs = mne.Epochs(raws, all_events, event_id=data['event_id'],
                         metadata=groups, preload=True, tmin=data['tmin'],
                         tmax=data['tmax'], baseline=baseline, verbose=False)
-    epochs.resample(10)  # resample to 10 Hz
+
+    # Downsample
+    if downsample and downsample < epochs.info['sfreq']:
+        epochs.resample(downsample)
 
     return epochs
```

### Comparing `benchnirs-1.2.1/src/benchnirs/viz.py` & `benchnirs-1.2.2/benchnirs/viz.py`

 * *Files identical despite different names*

