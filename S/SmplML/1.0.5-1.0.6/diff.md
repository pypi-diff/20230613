# Comparing `tmp/SmplML-1.0.5.tar.gz` & `tmp/SmplML-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SmplML-1.0.5.tar", last modified: Mon Jun 12 09:05:08 2023, max compression
+gzip compressed data, was "dist\SmplML-1.0.6.tar", last modified: Tue Jun 13 04:33:15 2023, max compression
```

## Comparing `SmplML-1.0.5.tar` & `SmplML-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:05:08.304169 SmplML-1.0.5/
--rw-rw-rw-   0        0        0      167 2023-06-12 09:04:12.000000 SmplML-1.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1086 2023-06-12 07:39:21.000000 SmplML-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       30 2023-06-12 07:39:19.000000 SmplML-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4159 2023-06-12 09:05:08.301602 SmplML-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3071 2023-06-12 09:03:38.000000 SmplML-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:05:08.291561 SmplML-1.0.5/SmplML.egg-info/
--rw-rw-rw-   0        0        0     4159 2023-06-12 09:05:07.000000 SmplML-1.0.5/SmplML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-12 09:05:08.000000 SmplML-1.0.5/SmplML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:05:07.000000 SmplML-1.0.5/SmplML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 09:05:07.000000 SmplML-1.0.5/SmplML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 09:05:07.000000 SmplML-1.0.5/SmplML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 09:05:08.304169 SmplML-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1436 2023-06-12 09:04:45.000000 SmplML-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:05:08.297613 SmplML-1.0.5/smpl_ml/
--rw-rw-rw-   0        0        0       46 2023-06-12 09:04:36.000000 SmplML-1.0.5/smpl_ml/__init__.py
--rw-rw-rw-   0        0        0    10140 2023-06-12 09:04:18.000000 SmplML-1.0.5/smpl_ml/smpl_ml.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:33:15.762853 SmplML-1.0.6/
+-rw-rw-rw-   0        0        0      223 2023-06-13 04:29:02.000000 SmplML-1.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-12 07:39:21.000000 SmplML-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-06-12 07:39:19.000000 SmplML-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    19267 2023-06-13 04:33:15.761597 SmplML-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    18123 2023-06-13 04:14:41.000000 SmplML-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 04:33:15.754964 SmplML-1.0.6/SmplML.egg-info/
+-rw-rw-rw-   0        0        0    19267 2023-06-13 04:33:15.000000 SmplML-1.0.6/SmplML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-13 04:33:15.000000 SmplML-1.0.6/SmplML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 04:33:15.000000 SmplML-1.0.6/SmplML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-13 04:33:15.000000 SmplML-1.0.6/SmplML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 04:33:15.000000 SmplML-1.0.6/SmplML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 04:33:15.762853 SmplML-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-06-13 04:32:35.000000 SmplML-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:33:15.759719 SmplML-1.0.6/smpl_ml/
+-rw-rw-rw-   0        0        0       46 2023-06-12 09:04:36.000000 SmplML-1.0.6/smpl_ml/__init__.py
+-rw-rw-rw-   0        0        0    11274 2023-06-13 04:04:57.000000 SmplML-1.0.6/smpl_ml/smpl_ml.py
```

### Comparing `SmplML-1.0.5/LICENSE` & `SmplML-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.5/setup.py` & `SmplML-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  
 dependencies = ['pandas', 
                 'numpy', 
                 'scikit-learn']
 
 setup(
   name='SmplML',
-  version='1.0.5',
+  version='1.0.6',
   description=desc,
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JhunBrian/SmplML',  
   author='Jhun Brian Andam',
   author_email='andam.jhunbrian@gmail.com',
   license='MIT',
```

### Comparing `SmplML-1.0.5/smpl_ml/smpl_ml.py` & `SmplML-1.0.6/smpl_ml/smpl_ml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
+
 
+########## Exception ########## 
 class VariableNotInitializedError(Exception):
     def __init__(self, variable_name, suggestion=None):
         self.variable_name = variable_name
         self.suggestion = suggestion
 
     def __str__(self):
         if self.suggestion:
             err = f"Variable '{self.variable_name}' is not initialized yet. {self.suggestion}"
         else:
             err = f"Variable '{self.variable_name}' is not initialized yet."
         return err
 
 
+########## Data Preparation ##########
 class Cat2Num:
-    """
-    Cat2Num: Categorical to Numerical
-    """
     def __init__(self):
+        """
+        Initializes an instance of the Cat2Num class.
+        """
         self.dict_map = {}
         
     def cat2num(self, df: pd.DataFrame):
         """
-        Convert categorical columns in the DataFrame to numerical representation.
-
+        Converts categorical columns in a DataFrame to numerical values using a mapping dictionary.
+        
         Args:
-            df (pd.DataFrame): The input DataFrame with categorical columns.
-
+            df (pd.DataFrame): The DataFrame containing categorical columns to be converted.
+        
         Returns:
-            pd.DataFrame: The DataFrame with categorical columns converted to numerical representation.
+            pd.DataFrame: A new DataFrame with categorical columns replaced by numerical values.
         """
         df = df.copy()
         for col in df:
             
             if df[col].dtype == 'object' or df[col].dtype == 'category':
                 if df[col].dtype == 'category':
                     df[col] = df[col].astype('object')
@@ -44,120 +47,91 @@
                     self.dict_map[col][orig] = repl
                     df[col].replace(orig, repl, inplace=True)
                     
         return df
     
     def num2cat(self, df: pd.DataFrame):
         """
-        Convert numerical representation of categorical columns back to their original values.
-
+        Converts numerical values in the DataFrame back to their original categorical values using the stored mapping dictionary.
+        
         Args:
-            df (pd.DataFrame): The input DataFrame with numerical representation of categorical columns.
-
+            df (pd.DataFrame): The DataFrame containing numerical values to be converted back to categorical values.
+        
         Returns:
-            pd.DataFrame: The DataFrame with numerical representation converted back to original categorical values.
+            pd.DataFrame: A new DataFrame with numerical values replaced by their original categorical values.
         
         Raises:
-            VariableNotInitializedError: If `cat2num()` has not been executed before calling `num2cat()`.
+            VariableNotInitializedError: If the `dict_map` variable is empty, indicating that 'cat2num()' has not been executed.
         """
         df = df.copy()
         if self.dict_map == {}:
             raise VariableNotInitializedError("dict_map", suggestion="Try executing 'cat2num()' first.")
             
         for col in df:
             if col in self.dict_map.keys():
                 for orig, repl in self.dict_map[col].items():
                     df[col].replace(repl, orig, inplace=True)
                     
         return df
-
-
+    
 def split_data(df, test_size=0.25, shuffle=True, random_state=143):
     """
-    Split the DataFrame into training and testing datasets.
+    Splits the provided DataFrame into train and test sets.
 
     Args:
-        df (pd.DataFrame): The input DataFrame to be split.
-        test_size (float, optional): The proportion of the DataFrame to be used for testing. Defaults to 0.25.
+        df (pd.DataFrame): The DataFrame to be split.
+        test_size (float, optional): The proportion of the DataFrame to be included in the test set. Defaults to 0.25.
         shuffle (bool, optional): Whether to shuffle the DataFrame before splitting. Defaults to True.
         random_state (int, optional): The random seed for shuffling the DataFrame. Defaults to 143.
 
     Returns:
-        tuple: A tuple containing the training and testing datasets.
+        Tuple[pd.DataFrame, pd.DataFrame]: A tuple containing the train and test DataFrames.
 
     """
     if shuffle:
         df = df.sample(frac=1, random_state=random_state)
     
     train = df[:-int(len(df) * test_size)]
     test = df[-int(len(df) * test_size):]
     return train, test
 
 
-def reg_metrics(y_true, y_pred):
-    """
-    Calculate performance metrics based on the provided y_true and y_pred.
-
-    Args:
-        y_true (np.ndarray): True data.
-        y_pred (np.ndarray): The rpedicted data.
-
-    Returns:
-        pd.DataFrame: A DataFrame containing performance metrics.
-
-    """
-    mse = np.mean((y_true - y_pred) ** 2)
-    rmse = np.sqrt(mse)
-    mae = np.mean(np.abs(y_true - y_pred))
-    r2 = 1 - (np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2))
-
-    dataframe = pd.DataFrame(data={'MSE': mse,
-                                   'RMSE': rmse,
-                                   'MAE': mae,
-                                   'R-squared': r2},
-                             index=['Metrics'])
-    
-    return dataframe.T
-
-
+########## Performance Metrics ##########
 def confusion_matrix(y_true, y_pred):
     """
-    Compute the confusion matrix based on the true and predicted labels.
+    Computes the confusion matrix based on the true and predicted labels.
 
     Args:
-        y_true (list or array-like): True labels.
-        y_pred (list or array-like): Predicted labels.
+        y_true (List[Any]): The true labels.
+        y_pred (List[Any]): The predicted labels.
 
     Returns:
-        list: Confusion matrix as a 2D list.
+        List[List[int]]: The confusion matrix.
+
     """
