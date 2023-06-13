# Comparing `tmp/fsrs4anki_optimizer-3.24.0.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.0.tar", last modified: Sat Jun 10 13:45:30 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.1.tar", last modified: Tue Jun 13 02:50:55 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.0.tar` & `fsrs4anki_optimizer-3.24.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.223906 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.048592 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43250 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         # pretrain
         best_loss = np.inf
         weighted_loss, w = self.eval()
         if weighted_loss < best_loss:
             best_loss = weighted_loss
             best_w = w
 
-        pbar = tqdm(desc="pre-train", colour="red", total=len(self.pre_train_data_loader) * self.n_epoch, )
+        pbar = tqdm(desc="pre-train", colour="red", total=len(self.pre_train_data_loader) * self.n_epoch)
         for k in range(self.n_epoch):
             for i, batch in enumerate(self.pre_train_data_loader):
                 self.model.train()
                 self.optimizer.zero_grad()
                 sequences, delta_ts, labels, seq_lens = batch
                 real_batch_size = seq_lens.shape[0]
                 outputs, _ = self.model(sequences)
@@ -488,34 +488,34 @@
         self.w = avg_w.tolist()
 
         print("\nTraining finished!")
         return plots
 
     def preview(self, requestRetention: float):
         my_collection = Collection(self.w)
-        print("1:again, 2:hard, 3:good, 4:easy\n")
+        preview_text = "1:again, 2:hard, 3:good, 4:easy\n"
         for first_rating in (1,2,3,4):
-            print(f'first rating: {first_rating}')
+            preview_text += f'\nfirst rating: {first_rating}\n'
             t_history = "0"
             d_history = "0"
             r_history = f"{first_rating}"  # the first rating of the new card
             # print("stability, difficulty, lapses")
             for i in range(10):
                 states = my_collection.predict(t_history, r_history)
                 # print('{0:9.2f} {1:11.2f} {2:7.0f}'.format(
                     # *list(map(lambda x: round(float(x), 4), states))))
                 next_t = max(round(float(np.log(requestRetention)/np.log(0.9) * states[0])), 1)
                 difficulty = round(float(states[1]), 1)
                 t_history += f',{int(next_t)}'
                 d_history += f',{difficulty}'
                 r_history += f",3"
-            print(f"rating history: {r_history}")
-            print("interval history: " + ",".join([f"{ivl}d" if ivl < 30 else f"{ivl / 30:.1f}m" if ivl < 365 else f"{ivl / 365:.1f}y" for ivl in map(int, t_history.split(','))]))
-            print(f"difficulty history: {d_history}")
-            print('')
+            preview_text += f"rating history: {r_history}\n"
+            preview_text += "interval history: " + ",".join([f"{ivl}d" if ivl < 30 else f"{ivl / 30:.1f}m" if ivl < 365 else f"{ivl / 365:.1f}y" for ivl in map(int, t_history.split(','))]) + "\n"
+            preview_text += f"difficulty history: {d_history}\n"
+        return preview_text
 
     def preview_sequence(self, test_rating_sequence: str, requestRetention: float, easyBonus: float, hardInterval: float):
         my_collection = Collection(self.w)
 
         t_history = "0"
         d_history = "0"
         for i in range(len(test_rating_sequence.split(','))):
@@ -528,17 +528,18 @@
             if rating == '4':
                 next_t = round(next_t * easyBonus)
             elif rating == '2':
                 next_t = round(last_t * hardInterval)
             t_history += f',{int(next_t)}'
             difficulty = round(float(states[1]), 1)
             d_history += f',{difficulty}'
-        print(f"rating history: {test_rating_sequence}")
-        print(f"interval history: {t_history}")
-        print(f"difficulty history: {d_history}")
+        preview_text = f"rating history: {test_rating_sequence}\n"
+        preview_text += f"interval history: {t_history}\n"
+        preview_text += f"difficulty history: {d_history}"
+        return preview_text
 
     def predict_memory_states(self):
         my_collection = Collection(self.w)
 
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         stabilities = map(lambda x: round(x, 2), stabilities)
         difficulties = map(lambda x: round(x, 2), difficulties)
@@ -548,19 +549,19 @@
         prediction.reset_index(inplace=True)
         prediction.sort_values(by=['r_history'], inplace=True)
         prediction.rename(columns={"id": "count"}, inplace=True)
         prediction.to_csv("./prediction.tsv", sep='\t', index=None)
         print("prediction.tsv saved.")
         prediction['difficulty'] = prediction['difficulty'].map(lambda x: int(round(x)))
         self.difficulty_distribution = prediction.groupby(by=['difficulty'])['count'].sum() / prediction['count'].sum()
-        print(self.difficulty_distribution)
         self.difficulty_distribution_padding = np.zeros(10)
         for i in range(10):
             if i+1 in self.difficulty_distribution.index:
                 self.difficulty_distribution_padding[i] = self.difficulty_distribution.loc[i+1]
+        return self.difficulty_distribution
     
     def find_optimal_retention(self):
         """should not be called before predict_memory_states"""
 
         base = 1.01
         index_len = 664
         index_offset = 200
@@ -664,32 +665,33 @@
     def evaluate(self):
         my_collection = Collection(self.init_w)
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         self.dataset['stability'] = stabilities
         self.dataset['difficulty'] = difficulties
         self.dataset['p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['stability'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['p']) if row['y'] == 1 else - np.log(1 - row['p']), axis=1)
-        print(f"Loss before training: {self.dataset['log_loss'].mean():.4f}")
+        loss_before = self.dataset['log_loss'].mean()
 
         my_collection = Collection(self.w)
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         self.dataset['stability'] = stabilities
         self.dataset['difficulty'] = difficulties
         self.dataset['p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['stability'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['p']) if row['y'] == 1 else - np.log(1 - row['p']), axis=1)
-        print(f"Loss after training: {self.dataset['log_loss'].mean():.4f}")
+        loss_after = self.dataset['log_loss'].mean()
 
         tmp = self.dataset.copy()
         tmp['stability'] = tmp['stability'].map(lambda x: round(x, 2))
         tmp['difficulty'] = tmp['difficulty'].map(lambda x: round(x, 2))
         tmp['p'] = tmp['p'].map(lambda x: round(x, 2))
         tmp['log_loss'] = tmp['log_loss'].map(lambda x: round(x, 2))
         tmp.rename(columns={"r": "grade", "p": "retrievability"}, inplace=True)
         tmp[['id', 'cid', 'review_date', 'r_history', 't_history', 'delta_t', 'grade', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
         del tmp
+        return loss_before, loss_after
 
     def calibration_graph(self):
         fig1 = plot_brier(self.dataset['p'], self.dataset['y'], bins=40)
 
         def to_percent(temp, position):
             return '%1.0f' % (100 * temp) + '%'
```