-    # Get unique labels
     labels = list(set(y_true).union(set(y_pred)))
     labels.sort()
 
-    # Initialize confusion matrix
     matrix = [[0] * len(labels) for _ in range(len(labels))]
 
-    # Populate confusion matrix
     for true, pred in zip(y_true, y_pred):
         matrix[labels.index(true)][labels.index(pred)] += 1
 
     return matrix
 
-
 def clf_metrics(matrix, class_labels):
     """
-    Calculate performance metrics based on the confusion matrix.
+    Computes various classification metrics based on the confusion matrix.
 
     Args:
         matrix (np.ndarray): The confusion matrix.
-        class_labels (list): The list of class labels.
+        class_labels (List[Any]): The list of class labels.
 
     Returns:
-        pd.DataFrame: A DataFrame containing performance metrics for each class.
+        pd.DataFrame: A DataFrame containing the classification metrics.
 
     """
     FP = np.sum(matrix, axis=0) - np.diag(matrix)
     FN = np.sum(matrix, axis=1) - np.diag(matrix)
     TP = np.diag(matrix)
     TN = np.sum(matrix) - (FP + FN + TP)
     FP = FP.astype(float)
@@ -169,111 +143,146 @@
     TNR = np.round(TN / (TN + FP), 2)
     PPV = np.round(TP / (TP + FP), 2)
     F1 = np.round(2 * (PPV * TPR) / (PPV + TPR), 2)
 
     dataframe = pd.DataFrame(data={'Recall': TPR,
                                    'Specificity': TNR,
                                    'Precision': PPV,
-                                   'F1-Score': F1},
+                                   'F1-Score': F1,
+                                   'Accuracy': np.round(np.sum(TP) / np.sum(matrix), 2)},
                              index=class_labels)
     dataframe.fillna(value=0, inplace=True)
-    dataframe['Accuracy'] = np.round(np.sum(TP) / np.sum(matrix), 2)
     return dataframe
 
+def reg_metrics(y_true, y_pred):
+    """
+    Computes various regression metrics based on the true and predicted values.
+
+    Args:
+        y_true (np.ndarray): The true values.
+        y_pred (np.ndarray): The predicted values.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the regression metrics.
+
+    """
+    mse = np.round(np.mean((y_true - y_pred) ** 2),2)
+    rmse = np.round(np.sqrt(mse),2)
+    mae = np.round(np.mean(np.abs(y_true - y_pred)),2)
+    r2 = np.round(1 - (np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2)),2)
+
+    dataframe = pd.DataFrame(data={'MSE': mse,
+                                   'RMSE': rmse,
+                                   'MAE': mae,
+                                   'R-squared': r2},
+                             index=['Metrics'])
+    
+    return dataframe
 
+
+########## Model Training Class ##########
 class TrainModel:
-    def __init__(self, df: pd.DataFrame, target: str, features: list, model, test_size=0.25, random_state=143, shuffle=True):
+    def __init__(self, df: pd.DataFrame, target: str, features: list, models, test_size=0.25, random_state=143, shuffle=True):
         """
-        Initialize the TrainClassifier object.
+        Initializes the TrainModel class.
 
         Args:
-            df (pd.DataFrame): The input DataFrame containing the data.
-            target (str): The name of the target variable column.
-            features (list): The list of feature columns.
-            model: The machine learning model to be trained.
-            test_size (float, optional): The proportion of the data to be used for testing. Defaults to 0.25.
-            random_state (int, optional): The random seed for data shuffling. Defaults to 143.
-            shuffle (bool, optional): Whether to shuffle the data before splitting. Defaults to True.
+            df (pd.DataFrame): The input DataFrame.
+            target (str): The target variable column name.
+            features (list): A list of feature column names.
+            models (Union[BaseEstimator, List[BaseEstimator]]): A single or a list of machine learning models.
+            test_size (float, optional): The proportion of the dataset to include in the test split. Defaults to 0.25.
+            random_state (int, optional): Random state for reproducibility. Defaults to 143.
+            shuffle (bool, optional): Whether to shuffle the dataset before splitting. Defaults to True.
         """
         self.__df = df.copy()
         self.__target = target
         self.__features = features
-        self.__model = model
+        self.__models = models if isinstance(models, list) else [models]  # Convert single model to a list
         self.__test_size = test_size
         self.__random_state = random_state
         self.__shuffle = shuffle
         
         self.__lbl_encoder = Cat2Num()
         self.__split_data = split_data
         self.__reg_metrics = reg_metrics
         self.__clf_metrics = clf_metrics
         self.__conf_matrix = confusion_matrix
-        self.__type = None
+        self.__type = 'regression' if np.issubdtype(self.__df[self.__target].dtype, np.floating) else 'classification'
         self.__train = None
         self.__test = None
-        self.__fitted_model = None
+        
+        self.fitted_models_dict = {}
+        self.results_df = None
         
     def fit(self, verbose=True):
         """
-        Fit the machine learning model using the training data.
+        Fits the machine learning models/model on the training data.
 
         Args:
-            verbose (bool, optional): Whether to display performance metrics. Defaults to True.
+            verbose (bool, optional): Whether to display verbose output during fitting. Defaults to True.
         """
         data = self.__lbl_encoder.cat2num(self.__df)
         train, test = self.__split_data(df=data, 
                                         test_size=self.__test_size, 
                                         shuffle=self.__shuffle, 
                                         random_state=self.__random_state)
-        
+
         X_train, y_train = train[self.__features], train[self.__target]
-        model_ = self.__model.fit(X=X_train, y=y_train)
-        y_pred = model_.predict(X_train)
-        
-        if self.__df[self.__target].dtype == 'float64':
-            self.__type = 'regression'
-            if verbose:
-                report_df = self.__reg_metrics(y_train, y_pred)
-                display(report_df)
-                
-        else:
-            self.__type = 'classification'
-            if verbose:
-                matrix = self.__conf_matrix(y_train, y_pred)
-                report_df = self.__clf_metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
-                display(report_df)
-            
-        self.__fitted_model = model_
+
+        for model in self.__models:
+            fitted_model = model.fit(X=X_train, y=y_train)
+            self.fitted_models_dict[model.__class__.__name__] = fitted_model
+
+            y_pred = fitted_model.predict(X_train)
+
+            if self.__type == 'regression':
+                if verbose:
+                    report_df = self.__reg_metrics(y_train, y_pred)
+                    display(report_df)
+            else:
+                if verbose:
+                    matrix = self.__conf_matrix(y_train, y_pred)
+                    report_df = self.__clf_metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
+                    display(report_df)
+
         self.__train = train
         self.__test = test
             
     def evaluate(self, verbose=True):
         """
-        Evaluate the trained machine learning model using the test data.
+        Evaluates the fitted machine learning models on the test data.
 
         Args:
-            verbose (bool, optional): Whether to display performance metrics. Defaults to True.
-
-        Returns:
-            trained_model: The trained machine learning model.
-
-        Raises:
-            VariableNotInitializedError: If `fit()` has not been executed before calling `evaluate()`.
+            verbose (bool, optional): Whether to display verbose output during evaluation. Defaults to True.
         """
-        if self.__fitted_model == None:
-            raise VariableNotInitializedError("model", suggestion="Try fitting it first using `fit()` method.")
+        if self.fitted_models_dict is None or len(self.fitted_models_dict) == 0:
+            raise VariableNotInitializedError("models", suggestion="Try fitting it first using `fit()` method.")
 
         X_test, y_test = self.__test[self.__features], self.__test[self.__target]
-        y_pred = self.__fitted_model.predict(X_test)
         
-        if self.__type == 'regression':
-            if verbose:
-                report_df = self.__reg_metrics(y_test, y_pred)
-                display(report_df)
+        results_list = []
+        
+        for fitted_model in self.fitted_models_dict.values():
+            y_pred = fitted_model.predict(X_test)
+
+            if self.__type == 'regression':
+                metrics_df = self.__reg_metrics(y_test, y_pred)
+                metrics_df.insert(0, 'Model',fitted_model.__class__.__name__)
+                results_list.append(metrics_df)
                 
-        elif self.__type == 'classification':
-            if verbose:
+                if verbose:
+                    display(metrics_df.drop('Model', axis=1))
+                    
+            elif self.__type == 'classification':
                 matrix = self.__conf_matrix(y_test, y_pred)
                 report_df = self.__clf_metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
-                display(report_df)
+                    
+                metrics_df = pd.DataFrame(data={'Model':[fitted_model.__class__.__name__],
+                                                'Accuracy':[report_df['Accuracy'][0]]})
+                results_list.append(metrics_df)
                 
-        return self.__fitted_model
+                if verbose:
+                    display(report_df)
+        
+            res_df = pd.concat(results_list)
+        self.results_df = res_df.sort_values(by=res_df.columns[1], ascending=True if self.__type == 'regression' else False).reset_index(drop=True)
```

